# Comparing `tmp/extract_office_content-0.0.4-py3-none-any.whl.zip` & `tmp/extract_office_content-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10708 bytes, number of entries: 11
--rw-r--r--  2.0 unx      227 b- defN 23-Jun-17 07:05 extract_office_content/__init__.py
--rw-r--r--  2.0 unx     4475 b- defN 23-Jun-17 07:05 extract_office_content/extract_excel.py
--rw-r--r--  2.0 unx     4186 b- defN 23-Jun-17 07:05 extract_office_content/extract_ppt.py
--rw-r--r--  2.0 unx     6492 b- defN 23-Jun-17 07:05 extract_office_content/extract_word.py
--rw-r--r--  2.0 unx     2265 b- defN 23-Jun-17 07:05 extract_office_content/main.py
--rw-r--r--  2.0 unx      973 b- defN 23-Jun-17 07:05 extract_office_content/utils.py
--rw-r--r--  2.0 unx     5316 b- defN 23-Jun-17 07:06 extract_office_content-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 07:06 extract_office_content-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx      245 b- defN 23-Jun-17 07:06 extract_office_content-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-17 07:06 extract_office_content-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1018 b- defN 23-Jun-17 07:06 extract_office_content-0.0.4.dist-info/RECORD
-11 files, 25312 bytes uncompressed, 8946 bytes compressed:  64.7%
+Zip file size: 10700 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      227 b- defN 23-Jul-02 09:11 extract_office_content/__init__.py
+-rw-r--r--  2.0 unx     4444 b- defN 23-Jul-02 09:11 extract_office_content/extract_excel.py
+-rw-r--r--  2.0 unx     4174 b- defN 23-Jul-02 09:11 extract_office_content/extract_ppt.py
+-rw-r--r--  2.0 unx     6505 b- defN 23-Jul-02 09:11 extract_office_content/extract_word.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-Jul-02 09:11 extract_office_content/main.py
+-rw-r--r--  2.0 unx      969 b- defN 23-Jul-02 09:11 extract_office_content/utils.py
+-rw-r--r--  2.0 unx     5315 b- defN 23-Jul-02 09:12 extract_office_content-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 09:12 extract_office_content-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx      245 b- defN 23-Jul-02 09:12 extract_office_content-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-02 09:12 extract_office_content-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1018 b- defN 23-Jul-02 09:12 extract_office_content-0.0.5.dist-info/RECORD
+11 files, 25287 bytes uncompressed, 8938 bytes compressed:  64.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: extract_office_content/main.py
 Comment: 
 
 Filename: extract_office_content/utils.py
 Comment: 
 
-Filename: extract_office_content-0.0.4.dist-info/METADATA
+Filename: extract_office_content-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: extract_office_content-0.0.4.dist-info/WHEEL
+Filename: extract_office_content-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: extract_office_content-0.0.4.dist-info/entry_points.txt
+Filename: extract_office_content-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: extract_office_content-0.0.4.dist-info/top_level.txt
+Filename: extract_office_content-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: extract_office_content-0.0.4.dist-info/RECORD
+Filename: extract_office_content-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## extract_office_content/extract_excel.py

```diff
@@ -13,37 +13,41 @@
 import openpyxl
 import pandas as pd
 from openpyxl.workbook.workbook import Workbook
 
 from .utils import mkdir
 
 
-class ExtractExcel():
-    def __init__(self,):
+class ExtractExcel:
+    def __init__(
+        self,
+    ):
         self.img_suffix = [".jpg", ".jpeg", ".png", ".bmp"]
 
-    def __call__(self, excel_content: Union[str, Path, bytes],
-                 out_format: str = 'markdown',
-                 save_img_dir: str = None) -> List:
-
+    def __call__(
+        self,
+        excel_content: Union[str, Path, bytes],
+        out_format: str = "markdown",
+        save_img_dir: str = None,
+    ) -> List:
         if isinstance(excel_content, (str, Path)):
             if not Path(excel_content).exists():
-                raise FileNotFoundError(f'{excel_content} does not exist.')
+                raise FileNotFoundError(f"{excel_content} does not exist.")
             excel_content = str(excel_content)
         elif isinstance(excel_content, bytes):
             excel_content = BytesIO(excel_content)
 
         wb = self.unmerge_cell(excel_content)
         data_table = self.extract_table(wb, out_format)
 
         if save_img_dir:
             try:
                 self.extract_imgs(excel_content, save_img_dir)
             except FileExistsError:
-                warnings.warn(f'The {excel_content} does not contain any images.')
+                warnings.warn(f"The {excel_content} does not contain any images.")
 
         return data_table
 
     def unmerge_cell(self, file_name: str) -> Workbook:
         wb = openpyxl.load_workbook(file_name)
         for sheet_name in wb.sheetnames:
             sheet = wb[sheet_name]
@@ -64,64 +68,70 @@
             for row_index, col_index in merged_cell_range.cells:
                 cell = worksheet.cell(row=row_index, column=col_index)
                 cell.value = merged_cell.value
 
     def extract_table(self, wb: Workbook, out_format: str) -> List:
         sheet_names = wb.sheetnames
         with tempfile.TemporaryDirectory() as tmp_dir:
-            tmp_save_path = Path(tmp_dir) / f'{uuid.uuid1()}.xlsx'
+            tmp_save_path = Path(tmp_dir) / f"{uuid.uuid1()}.xlsx"
             wb.save(str(tmp_save_path))
             wb.close()
 
             df_datas = []
             for name in sheet_names:
-                data = pd.read_excel(tmp_save_path, index_col=None,
-                                     sheet_name=name)
+                data = pd.read_excel(tmp_save_path, index_col=None, sheet_name=name)
                 cvt_data = self.convert_table(data, out_format)
                 df_datas.append(cvt_data)
         return df_datas
 
     @staticmethod
-    def convert_table(df_table: pd.core.frame.DataFrame,
-                      out_format: str) -> str:
-        if 'to_' not in out_format:
-            out_format = f'to_{out_format}'
+    def convert_table(df_table: pd.core.frame.DataFrame, out_format: str) -> str:
+        if "to_" not in out_format:
+            out_format = f"to_{out_format}"
 
         try:
             return getattr(df_table, out_format)()
         except AttributeError as exc:
-            raise AttributeError(f'{out_format} is not supported.') from exc
+            raise AttributeError(f"{out_format} is not supported.") from exc
 
-    def extract_imgs(self, excel_content: Union[str, Path, bytes],
-                     save_img_dir: Union[str, Path]) -> None:
+    def extract_imgs(
+        self, excel_content: Union[str, Path, bytes], save_img_dir: Union[str, Path]
+    ) -> None:
         with zipfile.ZipFile(excel_content) as zf:
             file_list = zf.namelist()
 
-            img_list = [path for path in file_list
-                        if Path(path).suffix in self.img_suffix]
+            img_list = [
+                path for path in file_list if Path(path).suffix in self.img_suffix
+            ]
 
             if not img_list:
-                raise FileExistsError('The xl/media is not existed.')
+                raise FileExistsError("The xl/media is not existed.")
 
             mkdir(save_img_dir)
             for img_path in img_list:
                 save_path = Path(save_img_dir) / Path(img_path).name
-                with open(save_path, 'wb') as f:
+                with open(save_path, "wb") as f:
                     f.write(zf.read(img_path))
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('excel_path', type=str)
-    parser.add_argument('-f', '--output_format', type=str, default='markdown',
-                        choices=['markdown', 'html', 'latex', 'string'])
-    parser.add_argument('-o', '--save_img_dir', type=str, default=None)
+    parser.add_argument("excel_path", type=str)
+    parser.add_argument(
+        "-f",
+        "--output_format",
+        type=str,
+        default="markdown",
+        choices=["markdown", "html", "latex", "string"],
+    )
+    parser.add_argument("-o", "--save_img_dir", type=str, default=None)
     args = parser.parse_args()
 
     excel_extract = ExtractExcel()
-    res = excel_extract(args.excel_path, out_format=args.output_format,
-                        save_img_dir=args.save_img_dir)
+    res = excel_extract(
+        args.excel_path, out_format=args.output_format, save_img_dir=args.save_img_dir
+    )
     print(res)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

## extract_office_content/extract_ppt.py

```diff
@@ -9,52 +9,55 @@
 import pandas as pd
 import pptx
 from pptx import Presentation
 
 from .utils import mkdir
 
 
-class ExtractPPT():
-    def __init__(self, ):
+class ExtractPPT:
+    def __init__(
+        self,
+    ):
         pass
 
-    def __call__(self, ppt_content: Union[str, bytes],
-                 save_img_dir: str = None) -> List:
+    def __call__(
+        self, ppt_content: Union[str, bytes], save_img_dir: str = None
+    ) -> List:
         """Extract content and images of ppt.
 
         Args:
             ppt_content (str, bytes): the path of ppt.
             save_img_dir (str, optional): The directory for saving images. Defaults to None.
 
         Returns:
             List: txts from pptx.
         """
         if isinstance(ppt_content, str):
             if not Path(ppt_content).exists():
-                raise FileNotFoundError(f'{ppt_content} does not exist.')
+                raise FileNotFoundError(f"{ppt_content} does not exist.")
         elif isinstance(ppt_content, bytes):
             ppt_content = BytesIO(ppt_content)
 
         txts, imgs, charts = self.extract_all(ppt_content)
         if save_img_dir:
             if imgs:
-                self.save_object(imgs, save_img_dir, suffix='png')
+                self.save_object(imgs, save_img_dir, suffix="png")
 
             if charts:
-                self.save_object(charts, save_img_dir, suffix='xlsx')
+                self.save_object(charts, save_img_dir, suffix="xlsx")
         return list(txts.values())
 
     def extract_all(self, ppt_path: Union[str, bytes]) -> Tuple[Dict, Dict]:
         prs = Presentation(ppt_path)
         extract_txts, extract_imgs, extract_charts = {}, {}, {}
         for i, slide in enumerate(prs.slides):
             cur_page = i + 1
             cur_txts, cur_imgs, cur_charts = self.extract_one(slide)
 
-            extract_txts[cur_page] = '\n'.join(cur_txts)
+            extract_txts[cur_page] = "\n".join(cur_txts)
             extract_imgs.update({cur_page: cur_imgs})
             extract_charts.update({cur_page: cur_charts})
         return extract_txts, extract_imgs, extract_charts
 
     def extract_one(self, slide: pptx.slide.Slide) -> Tuple[List, List, List]:
         cur_page_content, cur_page_imgs, cur_page_charts = [], [], []
         for shape in slide.shapes:
@@ -64,15 +67,15 @@
                     cur_page_content.append(txt)
             elif shape.has_table:
                 table_str = self.extract_table(shape.table)
                 cur_page_content.append(table_str)
             elif shape.has_chart:
                 excel_bytes = shape.chart.part.chart_workbook.xlsx_part.blob
                 cur_page_charts.append(excel_bytes)
-            elif hasattr(shape, 'image'):
+            elif hasattr(shape, "image"):
                 img_bytes = self.extract_image(shape.image)
                 cur_page_imgs.append(img_bytes)
             else:
                 pass
         return cur_page_content, cur_page_imgs, cur_page_charts
 
     @staticmethod
@@ -82,42 +85,41 @@
             return txt
         return None
 
     @staticmethod
     def extract_table(table_value: pptx.table.Table) -> str:
         table_list = []
         for one_row in table_value.rows:
-            each = ''
+            each = ""
             for cell in one_row.cells:
-                each += cell.text_frame.text + ','
+                each += cell.text_frame.text + ","
             table_list.append(each)
         table_df = pd.DataFrame(table_list)
         return table_df.to_markdown(index=None)
 
     @staticmethod
     def extract_image(img_value: pptx.parts.image.Image) -> bytes:
         return img_value.blob
 
     @staticmethod
-    def save_object(objs: Dict,
-                    save_dir: Union[str, Path], suffix: str) -> None:
+    def save_object(objs: Dict, save_dir: Union[str, Path], suffix: str) -> None:
         mkdir(save_dir)
         for page_num, obj_list in objs.items():
             for i, img in enumerate(obj_list):
-                save_full_path = Path(save_dir) / f'{page_num}_{i+1}.{suffix}'
-                with open(str(save_full_path), 'wb') as f:
+                save_full_path = Path(save_dir) / f"{page_num}_{i+1}.{suffix}"
+                with open(str(save_full_path), "wb") as f:
                     f.write(img)
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('ppt_path', type=str)
-    parser.add_argument('-img_dir', '--save_img_dir', type=str, default=None)
+    parser.add_argument("ppt_path", type=str)
+    parser.add_argument("-img_dir", "--save_img_dir", type=str, default=None)
     args = parser.parse_args()
 
     ppt_extracter = ExtractPPT()
     res = ppt_extracter(args.ppt_path, save_img_dir=args.save_img_dir)
     print(res)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

## extract_office_content/extract_word.py

```diff
@@ -14,132 +14,138 @@
 from docx.document import Document
 from docx.oxml.table import CT_Tbl
 from docx.table import Table, _Cell
 
 from .utils import is_contain, mkdir
 
 
-class ExtractWord():
-    def __init__(self, ):
+class ExtractWord:
+    def __init__(
+        self,
+    ):
         self.img_suffix = [".jpg", ".jpeg", ".png", ".bmp"]
         self.nsmap = {
-            'w': 'http://schemas.openxmlformats.org/wordprocessingml/2006/main'
+            "w": "http://schemas.openxmlformats.org/wordprocessingml/2006/main"
         }
         self.extract_table = ExtractWordTable()
         self.parser = etree.XMLParser()
 
     def __call__(self, docx_content: Union[str, bytes], save_img_dir=None):
         if isinstance(docx_content, str) and not Path(docx_content).exists():
-            raise FileNotFoundError(f'{docx_content} does not exist.')
+            raise FileNotFoundError(f"{docx_content} does not exist.")
         elif isinstance(docx_content, bytes):
             docx_content = BytesIO(docx_content)
 
         self.table_content = self.extract_table(docx_content)
-        text = ''
+        text = ""
 
         # unzip the docx_content in memory
         zipf = zipfile.ZipFile(docx_content)
         filelist = zipf.namelist()
 
         header_files, footer_files, img_files = [], [], []
-        header_xmls = 'word/header[0-9]*.xml'
-        footer_xmls = 'word/footer[0-9]*.xml'
+        header_xmls = "word/header[0-9]*.xml"
+        footer_xmls = "word/footer[0-9]*.xml"
 
         for fname in filelist:
             if re.match(header_xmls, fname):
                 header_files.append(fname)
             elif re.match(footer_xmls, fname):
                 footer_files.append(fname)
             elif Path(fname).suffix.lower() in self.img_suffix:
                 img_files.append(fname)
             else:
                 continue
 
         # get header text
         # there can be 3 header files in the zip
         header_text = [self.xml2text(zipf.read(path)) for path in header_files]
-        text += ''.join(header_text)
+        text += "".join(header_text)
 
         # get main text
-        doc_xml = 'word/document.xml'
+        doc_xml = "word/document.xml"
         main_txt = self.xml2text(zipf.read(doc_xml))
         text += main_txt
 
         # get footer text
         # there can be 3 footer files in the zip
         footer_text = [self.xml2text(zipf.read(path)) for path in footer_files]
-        text += ''.join(footer_text)
+        text += "".join(footer_text)
 
         if save_img_dir:
             mkdir(save_img_dir)
             for img_path in img_files:
                 dst_fname = Path(save_img_dir) / Path(img_path).name
                 with open(dst_fname, "wb") as dst_f:
                     dst_f.write(zipf.read(img_path))
         zipf.close()
-        return text.strip() + '\n'.join(self.table_content)
+        return text.strip() + "\n".join(self.table_content)
 
     def qn(self, tag):
         """
         Stands for 'qualified name', a utility function to turn a namespace
         prefixed tag name into a Clark-notation qualified tag name for lxml. For
         example, ``qn('p:cSld')`` returns ``'{http://schemas.../main}cSld'``.
         Source: https://github.com/python-openxml/python-docx/
         """
-        prefix, tagroot = tag.split(':')
+        prefix, tagroot = tag.split(":")
         uri = self.nsmap[prefix]
-        return f'{{{uri}}}{tagroot}'
+        return f"{{{uri}}}{tagroot}"
 
     def xml2text(self, xml):
         """
         A string representing the textual content of this run, with content
         child elements like ``<w:tab/>`` translated to their Python
         equivalent.
         Adapted from: https://github.com/python-openxml/python-docx/
         """
-        text = ''
+        text = ""
         table_xml = self.extract_table_by_xml(xml_path=xml)
 
         root = ET.fromstring(xml)
         for child in root.iter():
-            if child.tag == self.qn('w:t'):
+            if child.tag == self.qn("w:t"):
                 t_text = child.text
                 if t_text in table_xml:
                     continue
 
-                text += t_text if t_text is not None else ''
-            elif child.tag == self.qn('w:tab'):
-                text += '\t'
-            elif child.tag in (self.qn('w:br'), self.qn('w:cr')):
-                text += '\n'
+                text += t_text if t_text is not None else ""
+            elif child.tag == self.qn("w:tab"):
+                text += "\t"
+            elif child.tag in (self.qn("w:br"), self.qn("w:cr")):
+                text += "\n"
             elif child.tag == self.qn("w:p"):
-                text += '\n\n'
+                text += "\n\n"
         return text
 
-    def extract_table_by_xml(self, xml_path: str,) -> str:
+    def extract_table_by_xml(
+        self,
+        xml_path: str,
+    ) -> str:
         tree = etree.fromstring(xml_path, self.parser)
-        table_txts = tree.xpath('//w:tbl//w:t/text()',
-                                namespaces=self.nsmap)
+        table_txts = tree.xpath("//w:tbl//w:t/text()", namespaces=self.nsmap)
         return table_txts
 
 
-class ExtractWordTable():
-    def __init__(self,):
+class ExtractWordTable:
+    def __init__(
+        self,
+    ):
         pass
 
     def __call__(self, docx_content):
         curr_content = []
         doc = docx.Document(docx_content)
         for block in self.iter_block_items(doc):
-            if is_contain(block.style.name, ['Table', 'Table Grid']):
+            if is_contain(block.style.name, ["Table", "Table Grid"]):
                 df = self.get_table_dataframe(block)
                 try:
-                    curr_content.append(f'\n{df.to_markdown()}')
+                    curr_content.append(f"\n{df.to_markdown()}")
                 except:
-                    curr_content.append(f'\n{df}')
+                    curr_content.append(f"\n{df}")
         return curr_content
 
     def iter_block_items(self, parent):
         if isinstance(parent, Document):
             # 判断传入的是否为word文档对象，是则获取文档内容的全部子对象
             parent_elm = parent.element.body
         elif isinstance(parent, _Cell):
@@ -149,15 +155,15 @@
             raise ValueError("something's not right")
 
         for child in parent_elm.iterchildren():
             if isinstance(child, CT_Tbl):
                 yield Table(child, parent)
 
     def get_table_dataframe(self, table: docx.table.Table) -> pd.DataFrame:
-        '''获取表格数据，转换为dataframe数据结构'''
+        """获取表格数据，转换为dataframe数据结构"""
         text = []
         if len(table.rows) == 1:
             for i in table.rows[0].cells:
                 text.append(i.text)
             return text[-1]
 
         keys, table_data = None, []
@@ -173,18 +179,18 @@
             table_data.append(dict(zip(keys, text)))
         df = pd.DataFrame(table_data)
         return df
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('word_path', type=str)
-    parser.add_argument('-img_dir', '--save_img_dir', type=str, default=None)
+    parser.add_argument("word_path", type=str)
+    parser.add_argument("-img_dir", "--save_img_dir", type=str, default=None)
     args = parser.parse_args()
 
     word_extract = ExtractWord()
     res = word_extract(args.word_path, save_img_dir=args.save_img_dir)
     print(res)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

## extract_office_content/main.py

```diff
@@ -7,35 +7,34 @@
 from pathlib import Path
 
 from .extract_excel import ExtractExcel
 from .extract_ppt import ExtractPPT
 from .extract_word import ExtractWord
 
 
-class ExtractOfficeContent():
+class ExtractOfficeContent:
     def __init__(self) -> None:
         self.excel = ExtractExcel()
         self.ppt = ExtractPPT()
         self.word = ExtractWord()
 
-        self.doc_suffix = ['doc', 'docx']
-        self.excel_suffix = ['xls', 'xlsx']
-        self.ppt_suffix = ['ppt', 'pptx']
+        self.doc_suffix = ["doc", "docx"]
+        self.excel_suffix = ["xls", "xlsx"]
+        self.ppt_suffix = ["ppt", "pptx"]
 
-    def __call__(self, file_content: Union[Path, str],
-                 save_img_dir: str = None):
+    def __call__(self, file_content: Union[Path, str], save_img_dir: str = None):
         file_content = str(file_content)
 
         if not file_content:
-            raise ValueError(f'{file_content} must be Path or str.')
+            raise ValueError(f"{file_content} must be Path or str.")
 
         file_type = self.which_type(file_content)
         all_suffix = self.doc_suffix + self.excel_suffix + self.ppt_suffix
         if file_type not in all_suffix:
-            raise ValueError(f'{file_type} must in {all_suffix}')
+            raise ValueError(f"{file_type} must in {all_suffix}")
 
         if file_type in self.doc_suffix:
             return self.word(file_content, save_img_dir)
 
         if file_type in self.excel_suffix:
             return self.excel(file_content, save_img_dir=save_img_dir)
 
@@ -43,34 +42,38 @@
             return self.ppt(file_content, save_img_dir)
 
     def which_type(self, file_content: Union[str, Path]):
         if isinstance(file_content, str):
             return filetype.guess(file_content).extension
 
         if isinstance(file_content, bytes):
-            with open(file_content, 'rb') as f:
+            with open(file_content, "rb") as f:
                 data = f.read()
 
             return filetype.guess(data).extension
 
-        raise ValueError(f'{file_content} must be [str, Path] type.')
+        raise ValueError(f"{file_content} must be [str, Path] type.")
 
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('file_path', type=str)
-    parser.add_argument('-img_dir', '--save_img_dir', type=str, )
+    parser.add_argument("file_path", type=str)
+    parser.add_argument(
+        "-img_dir",
+        "--save_img_dir",
+        type=str,
+    )
     args = parser.parse_args()
 
     extracter = ExtractOfficeContent()
     if Path(args.file_path).is_dir():
         file_list = list(Path(args.file_path).iterdir())
     else:
         file_list = [args.file_path]
 
     for file_one in file_list:
         res = extracter(str(file_one))
         print(res)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

## extract_office_content/utils.py

```diff
@@ -9,28 +9,30 @@
     Path(dir_path).mkdir(parents=True, exist_ok=True)
 
 
 def read_txt(txt_path: str) -> List:
     if not isinstance(txt_path, str):
         txt_path = str(txt_path)
 
-    with open(txt_path, 'r', encoding='utf-8') as f:
-        data = list(map(lambda x: x.rstrip('\n'), f))
+    with open(txt_path, "r", encoding="utf-8") as f:
+        data = list(map(lambda x: x.rstrip("\n"), f))
     return data
 
 
-def write_txt(save_path: Union[str, Path],
-              content: list, mode: str = 'w'):
+def write_txt(save_path: Union[str, Path], content: list, mode: str = "w"):
     if not isinstance(save_path, str):
         save_path = str(save_path)
 
     if not isinstance(content, list):
         content = [content]
 
-    with open(save_path, mode, encoding='utf-8') as f:
+    with open(save_path, mode, encoding="utf-8") as f:
         for value in content:
-            f.write(f'{value}\n')
+            f.write(f"{value}\n")
 
 
-def is_contain(sentence: str, key_words: Union[str, List],) -> bool:
+def is_contain(
+    sentence: str,
+    key_words: Union[str, List],
+) -> bool:
     """sentences中是否包含key_words中任意一个"""
     return any(i in sentence for i in key_words)
```

## Comparing `extract_office_content-0.0.4.dist-info/METADATA` & `extract_office_content-0.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extract-office-content
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tool for extracting content from office files.
 Home-page: https://github.com/SWHL/ExtractOfficeText.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: extract,office,text,content
 Platform: Any
@@ -113,15 +113,14 @@
             res = extracter(file_path)
             print(res)
         ```
     - Extract Word.
         ```python
         from extract_office_content import ExtractWord
 
-
         word_extract = ExtractWord()
 
         word_path = 'tests/test_files/word_example.docx'
         text = word_extract(word_path, "outputs/word")
 
         # or bytes
         with open(word_path, 'rb') as f:
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: extract-office-content Version: 0.0.4 Summary: Tool
+Metadata-Version: 2.1 Name: extract-office-content Version: 0.0.5 Summary: Tool
 for extracting content from office files. Home-page: https://github.com/SWHL/
 ExtractOfficeText.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: extract,office,text,content Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Python: >=3.6,<=3.11 Description-Content-Type: text/
```

