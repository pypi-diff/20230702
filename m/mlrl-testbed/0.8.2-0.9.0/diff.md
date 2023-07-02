# Comparing `tmp/mlrl_testbed-0.8.2-py3-none-any.whl.zip` & `tmp/mlrl_testbed-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,30 @@
-Zip file size: 38765 bytes, number of entries: 22
--rw-r--r--  2.0 unx        0 b- defN 22-Apr-11 18:31 mlrl/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 22-Apr-11 18:31 mlrl/testbed/__init__.py
--rw-r--r--  2.0 unx    13467 b- defN 22-Apr-11 18:31 mlrl/testbed/args.py
--rw-r--r--  2.0 unx    15259 b- defN 22-Apr-11 18:31 mlrl/testbed/bbc_cv.py
--rw-r--r--  2.0 unx    19973 b- defN 22-Apr-11 18:31 mlrl/testbed/data.py
--rw-r--r--  2.0 unx    11725 b- defN 22-Apr-11 18:31 mlrl/testbed/data_characteristics.py
--rw-r--r--  2.0 unx    20311 b- defN 22-Apr-11 18:31 mlrl/testbed/evaluation.py
--rw-r--r--  2.0 unx     8977 b- defN 22-Apr-11 18:31 mlrl/testbed/experiments.py
--rw-r--r--  2.0 unx      373 b- defN 22-Apr-11 18:31 mlrl/testbed/interfaces.py
--rw-r--r--  2.0 unx     5535 b- defN 22-Apr-11 18:31 mlrl/testbed/io.py
--rw-r--r--  2.0 unx     7134 b- defN 22-Apr-11 18:31 mlrl/testbed/main_boomer.py
--rw-r--r--  2.0 unx    25874 b- defN 22-Apr-11 18:31 mlrl/testbed/model_characteristics.py
--rw-r--r--  2.0 unx    10207 b- defN 22-Apr-11 18:31 mlrl/testbed/parameters.py
--rw-r--r--  2.0 unx     3016 b- defN 22-Apr-11 18:31 mlrl/testbed/persistence.py
--rw-r--r--  2.0 unx     5692 b- defN 22-Apr-11 18:31 mlrl/testbed/runnables.py
--rw-r--r--  2.0 unx     7717 b- defN 22-Apr-11 18:31 mlrl/testbed/training.py
--rw-r--r--  2.0 unx     3833 b- defN 22-Apr-11 18:31 mlrl_testbed-0.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Apr-11 18:31 mlrl_testbed-0.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx      108 b- defN 22-Apr-11 18:31 mlrl_testbed-0.8.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 22-Apr-11 18:31 mlrl_testbed-0.8.2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Apr-11 18:31 mlrl_testbed-0.8.2.dist-info/zip-safe
-?rw-rw-r--  2.0 unx     1822 b- defN 22-Apr-11 18:31 mlrl_testbed-0.8.2.dist-info/RECORD
-22 files, 161121 bytes uncompressed, 35809 bytes compressed:  77.8%
+Zip file size: 52188 bytes, number of entries: 28
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 16:27 mlrl/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 16:27 mlrl/testbed/__init__.py
+-rw-r--r--  2.0 unx     6126 b- defN 23-Jul-02 16:27 mlrl/testbed/characteristics.py
+-rw-r--r--  2.0 unx    21950 b- defN 23-Jul-02 16:27 mlrl/testbed/data.py
+-rw-r--r--  2.0 unx     6667 b- defN 23-Jul-02 16:27 mlrl/testbed/data_characteristics.py
+-rw-r--r--  2.0 unx    18816 b- defN 23-Jul-02 16:27 mlrl/testbed/data_splitting.py
+-rw-r--r--  2.0 unx    20458 b- defN 23-Jul-02 16:27 mlrl/testbed/evaluation.py
+-rw-r--r--  2.0 unx    20423 b- defN 23-Jul-02 16:27 mlrl/testbed/experiments.py
+-rw-r--r--  2.0 unx     5043 b- defN 23-Jul-02 16:27 mlrl/testbed/format.py
+-rw-r--r--  2.0 unx     5691 b- defN 23-Jul-02 16:27 mlrl/testbed/io.py
+-rw-r--r--  2.0 unx     7102 b- defN 23-Jul-02 16:27 mlrl/testbed/label_vectors.py
+-rw-r--r--  2.0 unx      654 b- defN 23-Jul-02 16:27 mlrl/testbed/main_boomer.py
+-rw-r--r--  2.0 unx    14769 b- defN 23-Jul-02 16:27 mlrl/testbed/model_characteristics.py
+-rw-r--r--  2.0 unx     9108 b- defN 23-Jul-02 16:27 mlrl/testbed/models.py
+-rw-r--r--  2.0 unx    12656 b- defN 23-Jul-02 16:27 mlrl/testbed/output_writer.py
+-rw-r--r--  2.0 unx     3724 b- defN 23-Jul-02 16:27 mlrl/testbed/parameters.py
+-rw-r--r--  2.0 unx     2376 b- defN 23-Jul-02 16:27 mlrl/testbed/persistence.py
+-rw-r--r--  2.0 unx     2058 b- defN 23-Jul-02 16:27 mlrl/testbed/prediction_characteristics.py
+-rw-r--r--  2.0 unx     2279 b- defN 23-Jul-02 16:27 mlrl/testbed/prediction_scope.py
+-rw-r--r--  2.0 unx     4153 b- defN 23-Jul-02 16:27 mlrl/testbed/predictions.py
+-rw-r--r--  2.0 unx     9026 b- defN 23-Jul-02 16:27 mlrl/testbed/probability_calibration.py
+-rw-r--r--  2.0 unx    52453 b- defN 23-Jul-02 16:27 mlrl/testbed/runnables.py
+-rw-r--r--  2.0 unx     4694 b- defN 23-Jul-02 16:27 mlrl_testbed-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 16:27 mlrl_testbed-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 23-Jul-02 16:27 mlrl_testbed-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-Jul-02 16:27 mlrl_testbed-0.9.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-02 16:27 mlrl_testbed-0.9.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     2374 b- defN 23-Jul-02 16:27 mlrl_testbed-0.9.0.dist-info/RECORD
+28 files, 232764 bytes uncompressed, 48354 bytes compressed:  79.2%
```

## zipnote {}

```diff
@@ -1,67 +1,85 @@
 Filename: mlrl/__init__.py
 Comment: 
 
 Filename: mlrl/testbed/__init__.py
 Comment: 
 
-Filename: mlrl/testbed/args.py
-Comment: 
-
-Filename: mlrl/testbed/bbc_cv.py
+Filename: mlrl/testbed/characteristics.py
 Comment: 
 
 Filename: mlrl/testbed/data.py
 Comment: 
 
 Filename: mlrl/testbed/data_characteristics.py
 Comment: 
 
+Filename: mlrl/testbed/data_splitting.py
+Comment: 
+
 Filename: mlrl/testbed/evaluation.py
 Comment: 
 
 Filename: mlrl/testbed/experiments.py
 Comment: 
 
-Filename: mlrl/testbed/interfaces.py
+Filename: mlrl/testbed/format.py
 Comment: 
 
 Filename: mlrl/testbed/io.py
 Comment: 
 
+Filename: mlrl/testbed/label_vectors.py
+Comment: 
+
 Filename: mlrl/testbed/main_boomer.py
 Comment: 
 
 Filename: mlrl/testbed/model_characteristics.py
 Comment: 
 
+Filename: mlrl/testbed/models.py
+Comment: 
+
+Filename: mlrl/testbed/output_writer.py
+Comment: 
+
 Filename: mlrl/testbed/parameters.py
 Comment: 
 
 Filename: mlrl/testbed/persistence.py
 Comment: 
 
-Filename: mlrl/testbed/runnables.py
+Filename: mlrl/testbed/prediction_characteristics.py
 Comment: 
 
-Filename: mlrl/testbed/training.py
+Filename: mlrl/testbed/prediction_scope.py
+Comment: 
+
+Filename: mlrl/testbed/predictions.py
+Comment: 
+
+Filename: mlrl/testbed/probability_calibration.py
+Comment: 
+
+Filename: mlrl/testbed/runnables.py
 Comment: 
 
-Filename: mlrl_testbed-0.8.2.dist-info/METADATA
+Filename: mlrl_testbed-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: mlrl_testbed-0.8.2.dist-info/WHEEL
+Filename: mlrl_testbed-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: mlrl_testbed-0.8.2.dist-info/entry_points.txt
+Filename: mlrl_testbed-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlrl_testbed-0.8.2.dist-info/top_level.txt
+Filename: mlrl_testbed-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mlrl_testbed-0.8.2.dist-info/zip-safe
+Filename: mlrl_testbed-0.9.0.dist-info/zip-safe
 Comment: 
 
-Filename: mlrl_testbed-0.8.2.dist-info/RECORD
+Filename: mlrl_testbed-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlrl/testbed/data.py

```diff
@@ -1,37 +1,38 @@
-#!/usr/bin/python
-
 """
 Author: Michael Rapp (michael.rapp.ml@gmail.com)
 
 Provides functions for handling multi-label data.
 """
 import logging as log
 import os.path as path
 import xml.etree.ElementTree as XmlTree
+
 from enum import Enum, auto
-from typing import List, Optional
+from typing import List, Optional, Set, Tuple
 from xml.dom import minidom
 
 import arff
 import numpy as np
-from mlrl.common.data_types import DTYPE_UINT8, DTYPE_FLOAT32
-from mlrl.testbed.io import write_xml_file
-from scipy.sparse import coo_matrix, lil_matrix, csc_matrix, issparse, dok_matrix
+
+from scipy.sparse import coo_matrix, csc_matrix, dok_matrix, issparse, lil_matrix
 from sklearn.compose import ColumnTransformer
 from sklearn.preprocessing import OneHotEncoder
 
+from mlrl.common.data_types import DTYPE_FLOAT32, DTYPE_UINT8
+
+from mlrl.testbed.io import write_xml_file
+
 
 class AttributeType(Enum):
     """
     All supported types of attributes.
     """
-
-    NUMERIC = auto()
-
+    NUMERICAL = auto()
+    ORDINAL = auto()
     NOMINAL = auto()
 
 
 class Attribute:
     """
     Represents a numerical or nominal attribute that is contained by a data set.
     """
@@ -49,107 +50,127 @@
 
 class Label(Attribute):
     """
     Represents a label that is contained by a data set.
     """
 
     def __init__(self, name: str):
-        super().__init__(name, AttributeType.NOMINAL, [str(0), str(1)])
+        super(Label, self).__init__(name, AttributeType.NOMINAL, [str(0), str(1)])
 
 
 class MetaData:
     """
-    Stores the meta data of a multi-label data set.
+    Stores the meta-data of a multi-label data set.
     """
 
     def __init__(self, attributes: List[Attribute], labels: List[Attribute], labels_at_start: bool):
         """
         :param attributes:      A list that contains all attributes in the data set
         :param labels:          A list that contains all labels in the data set
         :param labels_at_start: True, if the labels are located at the start, False, if they are located at the end
         """
         self.attributes = attributes
         self.labels = labels
         self.labels_at_start = labels_at_start
 
-    def get_attribute_indices(self, attribute_type: AttributeType = None) -> List[int]:
+    def get_attribute_indices(self, attribute_types: Optional[Set[AttributeType]] = None) -> List[int]:
         """
-        Returns a list that contains the indices of all attributes of a specific type (in ascending order).
+        Returns a list that contains the indices of all attributes with one out of a set of given types (in ascending
+        order).
 
-        :param attribute_type:  The type of the attributes whose indices should be returned or None, if all indices
-                                should be returned
-        :return:                A list that contains the indices of all attributes of the given type
+        :param attribute_types: A set that contains the types of the attributes whose indices should be returned or
+                                None, if all indices should be returned
+        :return:                A list that contains the indices of all attributes of the given types
         """
-        return [i for i, attribute in enumerate(self.attributes) if
-                attribute_type is None or attribute.attribute_type == attribute_type]
+        return [
+            i for i, attribute in enumerate(self.attributes)
+            if attribute_types is None or attribute.attribute_type in attribute_types
+        ]
 
 
-def load_data_set_and_meta_data(data_dir: str, arff_file_name: str, xml_file_name: str,
+def load_data_set_and_meta_data(data_dir: str,
+                                arff_file_name: str,
+                                xml_file_name: str,
                                 feature_dtype=DTYPE_FLOAT32,
-                                label_dtype=DTYPE_UINT8) -> (lil_matrix, lil_matrix, MetaData):
+                                label_dtype=DTYPE_UINT8) -> Tuple[lil_matrix, lil_matrix, MetaData]:
     """
     Loads a multi-label data set from an ARFF file and the corresponding Mulan XML file.
 
     :param data_dir:        The path of the directory that contains the files
     :param arff_file_name:  The name of the ARFF file (including the suffix)
     :param xml_file_name:   The name of the XML file (including the suffix)
     :param feature_dtype:   The requested type of the feature matrix
     :param label_dtype:     The requested type of the label matrix
     :return:                A `scipy.sparse.lil_matrix` of type `feature_dtype`, shape `(num_examples, num_features)`,
                             representing the feature values of the examples, a `scipy.sparse.lil_matrix` of type
                             `label_dtype`, shape `(num_examples, num_labels)`, representing the corresponding label
-                            vectors, as well as the data set's meta data
+                            vectors, as well as the data set's meta-data
     """
     xml_file = path.join(data_dir, xml_file_name)
-    log.debug('Parsing meta data from file \"%s\"...', xml_file)
-    labels = __parse_labels(xml_file)
+    labels = None
+
+    if path.isfile(xml_file):
+        log.debug('Parsing meta data from file \"%s\"...', xml_file)
+        labels = __parse_labels_from_xml_file(xml_file)
+    else:
+        log.debug(
+            'Mulan XML file \"%s\" does not exist. If possible, information about the class labels is parsed from the '
+            + 'ARFF file\'s @relation declaration as intended by the MEKA data set format...', xml_file)
+
     arff_file = path.join(data_dir, arff_file_name)
     log.debug('Loading data set from file \"%s\"...', arff_file)
-    matrix, attributes = __load_arff(arff_file, feature_dtype=feature_dtype)
+    matrix, attributes, relation = __load_arff(arff_file, feature_dtype=feature_dtype)
+
+    if labels is None:
+        labels = __parse_labels_from_relation(relation, attributes)
+
     meta_data = __create_meta_data(attributes, labels)
     x, y = __create_feature_and_label_matrix(matrix, meta_data, label_dtype)
     return x, y, meta_data
 
 
-def load_data_set(data_dir: str, arff_file_name: str, meta_data: MetaData, feature_dtype=DTYPE_FLOAT32,
-                  label_dtype=DTYPE_UINT8) -> (lil_matrix, lil_matrix):
+def load_data_set(data_dir: str,
+                  arff_file_name: str,
+                  meta_data: MetaData,
+                  feature_dtype=DTYPE_FLOAT32,
+                  label_dtype=DTYPE_UINT8) -> Tuple[lil_matrix, lil_matrix]:
     """
-    Loads a multi-label data set from an ARFF file given its meta data.
+    Loads a multi-label data set from an ARFF file given its meta-data.
 
     :param data_dir:        The path of the directory that contains the ARFF file
     :param arff_file_name:  The name of the ARFF file (including the suffix)
-    :param meta_data:       The meta data
-    :param feature_dtype:   The requested dtype of the feature matrix
-    :param label_dtype:     The requested dtype of the label matrix
+    :param meta_data:       The meta-data
+    :param feature_dtype:   The requested data type of the feature matrix
+    :param label_dtype:     The requested data type of the label matrix
     :return:                A `scipy.sparse.lil_matrix` of type `feature_dtype`, shape `(num_examples, num_features)`,
                             representing the feature values of the examples, as well as a `scipy.sparse.lil_matrix` of
                             type `label_dtype`, shape `(num_examples, num_labels)`, representing the corresponding
                             label vectors
     """
     arff_file = path.join(data_dir, arff_file_name)
     log.debug('Loading data set from file \"%s\"...', arff_file)
-    matrix, _ = __load_arff(arff_file, feature_dtype=feature_dtype)
+    matrix, _, _ = __load_arff(arff_file, feature_dtype=feature_dtype)
     x, y = __create_feature_and_label_matrix(matrix, meta_data, label_dtype)
     return x, y
 
 
 def save_data_set_and_meta_data(output_dir: str, arff_file_name: str, xml_file_name: str, x: np.ndarray,
                                 y: np.ndarray) -> MetaData:
     """
-    Saves a multi-label data set to an ARFF file and its meta data to a XML file. All attributes in the data set are
+    Saves a multi-label data set to an ARFF file and its meta-data to an XML file. All attributes in the data set are
     considered to be numerical.
 
     :param output_dir:      The path of the directory where the ARFF file and the XML file should be saved
     :param arff_file_name:  The name of the ARFF file (including the suffix)
     :param xml_file_name:   The name of the XML file (including the suffix)
     :param x:               An array of type `float`, shape `(num_examples, num_features)`, representing the features of
                             the examples that are contained in the data set
     :param y:               An array of type `float`, shape `(num_examples, num_labels)`, representing the label vectors
                             of the examples that are contained in the data set
-    :return:                The meta data of the data set that has been saved
+    :return:                The meta-data of the data set that has been saved
     """
     meta_data = save_data_set(output_dir, arff_file_name, x, y)
     save_meta_data(output_dir, xml_file_name, meta_data)
     return meta_data
 
 
 def save_data_set(output_dir: str, arff_file_name: str, x: np.ndarray, y: np.ndarray) -> MetaData:
@@ -158,19 +179,19 @@
 
     :param output_dir:      The path of the directory where the ARFF file should be saved
     :param arff_file_name:  The name of the ARFF file (including the suffix)
     :param x:               A `np.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_features)`, that stores
                             the features of the examples that are contained in the data set
     :param y:               A `np.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_labels)`, that stores the
                             labels of the examples that are contained in the data set
-    :return:                The meta data of the data set that has been saved
+    :return:                The meta-data of the data set that has been saved
     """
 
     num_attributes = x.shape[1]
-    attributes = [Attribute('X' + str(i), AttributeType.NUMERIC) for i in range(num_attributes)]
+    attributes = [Attribute('X' + str(i), AttributeType.NUMERICAL) for i in range(num_attributes)]
     num_labels = y.shape[1]
     labels = [Label('y' + str(i)) for i in range(num_labels)]
     meta_data = MetaData(attributes, labels, labels_at_start=False)
     save_arff_file(output_dir, arff_file_name, x, y, meta_data)
     return meta_data
 
 
@@ -180,34 +201,34 @@
 
     :param output_dir:      The path of the directory where the ARFF file should be saved
     :param arff_file_name:  The name of the ARFF file (including the suffix)
     :param x:               A `np.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_features)`, that stores
                             the features of the examples that are contained in the data set
     :param y:               A `np.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_labels)`, that stores the
                             labels of the examples that are contained in the data set
-    :param meta_data:       The meta data of the data set that should be saved
+    :param meta_data:       The meta-data of the data set that should be saved
     """
     arff_file = path.join(output_dir, arff_file_name)
     log.debug('Saving data set to file \'' + str(arff_file) + '\'...')
     sparse = issparse(x) and issparse(y)
     x = dok_matrix(x)
     y = dok_matrix(y)
     x_prefix = 0
     y_prefix = 0
 
     attributes = meta_data.attributes
     x_attributes = [(u'{}'.format(attributes[i].attribute_name if len(attributes) > i else 'X' + str(i)),
-                     u'NUMERIC' if len(attributes) <= i or attributes[i].nominal_values is None or attributes[
-                         i].attribute_type == AttributeType.NUMERIC else attributes[i].nominal_values)
+                     u'NUMERIC' if len(attributes) <= i or attributes[i].nominal_values is None
+                     or attributes[i].attribute_type == AttributeType.NUMERICAL else attributes[i].nominal_values)
                     for i in range(x.shape[1])]
 
     labels = meta_data.labels
     y_attributes = [(u'{}'.format(labels[i].attribute_name if len(labels) > i else 'y' + str(i)),
-                     u'NUMERIC' if len(labels) <= i or labels[i].nominal_values is None or labels[
-                         i].attribute_type == AttributeType.NUMERIC else labels[i].nominal_values)
+                     u'NUMERIC' if len(labels) <= i or labels[i].nominal_values is None
+                     or labels[i].attribute_type == AttributeType.NUMERICAL else labels[i].nominal_values)
                     for i in range(y.shape[1])]
 
     if meta_data.labels_at_start:
         x_prefix = y.shape[1]
         relation_sign = 1
         attributes = y_attributes + x_attributes
     else:
@@ -223,90 +244,92 @@
     for keys, value in list(x.items()):
         data[keys[0]][x_prefix + keys[1]] = value
 
     for keys, value in list(y.items()):
         data[keys[0]][y_prefix + keys[1]] = value
 
     with open(arff_file, 'w') as file:
-        file.write(arff.dumps({
-            u'description': u'traindata',
-            u'relation': u'traindata: -C {}'.format(y.shape[1] * relation_sign),
-            u'attributes': attributes,
-            u'data': data
-        }))
+        file.write(
+            arff.dumps({
+                u'description': u'traindata',
+                u'relation': u'traindata: -C {}'.format(y.shape[1] * relation_sign),
+                u'attributes': attributes,
+                u'data': data
+            }))
     log.info('Successfully saved data set to file \'' + str(arff_file) + '\'.')
 
 
 def save_meta_data(output_dir: str, xml_file_name: str, meta_data: MetaData):
     """
-    Saves the meta data of a multi-label data set to a XML file.
+    Saves the meta-data of a multi-label data set to an XML file.
 
     :param output_dir:      The path of the directory where the XML file should be saved
     :param xml_file_name:   The name of the XML file (including the suffix)
-    :param meta_data:       The meta data of the data set
+    :param meta_data:       The meta-data of the data set
     """
     xml_file = path.join(output_dir, xml_file_name)
     log.debug('Saving meta data to file \'' + str(xml_file) + '\'...')
     __write_meta_data(xml_file, meta_data)
     log.info('Successfully saved meta data to file \'' + str(xml_file) + '\'.')
 
 
 def one_hot_encode(x, y, meta_data: MetaData, encoder=None):
     """
     One-hot encodes the nominal attributes contained in a data set, if any.
 
     If the given feature matrix is sparse, it will be converted into a dense matrix. Also, an updated variant of the
-    given meta data, where the attributes have been removed, will be returned, as the original attributes become invalid
+    given meta-data, where the attributes have been removed, will be returned, as the original attributes become invalid
     by applying one-hot-encoding.
 
     :param x:           A `np.ndarray` or `scipy.sparse.matrix`, shape `(num_examples, num_features)`, representing the
                         features of the examples in the data set
     :param y:           A `np.ndarray` or `scipy.sparse.matrix`, shape `(num_examples, num_labels)`, representing the
                         labels of the examples in the data set
-    :param meta_data:   The meta data of the data set
+    :param meta_data:   The meta-data of the data set
     :param encoder:     The 'ColumnTransformer' to be used or None, if a new encoder should be created
     :return:            A `np.ndarray`, shape `(num_examples, num_encoded_features)`, representing the encoded features
-                        of the given examples, the encoder that has been used, as well as the updated meta data
+                        of the given examples, the encoder that has been used, as well as the updated meta-data
     """
-    nominal_indices = meta_data.get_attribute_indices(AttributeType.NOMINAL)
+    nominal_indices = meta_data.get_attribute_indices({AttributeType.NOMINAL})
     num_nominal_attributes = len(nominal_indices)
     log.info('Data set contains %s nominal and %s numerical attributes.', num_nominal_attributes,
              (len(meta_data.attributes) - num_nominal_attributes))
 
     if num_nominal_attributes > 0:
         if issparse(x):
             x = x.toarray()
 
         old_shape = x.shape
 
         if encoder is None:
             log.info('Applying one-hot encoding...')
             encoder = ColumnTransformer(
-                [('one_hot_encoder', OneHotEncoder(handle_unknown='ignore', sparse=False), nominal_indices)],
+                [('one_hot_encoder', OneHotEncoder(handle_unknown='ignore', sparse_output=False), nominal_indices)],
                 remainder='passthrough')
             encoder.fit(x, y)
 
         x = encoder.transform(x)
         new_shape = x.shape
         updated_meta_data = MetaData([], meta_data.labels, meta_data.labels_at_start)
         log.info('Original data set contained %s attributes, one-hot encoded data set contains %s attributes',
                  old_shape[1], new_shape[1])
         return x, encoder, updated_meta_data
     else:
         log.debug('No need to apply one-hot encoding, as the data set does not contain any nominal attributes.')
         return x, None, meta_data
 
 
-def __create_feature_and_label_matrix(matrix: csc_matrix, meta_data: MetaData, label_dtype) -> (lil_matrix, lil_matrix):
+def __create_feature_and_label_matrix(matrix: csc_matrix, meta_data: MetaData,
+                                      label_dtype) -> Tuple[lil_matrix, lil_matrix]:
     """
     Creates and returns the feature and label matrix from a single matrix, representing the values in an ARFF file.
 
     :param matrix:      A `scipy.sparse.csc_matrix` of type `feature_dtype`, shape
                         `(num_examples, num_features + num_labels)`, representing the values in an ARFF file
-    :param meta_data:   The meta data of the data set
+    :param meta_data:   The meta-data of the data set
     :param label_dtype: The requested type of the label matrix
     :return:            A `scipy.sparse.lil_matrix` of type `feature_dtype`, shape `(num_examples, num_features)`,
                         representing the feature matrix, as well as `scipy.sparse.lil_matrix` of type `label_dtype`,
                         shape `(num_examples, num_labels)`, representing the label matrix
     """
     num_labels = len(meta_data.labels)
 
@@ -318,22 +341,23 @@
         y = matrix[:, -num_labels:]
 
     x = x.tolil()
     y = y.astype(label_dtype).tolil()
     return x, y
 
 
-def __load_arff(arff_file: str, feature_dtype) -> (csc_matrix, list):
+def __load_arff(arff_file: str, feature_dtype) -> Tuple[csc_matrix, list, str]:
     """
     Loads the content of an ARFF file.
 
     :param arff_file:       The path of the ARFF file (including the suffix)
     :param feature_dtype:   The type, the data should be converted to
-    :return:                A `np.sparse.csc_matrix` of type `feature_dtype`, containing the values in the ARFF file, as
-                            well as a list that contains a description of each attribute in the ARFF file
+    :return:                A `np.sparse.csc_matrix` of type `feature_dtype`, containing the values in the ARFF file, a
+                            list that contains a description of each attribute in the ARFF file, as well as its
+                            @relation name
     """
     try:
         arff_dict = __load_arff_as_dict(arff_file, sparse=True)
         data = arff_dict['data']
         matrix_data = data[0]
         matrix_row_indices = data[1]
         matrix_col_indices = data[2]
@@ -342,15 +366,16 @@
         matrix = matrix.tocsc()
     except arff.BadLayout:
         arff_dict = __load_arff_as_dict(arff_file, sparse=False)
         data = arff_dict['data']
         matrix = csc_matrix(data, dtype=feature_dtype)
 
     attributes = arff_dict['attributes']
-    return matrix, attributes
+    relation = arff_dict['relation']
+    return matrix, attributes, relation
 
 
 def __load_arff_as_dict(arff_file: str, sparse: bool) -> dict:
     """
     Loads the content of an ARFF file.
 
     :param arff_file:   The path of the ARFF file (including the suffix)
@@ -359,27 +384,46 @@
     :return:            A dictionary that stores the content of the ARFF file
     """
     with open(arff_file, 'r') as file:
         sparse_format = arff.COO if sparse else arff.DENSE
         return arff.load(file, encode_nominal=True, return_type=sparse_format)
 
 
-def __parse_labels(xml_file) -> List[Attribute]:
+def __parse_labels_from_xml_file(xml_file) -> List[Attribute]:
     """
     Parses a Mulan XML file to retrieve information about the labels contained in a data set.
 
     :param xml_file:    The path of the XML file (including the suffix)
     :return:            A list containing the labels
     """
 
     xml_doc = minidom.parse(xml_file)
     tags = xml_doc.getElementsByTagName('label')
     return [Label(__parse_attribute_or_label_name(tag.getAttribute('name'))) for tag in tags]
 
 
+def __parse_labels_from_relation(relation: str, attributes: list) -> List[Attribute]:
+    """
+    Parses the @relation declaration of an ARFF file to retrieve information about the labels contained in a data set.
+
+    :param relation:    The @relation declaration to be parsed
+    :return:            A list containing the labels
+    """
+    parameter_name = '-C '
+    index = relation.index(parameter_name)
+    parameter_value = relation[index + len(parameter_name):]
+    index = parameter_value.find(' ')
+
+    if index >= 0:
+        parameter_value = parameter_value[:index]
+
+    num_labels = int(parameter_value)
+    return [Label(__parse_attribute_or_label_name(attributes[i][0])) for i in range(num_labels)]
+
+
 def __create_meta_data(attributes: list, labels: List[Attribute]) -> MetaData:
     """
     Creates and returns the `MetaData` of a data set by parsing the attributes in an ARFF file to retrieve information
     about the attributes and labels contained in a data set.
 
     :param attributes:  A list that contains a description of each attribute in an ARFF file (including the labels)
     :param labels:      A list that contains the all labels
@@ -395,17 +439,24 @@
         if attribute_name not in label_names:
             type_definition = attribute[1]
 
             if isinstance(type_definition, list):
                 attribute_type = AttributeType.NOMINAL
                 nominal_values = type_definition
             else:
-                attribute_type = AttributeType.NUMERIC
+                type_definition = str(type_definition).lower()
                 nominal_values = None
 
+                if type_definition == 'integer':
+                    attribute_type = AttributeType.ORDINAL
+                elif type_definition == 'real' or type_definition == 'numeric':
+                    attribute_type = AttributeType.NUMERICAL
+                else:
+                    raise ValueError('Encountered unsupported attribute type: ' + type_definition)
+
             attribute_list.append(Attribute(attribute_name, attribute_type, nominal_values))
         elif len(attribute_list) == 0:
             labels_at_start = True
 
     meta_data = MetaData(attribute_list, labels, labels_at_start)
     return meta_data
 
@@ -423,18 +474,18 @@
     if name.endswith('\'') or name.endswith('\"'):
         name = name[:(len(name) - 1)]
     return name.replace('\\\'', '\'').replace('\\\"', '\"')
 
 
 def __write_meta_data(xml_file, meta_data: MetaData):
     """
-    Writes meta data to a Mulan XML file.
+    Writes meta-data to a Mulan XML file.
 
     :param xml_file:    The path fo the XML file (including the suffix)
-    :param meta_data:   The meta data to be written
+    :param meta_data:   The meta-data to be written
     """
     root_element = XmlTree.Element('labels')
     root_element.set('xmlns', 'http://mulan.sourceforge.net/labels')
 
     for label in meta_data.labels:
         label_element = XmlTree.SubElement(root_element, 'label')
         label_element.set('name', label.attribute_name)
```

## mlrl/testbed/data_characteristics.py

```diff
@@ -1,253 +1,157 @@
-#!/usr/bin/python
-
 """
 Author: Michael Rapp (michael.rapp.ml@gmail.com)
 
-Provides functions to determine certain characteristics of multi-label data sets.
+Provides classes for printing certain characteristics of multi-label data sets. The characteristics can be written to
+one or several outputs, e.g., to the console or to a file.
 """
-import logging as log
-from abc import ABC, abstractmethod
-from functools import reduce
-from typing import List
-
-import numpy as np
-from mlrl.testbed.data import MetaData, AttributeType
-from mlrl.testbed.io import clear_directory, open_writable_csv_file, create_csv_dict_writer
-from scipy.sparse import issparse
+from functools import cached_property, reduce
+from typing import Any, Dict, List, Optional
 
+from mlrl.common.options import Options
 
-def density(m) -> float:
-    """
-    Calculates and returns the density of a given feature or label matrix.
+from mlrl.testbed.characteristics import LABEL_CHARACTERISTICS, Characteristic, LabelCharacteristics, density
+from mlrl.testbed.data import AttributeType, MetaData
+from mlrl.testbed.data_splitting import DataSplit, DataType
+from mlrl.testbed.format import OPTION_DECIMALS, OPTION_PERCENTAGE, filter_formatters, format_table
+from mlrl.testbed.output_writer import Formattable, OutputWriter, Tabularizable
+from mlrl.testbed.prediction_scope import PredictionScope, PredictionType
 
-    :param m:   A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_rows, num_cols)`, that stores the feature values
-                of training examples or their labels
-    :return:    The fraction of non-zero elements in the given matrix among all elements
-    """
-    num_elements = m.shape[0] * m.shape[1]
+OPTION_EXAMPLES = 'examples'
 
-    if issparse(m):
-        num_non_zero = m.nnz
-    else:
-        num_non_zero = np.count_nonzero(m)
+OPTION_FEATURES = 'features'
 
-    return num_non_zero / num_elements if num_elements > 0 else 0
+OPTION_NUMERICAL_FEATURES = 'numerical_features'
 
+OPTION_NOMINAL_FEATURES = 'nominal_features'
 
-def label_cardinality(y) -> float:
-    """
-    Calculates and returns the average label cardinality of a given label matrix.
+OPTION_FEATURE_DENSITY = 'feature_density'
 
-    :param y:   A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_labels)`, that stores the labels
-                of training examples
-    :return:    The average number of relevant labels per training example
-    """
-    if issparse(y):
-        y = y.tolil()
-        num_relevant_per_example = y.getnnz(axis=1)
-    else:
-        num_relevant_per_example = np.count_nonzero(y, axis=1)
-
-    return np.average(num_relevant_per_example)
+OPTION_FEATURE_SPARSITY = 'feature_sparsity'
 
 
-def distinct_label_vectors(y) -> int:
+class FeatureCharacteristics:
     """
-    Determines and returns the number of distinct label vectors in a label matrix.
-
-    :param y:   A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_labels)`, that stores the labels
-                of training examples
-    :return:    The number of distinct label vectors in the given matrix
+    Stores characteristics of a feature matrix.
     """
-    if issparse(y):
-        y = y.tolil()
-        return np.unique(y.rows).shape[0]
-    else:
-        return np.unique(y, axis=0).shape[0]
 
+    def __init__(self, meta_data: MetaData, x):
+        """
+        :param meta_data:   The meta-data of the data set
+        :param x:           A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_features)`, that
+                            stores the feature values
+        """
+        self._x = x
+        self._meta_data = meta_data
+        self.num_examples = x.shape[0]
+        self.num_features = x.shape[1]
 
-def label_imbalance_ratio(y) -> float:
-    """
-    Calculates and returns the average label imbalance ratio of a given label matrix.
+    @cached_property
+    def num_nominal_features(self):
+        return reduce(lambda num, attribute: num + (1 if attribute.attribute_type == AttributeType.NOMINAL else 0),
+                      self._meta_data.attributes, 0)
 
-    :param y:   A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_labels)`, that stores the labels
-                of training examples
-    :return:    The label imbalance ratio averaged over the available labels
-    """
-    if issparse(y):
-        y = y.tocsc()
-        num_relevant_per_label = y.getnnz(axis=0)
-    else:
-        num_relevant_per_label = np.count_nonzero(y, axis=0)
+    @property
+    def num_numerical_features(self):
+        return self.num_features - self.num_nominal_features
 
-    max_relevant = np.max(num_relevant_per_label)
-    return np.average(max_relevant / num_relevant_per_label[num_relevant_per_label != 0])
+    @cached_property
+    def feature_density(self):
+        return density(self._x)
 
+    @property
+    def feature_sparsity(self):
+        return 1 - self.feature_density
 
-class DataCharacteristics:
-    """
-    Stores characteristics of a multi-label data set.
-    """
 
-    def __init__(self, num_examples: int, num_nominal_features: int, num_numerical_features: int,
-                 feature_density: float, num_labels: int, label_density: float, avg_label_imbalance_ratio: float,
-                 avg_label_cardinality: float, num_distinct_label_vectors: int):
-        """
-        :param num_examples:                The number of examples in the data set
-        :param num_nominal_features:        The number of nominal features in the data set
-        :param num_numerical_features:      The number of numerical features in the data set
-        :param feature_density:             The feature density
-        :param num_labels:                  The number of labels in the data set
-        :param label_density:               The label density
-        :param avg_label_imbalance_ratio:   The average label imbalance ratio
-        :param avg_label_cardinality:       The average label cardinality
-        :param num_distinct_label_vectors:  The number of distinct label vectors in the data set
-        """
-        self.num_examples = num_examples
-        self.num_nominal_features = num_nominal_features
-        self.num_numerical_features = num_numerical_features
-        self.feature_density = feature_density
-        self.num_labels = num_labels
-        self.label_density = label_density
-        self.avg_label_imbalance_ratio = avg_label_imbalance_ratio
-        self.avg_label_cardinality = avg_label_cardinality
-        self.num_distinct_label_vectors = num_distinct_label_vectors
+FEATURE_CHARACTERISTICS: List[Characteristic] = [
+    Characteristic(OPTION_EXAMPLES, 'Examples', lambda x: x.num_examples),
+    Characteristic(OPTION_FEATURES, 'Features', lambda x: x.num_features),
+    Characteristic(OPTION_NUMERICAL_FEATURES, 'Numerical Features', lambda x: x.num_nominal_features),
+    Characteristic(OPTION_NOMINAL_FEATURES, 'Nominal Features', lambda x: x.num_numerical_features),
+    Characteristic(OPTION_FEATURE_DENSITY, 'Feature Density', lambda x: x.feature_density, percentage=True),
+    Characteristic(OPTION_FEATURE_SPARSITY, 'Feature Sparsity', lambda x: x.feature_sparsity, percentage=True),
+]
 
 
-class DataCharacteristicsOutput(ABC):
+class DataCharacteristicsWriter(OutputWriter):
     """
-    An abstract base class for all outputs, the characteristics of a data set may be written to.
+    Allows to write the characteristics of a data set to one or severals sinks.
     """
 
-    @abstractmethod
-    def write_data_characteristics(self, experiment_name: str, characteristics: DataCharacteristics, total_folds: int,
-                                   fold: int = None):
+    class DataCharacteristics(Formattable, Tabularizable):
         """
-        Writes the characteristics of a data set to the output.
-
-        :param experiment_name: The name of the experiment
-        :param characteristics: The characteristics of the data set
-        :param total_folds:     The total number of folds
-        :param fold:            The fold for which the characteristics should be written or None, if no cross validation
-                                is used
+        Stores characteristics of a feature matrix and a label matrix.
         """
-        pass
 
+        def __init__(self, feature_characteristics: FeatureCharacteristics,
+                     label_characteristics: LabelCharacteristics):
+            """
+            :param feature_characteristics: The characteristics of the feature matrix
+            :param label_characteristics:   The characteristics of the label matrix
+            """
+            self.feature_characteristics = feature_characteristics
+            self.label_characteristics = label_characteristics
 
-class DataCharacteristicsLogOutput(DataCharacteristicsOutput):
-    """
-    Outputs the characteristics of a data set using the logger.
-    """
+        def format(self, options: Options, **kwargs) -> str:
+            percentage = options.get_bool(OPTION_PERCENTAGE, True)
+            decimals = options.get_int(OPTION_DECIMALS, 2)
+            rows = []
 
-    def write_data_characteristics(self, experiment_name: str, characteristics: DataCharacteristics, total_folds: int,
-                                   fold: int = None):
-        msg = 'Data characteristics for experiment \"' + experiment_name + '\"' + (
-            ' (Fold ' + str(fold + 1) + ')' if fold is not None else '') + ':\n\n'
-        msg += 'Examples: ' + str(characteristics.num_examples) + '\n'
-        msg += 'Features: ' + str(
-            characteristics.num_nominal_features + characteristics.num_numerical_features) + ' (' + str(
-            characteristics.num_numerical_features) + ' numerical, ' + str(
-            characteristics.num_nominal_features) + ' nominal)\n'
-        msg += 'Feature density: ' + str(characteristics.feature_density) + '\n'
-        msg += 'Feature sparsity: ' + str(1 - characteristics.feature_density) + '\n'
-        msg += 'Labels: ' + str(characteristics.num_labels) + '\n'
-        msg += 'Label density: ' + str(characteristics.label_density) + '\n'
-        msg += 'Label sparsity: ' + str(1 - characteristics.label_density) + '\n'
-        msg += 'Label imbalance ratio: ' + str(characteristics.avg_label_imbalance_ratio) + '\n'
-        msg += 'Label cardinality: ' + str(characteristics.avg_label_cardinality) + '\n'
-        msg += 'Distinct label vectors: ' + str(characteristics.num_distinct_label_vectors) + '\n'
-        log.info(msg)
+            for formatter in filter_formatters(FEATURE_CHARACTERISTICS, [options]):
+                rows.append([
+                    formatter.name,
+                    formatter.format(self.feature_characteristics, percentage=percentage, decimals=decimals)
+                ])
 
+            for formatter in filter_formatters(LABEL_CHARACTERISTICS, [options]):
+                rows.append([
+                    formatter.name,
+                    formatter.format(self.label_characteristics, percentage=percentage, decimals=decimals)
+                ])
 
-class DataCharacteristicsCsvOutput(DataCharacteristicsOutput):
-    """
-    Writes the characteristics of a data set to a CSV file.
-    """
+            return format_table(rows)
 
-    def __init__(self, output_dir: str, clear_dir: bool = True):
-        """
-        :param output_dir:  The path of the directory, the CSV files should be written to
-        :param clear_dir:   True, if the directory, the CSV files should be written to, should be cleared
-        """
-        self.output_dir = output_dir
-        self.clear_dir = clear_dir
+        def tabularize(self, options: Options, **kwargs) -> Optional[List[Dict[str, str]]]:
+            percentage = options.get_bool(OPTION_PERCENTAGE, True)
+            decimals = options.get_int(OPTION_DECIMALS, 0)
+            columns = {}
 
-    def write_data_characteristics(self, experiment_name: str, characteristics: DataCharacteristics, total_folds: int,
-                                   fold: int = None):
-        if fold is not None:
-            self.__clear_dir_if_necessary()
-            columns = {
-                'Examples': characteristics.num_examples,
-                'Features': characteristics.num_nominal_features + characteristics.num_numerical_features,
-                'Numerical features': characteristics.num_numerical_features,
-                'Nominal features': characteristics.num_nominal_features,
-                'Feature density': characteristics.feature_density,
-                'Feature sparsity': 1 - characteristics.feature_density,
-                'Labels': characteristics.num_labels,
-                'Label density': characteristics.label_density,
-                'Label sparsity': 1 - characteristics.label_density,
-                'Label imbalance ratio': characteristics.avg_label_imbalance_ratio,
-                'Label cardinality': characteristics.avg_label_cardinality,
-                'Distinct label vectors': characteristics.num_distinct_label_vectors
-            }
-            header = sorted(columns.keys())
-            header.insert(0, 'Approach')
-            columns['Approach'] = experiment_name
-            with open_writable_csv_file(self.output_dir, 'data_characteristics', fold) as csv_file:
-                csv_writer = create_csv_dict_writer(csv_file, header)
-                csv_writer.writerow(columns)
-
-    def __clear_dir_if_necessary(self):
-        """
-        Clears the output directory, if necessary.
-        """
-        if self.clear_dir:
-            clear_directory(self.output_dir)
-            self.clear_dir = False
+            for formatter in filter_formatters(FEATURE_CHARACTERISTICS, [options]):
+                columns[formatter] = formatter.format(self.feature_characteristics,
+                                                      percentage=percentage,
+                                                      decimals=decimals)
 
+            for formatter in filter_formatters(LABEL_CHARACTERISTICS, [options]):
+                columns[formatter] = formatter.format(self.label_characteristics,
+                                                      percentage=percentage,
+                                                      decimals=decimals)
 
-class DataCharacteristicsPrinter:
-    """
-    A class that allows to print the characteristics of data sets.
-    """
+            return [columns]
 
-    def __init__(self, outputs: List[DataCharacteristicsOutput]):
+    class LogSink(OutputWriter.LogSink):
         """
-        :param outputs: The outputs, the characteristics of data sets should be written to
+        Allows to write the characteristics of a data set to the console.
         """
-        self.outputs = outputs
 
-    def print(self, experiment_name: str, x, y, meta_data: MetaData, current_fold: int, num_folds: int):
+        def __init__(self, options: Options = Options()):
+            super().__init__(title='Data characteristics', options=options)
+
+    class CsvSink(OutputWriter.CsvSink):
+        """
+        Allows to write the characteristics of a data set to a CSV file.
         """
-        :param experiment_name: The name of the experiment
-        :param x:               A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_features)`, that
-                                stores the feature values
-        :param y:               A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_labels)`, that
-                                stores the ground truth labels
-        :param meta_data:       The meta data of the data set
-        :param current_fold:    The current fold
-        :param num_folds:       The total number of folds
-        """
-        if len(self.outputs) > 0:
-            num_examples = x.shape[0]
-            num_features = len(meta_data.attributes)
-            num_nominal_features = reduce(
-                lambda num, attribute: num + (1 if attribute.attribute_type == AttributeType.NOMINAL else 0),
-                meta_data.attributes, 0)
-            num_numerical_features = num_features - num_nominal_features
-            feature_density = density(x)
-            num_labels = len(meta_data.labels)
-            label_density = density(y)
-            avg_label_imbalance_ratio = label_imbalance_ratio(y)
-            avg_label_cardinality = label_cardinality(y)
-            num_distinct_label_vectors = distinct_label_vectors(y)
-            characteristics = DataCharacteristics(num_examples=num_examples, num_nominal_features=num_nominal_features,
-                                                  num_numerical_features=num_numerical_features,
-                                                  feature_density=feature_density, num_labels=num_labels,
-                                                  label_density=label_density,
-                                                  avg_label_imbalance_ratio=avg_label_imbalance_ratio,
-                                                  avg_label_cardinality=avg_label_cardinality,
-                                                  num_distinct_label_vectors=num_distinct_label_vectors)
-            for output in self.outputs:
-                output.write_data_characteristics(experiment_name, characteristics, num_folds,
-                                                  current_fold if num_folds > 1 else None)
+
+        def __init__(self, output_dir: str, options: Options = Options()):
+            super().__init__(output_dir=output_dir, file_name='data_characteristics', options=options)
+
+    def __init__(self, sinks: List[OutputWriter.Sink]):
+        super().__init__(sinks)
+
+    def _generate_output_data(self, meta_data: MetaData, x, y, data_split: DataSplit, learner,
+                              data_type: Optional[DataType], prediction_type: Optional[PredictionType],
+                              prediction_scope: Optional[PredictionScope], predictions: Optional[Any],
+                              train_time: float, predict_time: float) -> Optional[Any]:
+        feature_characteristics = FeatureCharacteristics(meta_data, x)
+        label_characteristics = LabelCharacteristics(y)
+        return DataCharacteristicsWriter.DataCharacteristics(feature_characteristics=feature_characteristics,
+                                                             label_characteristics=label_characteristics)
```

## mlrl/testbed/evaluation.py

```diff
@@ -1,451 +1,459 @@
-#!/usr/bin/python
-
 """
 Author: Michael Rapp (michael.rapp.ml@gmail.com)
 
 Provides classes for evaluating the predictions or rankings provided by a multi-label learner according to different
-measures. The evaluation results can be written to one or several outputs, e.g. to the console or to a file.
+measures. The evaluation results can be written to one or several outputs, e.g., to the console or to a file.
 """
-import logging as log
-from abc import ABC, abstractmethod
-from typing import List, Dict, Set, Optional
+from abc import ABC
+from typing import Any, Dict, List, Optional, Set, Tuple
 
 import numpy as np
 import sklearn.metrics as metrics
-from mlrl.common.arrays import enforce_dense
-from mlrl.common.data_types import DTYPE_UINT8
-from mlrl.testbed.data import MetaData, save_arff_file, Label
-from mlrl.testbed.io import open_writable_csv_file, create_csv_dict_writer, clear_directory, SUFFIX_ARFF, \
-    get_file_name_per_fold
-from sklearn.utils.multiclass import is_multilabel
-
-# The name of the accuracy metric
-ACCURACY = 'Acc.'
-
-# The name of the 0/1 loss metric.
-ZERO_ONE_LOSS = '0/1 Loss'
-
-# The name of the precision metric
-PRECISION = 'Prec.'
-
-# The name of the recall metric
-RECALL = 'Rec.'
 
-# The name of the F1 metric
-F1 = 'F1'
-
-# The name of the hamming loss metric
-HAMMING_LOSS = 'Hamm. Loss'
-
-# The name of the hamming accuracy metric
-HAMMING_ACCURACY = 'Hamm. Acc.'
+from sklearn.utils.multiclass import is_multilabel
 
-# The name of the subset 0/1 loss metric
-SUBSET_ZERO_ONE_LOSS = 'Subs. 0/1 Loss'
+from mlrl.common.arrays import enforce_dense
+from mlrl.common.data_types import DTYPE_UINT8
+from mlrl.common.options import Options
 
-# The name of the subset accuracy metric
-SUBSET_ACCURACY = 'Subs. Acc.'
+from mlrl.testbed.data import MetaData
+from mlrl.testbed.data_splitting import CrossValidationOverall, DataSplit, DataType
+from mlrl.testbed.format import OPTION_DECIMALS, OPTION_PERCENTAGE, Formatter, filter_formatters, format_table
+from mlrl.testbed.output_writer import Formattable, OutputWriter, Tabularizable
+from mlrl.testbed.prediction_scope import PredictionScope, PredictionType
 
-# The name of the micro-averaged precision metric
-MICRO_PRECISION = 'Mi. Prec.'
+OPTION_ENABLE_ALL = 'enable_all'
 
-# The name of the macro-averaged precision metric
-MACRO_PRECISION = 'Ma. Prec.'
+OPTION_HAMMING_LOSS = 'hamming_loss'
 
-# The name of the micro-averaged recall metric
-MICRO_RECALL = 'Mi. Rec.'
+OPTION_HAMMING_ACCURACY = 'hamming_accuracy'
 
-# The name of the macro-averaged recall metric
-MACRO_RECALL = 'Ma. Rec.'
+OPTION_SUBSET_ZERO_ONE_LOSS = 'subset_zero_one_loss'
 
-# The name of the micro-averaged F1 metric
-MICRO_F1 = 'Mi. F1'
+OPTION_SUBSET_ACCURACY = 'subset_accuracy'
 
-# The name of the macro-averaged F1 metric
-MACRO_F1 = 'Ma. F1'
+OPTION_MICRO_PRECISION = 'micro_precision'
 
-# The name of the example-based precision metric
-EX_BASED_PRECISION = 'Ex.-based Prec.'
+OPTION_MICRO_RECALL = 'micro_recall'
 
-# The name of the example-based recall metric
-EX_BASED_RECALL = 'Ex.-based Rec.'
+OPTION_MICRO_F1 = 'micro_f1'
 
-# The name of the example-based F1 metric
-EX_BASED_F1 = 'Ex.-based F1'
+OPTION_MICRO_JACCARD = 'micro_jaccard'
 
-# The name of the rank loss metric
-RANK_LOSS = 'Rank Loss'
+OPTION_MACRO_PRECISION = 'macro_precision'
 
-# The time needed to train the model
-TIME_TRAIN = 'Training Time'
+OPTION_MACRO_RECALL = 'macro_recall'
 
-# The time needed to make predictions
-TIME_PREDICT = 'Prediction Time'
+OPTION_MACRO_F1 = 'macro_f1'
 
+OPTION_MACRO_JACCARD = 'macro_jaccard'
 
-class Evaluation(ABC):
-    """
-    An abstract base class for all classes that evaluate the predictions provided by a classifier or ranker.
-    """
+OPTION_EXAMPLE_WISE_PRECISION = 'example_wise_precision'
 
-    @abstractmethod
-    def evaluate(self, experiment_name: str, meta_data: MetaData, predictions, ground_truth, first_fold: int,
-                 current_fold: int, last_fold: int, num_folds: int, train_time: float, predict_time: float):
-        """
-        Evaluates the predictions provided by a classifier or ranker.
+OPTION_EXAMPLE_WISE_RECALL = 'example_wise_recall'
 
-        :param experiment_name: The name of the experiment
-        :param meta_data:       The meta data of the data set
-        :param predictions:     The predictions provided by the classifier
-        :param ground_truth:    The true labels
-        :param first_fold:      The first cross validation fold or 0, if no cross validation is used
-        :param current_fold:    The current cross validation fold starting at 0, or 0 if no cross validation is used
-        :param last_fold:       The last cross validation fold or 0, if no cross validation is used
-        :param num_folds:       The total number of cross validation folds or 1, if no cross validation is used
-        :param train_time:      The time needed to train the model
-        :param predict_time:    The time needed to make predictions
-        """
-        pass
+OPTION_EXAMPLE_WISE_F1 = 'example_wise_f1'
 
+OPTION_EXAMPLE_WISE_JACCARD = 'example_wise_jaccard'
 
-class EvaluationResult:
-    """
-    Stores the evaluation results according to different measures.
-    """
+OPTION_ACCURACY = 'accuracy'
 
-    def __init__(self):
-        self.measures: Set[str] = set()
-        self.results: Optional[List[Dict[str, float]]] = None
+OPTION_ZERO_ONE_LOSS = 'zero_one_loss'
 
-    def put(self, name: str, score: float, fold: int, num_folds: int):
-        """
-        Adds a new score according to a specific measure to the evaluation result.
+OPTION_PRECISION = 'precision'
 
-        :param name:        The name of the measure
-        :param score:       The score according to the measure
-        :param fold:        The fold the score corresponds to
-        :param num_folds:   The total number of cross validation folds
-        """
+OPTION_RECALL = 'recall'
 
-        if self.results is None:
-            self.results = [{} for _ in range(num_folds)]
-        elif len(self.results) != num_folds:
-            raise AssertionError('Inconsistent number of total folds given')
-
-        self.measures.add(name)
-        values = self.results[fold]
-        values[name] = score
+OPTION_F1 = 'f1'
 
-    def get(self, name: str, fold: int) -> float:
-        """
-        Returns the score according to a specific measure and fold.
+OPTION_JACCARD = 'jaccard'
 
-        :param name:    The name of the measure
-        :param fold:    The fold the score corresponds to
-        :return:        The score
-        """
+OPTION_MEAN_ABSOLUTE_ERROR = 'mean_absolute_error'
 
-        values = self.results[fold] if self.results is not None else None
+OPTION_MEAN_SQUARED_ERROR = 'mean_squared_error'
 
-        if values is None:
-            raise AssertionError('No evaluation results available')
+OPTION_MEDIAN_ABSOLUTE_ERROR = 'mean_absolute_error'
 
-        return values[name]
+OPTION_MEAN_ABSOLUTE_PERCENTAGE_ERROR = 'mean_absolute_percentage_error'
 
-    def dict(self, fold: int) -> Dict:
-        values = self.results[fold].copy() if self.results is not None else None
+OPTION_RANK_LOSS = 'rank_loss'
 
-        if values is None:
-            raise AssertionError('No evaluation results available')
+OPTION_COVERAGE_ERROR = 'coverage_error'
 
-        return values
+OPTION_LABEL_RANKING_AVERAGE_PRECISION = 'lrap'
 
-    def avg(self, name: str) -> (float, float):
-        """
-        Returns the score and standard deviation according to a specific measure averaged over all available folds.
+OPTION_DISCOUNTED_CUMULATIVE_GAIN = 'dcg'
 
-        :param name:    The name of the measure
-        :return:        A tuple consisting of the averaged score and standard deviation
-        """
-        values = []
+OPTION_NORMALIZED_DISCOUNTED_CUMULATIVE_GAIN = 'ndcg'
 
-        for i in range(len(self.results)):
-            if len(self.results[i]) > 0:
-                values.append(self.get(name, i))
-
-        values = np.array(values)
-        return np.average(values), np.std(values)
-
-    def avg_dict(self) -> Dict:
-        result: Dict[str, float] = {}
-
-        for measure in self.measures:
-            score, std_dev = self.avg(measure)
-            result[measure] = score
-            result['Std.-dev. ' + measure] = std_dev.item()
+OPTION_TRAINING_TIME = 'training_time'
 
-        return result
+OPTION_PREDICTION_TIME = 'prediction_time'
 
 
-class EvaluationOutput(ABC):
+class EvaluationFunction(Formatter):
     """
-    An abstract base class for all outputs, evaluation results may be written to.
+    An evaluation function.
     """
 
-    def __init__(self, output_predictions: bool, output_individual_folds: bool):
-        """
-        :param output_predictions:      True, if predictions provided by a classifier or ranker should be written to the
-                                        output, False otherwise
-        :param output_individual_folds: True, if the evaluation results for individual cross validation folds should be
-                                        written to the outputs, False, if only the overall evaluation results, i.e.,
-                                        averaged over all folds, should be written to the outputs
-        """
-        self.output_predictions = output_predictions
-        self.output_individual_folds = output_individual_folds
-
-    @abstractmethod
-    def write_evaluation_results(self, experiment_name: str, evaluation_result: EvaluationResult, total_folds: int,
-                                 fold: int = None):
+    def __init__(self, option: str, name: str, evaluation_function, percentage: bool = True, **kwargs):
         """
-        Writes an evaluation result to the output.
-
-        :param experiment_name:     The name of the experiment
-        :param evaluation_result:   The evaluation result to be written
-        :param total_folds:         The total number of folds
-        :param fold:                The fold for which the results should be written or None, if no cross validation is
-                                    used or if the overall results, averaged over all folds, should be written
+        :param evaluation_function: The function that should be invoked for evaluation
         """
-        pass
+        super().__init__(option, name, percentage)
+        self.evaluation_function = evaluation_function
+        self.kwargs = kwargs
 
-    @abstractmethod
-    def write_predictions(self, experiment_name: str, meta_data: MetaData, predictions, ground_truth, total_folds: int,
-                          fold: int = None):
+    def evaluate(self, ground_truth, predictions) -> float:
         """
-        Writes predictions to the output.
+        Applies the evaluation function to given predictions and ground truth labels.
 
-        :param experiment_name: The name of the experiment
-        :param meta_data:       The meta data of the data set
-        :param predictions:     The predictions
         :param ground_truth:    The ground truth
-        :param total_folds:     The total number of folds
-        :param fold:            The fold for which the predictions should be written or None, if no cross validation is
-                                used
+        :param predictions:     The predictions
+        :return:                An evaluation score
         """
-        pass
+        return self.evaluation_function(ground_truth, predictions, **self.kwargs)
 
 
-class EvaluationLogOutput(EvaluationOutput):
-    """
-    Outputs evaluation result using the logger.
-    """
+ARGS_SINGLE_LABEL = {'zero_division': 1}
 
-    def __init__(self, output_predictions: bool = False, output_individual_folds: bool = True):
-        super().__init__(output_predictions, output_individual_folds)
-
-    def write_evaluation_results(self, experiment_name: str, evaluation_result: EvaluationResult, total_folds: int,
-                                 fold: int = None):
-        if fold is None or self.output_individual_folds:
-            text = ''
-
-            for measure in sorted(evaluation_result.measures):
-                if measure != TIME_TRAIN and measure != TIME_PREDICT:
-                    if len(text) > 0:
-                        text += '\n'
+ARGS_MICRO = {'average': 'micro', 'zero_division': 1}
 
+ARGS_MACRO = {'average': 'macro', 'zero_division': 1}
+
+ARGS_EXAMPLE_WISE = {'average': 'samples', 'zero_division': 1}
+
+EVALUATION_MEASURE_TRAINING_TIME = Formatter(OPTION_TRAINING_TIME, 'Training Time')
+
+EVALUATION_MEASURE_PREDICTION_TIME = Formatter(OPTION_PREDICTION_TIME, 'Prediction Time')
+
+MULTI_LABEL_EVALUATION_MEASURES: List[Formatter] = [
+    EvaluationFunction(OPTION_HAMMING_ACCURACY, 'Hamming Accuracy', lambda a, b: 1 - metrics.hamming_loss(a, b)),
+    EvaluationFunction(OPTION_HAMMING_LOSS, 'Hamming Loss', metrics.hamming_loss),
+    EvaluationFunction(OPTION_SUBSET_ACCURACY, 'Subset Accuracy', metrics.accuracy_score),
+    EvaluationFunction(OPTION_SUBSET_ZERO_ONE_LOSS, 'Subset 0/1 Loss', lambda a, b: 1 - metrics.accuracy_score(a, b)),
+    EvaluationFunction(OPTION_MICRO_PRECISION, 'Micro Precision', metrics.precision_score, **ARGS_MICRO),
+    EvaluationFunction(OPTION_MICRO_RECALL, 'Micro Recall', metrics.recall_score, **ARGS_MICRO),
+    EvaluationFunction(OPTION_MICRO_F1, 'Micro F1', metrics.f1_score, **ARGS_MICRO),
+    EvaluationFunction(OPTION_MICRO_JACCARD, 'Micro Jaccard', metrics.jaccard_score, **ARGS_MICRO),
+    EvaluationFunction(OPTION_MACRO_PRECISION, 'Macro Precision', metrics.precision_score, **ARGS_MACRO),
+    EvaluationFunction(OPTION_MACRO_RECALL, 'Macro Recall', metrics.recall_score, **ARGS_MACRO),
+    EvaluationFunction(OPTION_MACRO_F1, 'Macro F1', metrics.f1_score, **ARGS_MACRO),
+    EvaluationFunction(OPTION_MACRO_JACCARD, 'Macro Jaccard', metrics.jaccard_score, **ARGS_MACRO),
+    EvaluationFunction(OPTION_EXAMPLE_WISE_PRECISION, 'Example-wise Precision', metrics.precision_score,
+                       **ARGS_EXAMPLE_WISE),
+    EvaluationFunction(OPTION_EXAMPLE_WISE_RECALL, 'Example-wise Recall', metrics.recall_score, **ARGS_EXAMPLE_WISE),
+    EvaluationFunction(OPTION_EXAMPLE_WISE_F1, 'Example-wise F1', metrics.f1_score, **ARGS_EXAMPLE_WISE),
+    EvaluationFunction(OPTION_EXAMPLE_WISE_JACCARD, 'Example-wise Jaccard', metrics.jaccard_score, **ARGS_EXAMPLE_WISE),
+    EVALUATION_MEASURE_TRAINING_TIME,
+    EVALUATION_MEASURE_PREDICTION_TIME,
+]
+
+SINGLE_LABEL_EVALUATION_MEASURES: List[Formatter] = [
+    EvaluationFunction(OPTION_ACCURACY, 'Accuracy', metrics.accuracy_score),
+    EvaluationFunction(OPTION_ZERO_ONE_LOSS, '0/1 Loss', lambda a, b: 1 - metrics.accuracy_score(a, b)),
+    EvaluationFunction(OPTION_PRECISION, 'Precision', metrics.precision_score, **ARGS_SINGLE_LABEL),
+    EvaluationFunction(OPTION_RECALL, 'Recall', metrics.recall_score, **ARGS_SINGLE_LABEL),
+    EvaluationFunction(OPTION_F1, 'F1', metrics.f1_score, **ARGS_SINGLE_LABEL),
+    EvaluationFunction(OPTION_JACCARD, 'Jaccard', metrics.jaccard_score, **ARGS_SINGLE_LABEL),
+    EVALUATION_MEASURE_TRAINING_TIME,
+    EVALUATION_MEASURE_PREDICTION_TIME,
+]
+
+REGRESSION_EVALUATION_MEASURES: List[Formatter] = [
+    EvaluationFunction(OPTION_MEAN_ABSOLUTE_ERROR, 'Mean Absolute Error', metrics.mean_absolute_error,
+                       percentage=False),
+    EvaluationFunction(OPTION_MEAN_SQUARED_ERROR, 'Mean Squared Error', metrics.mean_squared_error, percentage=False),
+    EvaluationFunction(OPTION_MEDIAN_ABSOLUTE_ERROR,
+                       'Median Absolute Error',
+                       metrics.median_absolute_error,
+                       percentage=False),
+    EvaluationFunction(OPTION_MEAN_ABSOLUTE_PERCENTAGE_ERROR,
+                       'Mean Absolute Percentage Error',
+                       metrics.mean_absolute_percentage_error,
+                       percentage=False),
+    EVALUATION_MEASURE_TRAINING_TIME,
+    EVALUATION_MEASURE_PREDICTION_TIME,
+]
+
+RANKING_EVALUATION_MEASURES: List[Formatter] = [
+    EvaluationFunction(OPTION_RANK_LOSS, 'Ranking Loss', metrics.label_ranking_loss, percentage=False),
+    EvaluationFunction(OPTION_COVERAGE_ERROR, 'Coverage Error', metrics.coverage_error, percentage=False),
+    EvaluationFunction(OPTION_LABEL_RANKING_AVERAGE_PRECISION,
+                       'Label Ranking Average Precision',
+                       metrics.label_ranking_average_precision_score,
+                       percentage=False),
+    EvaluationFunction(OPTION_DISCOUNTED_CUMULATIVE_GAIN,
+                       'Discounted Cumulative Gain',
+                       metrics.dcg_score,
+                       percentage=False),
+    EvaluationFunction(OPTION_NORMALIZED_DISCOUNTED_CUMULATIVE_GAIN, 'NDCG', metrics.ndcg_score),
+    EVALUATION_MEASURE_TRAINING_TIME,
+    EVALUATION_MEASURE_PREDICTION_TIME,
+]
+
+
+class EvaluationWriter(OutputWriter, ABC):
+    """
+    An abstract base class for all classes that evaluate the predictions provided by a learner and allow to write the
+    evaluation results to one or several sinks.
+    """
+
+    KWARG_FOLD = 'fold'
+
+    class EvaluationResult(Formattable, Tabularizable):
+        """
+        Stores the evaluation results according to different measures.
+        """
+
+        def __init__(self):
+            self.measures: Set[Formatter] = set()
+            self.results: Optional[List[Dict[Formatter, float]]] = None
+
+        def put(self, measure: Formatter, score: float, num_folds: int, fold: Optional[int]):
+            """
+            Adds a new score according to a specific measure to the evaluation result.
+
+            :param measure:     The measure
+            :param score:       The score according to the measure
+            :param num_folds:   The total number of cross validation folds
+            :param fold:        The fold, the score corresponds to, or None, if no cross validation is used
+            """
+            if self.results is None:
+                self.results = [{} for _ in range(num_folds)]
+            elif len(self.results) != num_folds:
+                raise AssertionError('Inconsistent number of total folds given')
+
+            self.measures.add(measure)
+            values = self.results[fold if fold is not None else 0]
+            values[measure] = score
+
+        def get(self, measure: Formatter, fold: Optional[int], **kwargs) -> str:
+            """
+            Returns the score according to a specific measure.
+
+            :param measure: The measure
+            :param fold:    The fold, the score corresponds to, or None, if no cross validation is used
+            :return:        A textual representation of the score
+            """
+            if self.results is None:
+                raise AssertionError('No evaluation results available')
+
+            score = self.results[fold if fold is not None else 0][measure]
+            return measure.format(score, **kwargs)
+
+        def dict(self, fold: Optional[int], **kwargs) -> Dict[Formatter, str]:
+            """
+            Returns a dictionary that stores the scores for a specific fold according to each measure.
+
+            :param fold:    The fold, the scores correspond to, or None, if no cross validation is used
+            :return:        A dictionary that stores textual representations of the scores for the given fold according
+                            to each measure
+            """
+            if self.results is None:
+                raise AssertionError('No evaluation results available')
+
+            results: Dict[Formatter, str] = {}
+
+            for measure, score in self.results[fold if fold is not None else 0].items():
+                results[measure] = measure.format(score, **kwargs)
+
+            return results
+
+        def avg(self, measure: Formatter, **kwargs) -> Tuple[str, str]:
+            """
+            Returns the score and standard deviation according to a specific measure averaged over all available folds.
+
+            :param measure: The measure
+            :return:        A tuple consisting of textual representations of the averaged score and standard deviation
+            """
+            values = []
+
+            for i in range(len(self.results)):
+                results = self.results[i]
+
+                if len(results) > 0:
+                    values.append(results[measure])
+
+            values = np.array(values)
+            return measure.format(np.average(values), **kwargs), measure.format(np.std(values), **kwargs)
+
+        def avg_dict(self, **kwargs) -> Dict[Formatter, str]:
+            """
+            Returns a dictionary that stores the scores, averaged across all folds, as well as the standard deviation,
+            according to each measure.
+
+            :return: A dictionary that stores textual representations of the scores and standard deviation according to
+                     each measure
+            """
+            result: Dict[Formatter, str] = {}
+
+            for measure in self.measures:
+                score, std_dev = self.avg(measure, **kwargs)
+                result[measure] = score
+                result[Formatter(measure.option, 'Std.-dev. ' + measure.name, measure.percentage)] = std_dev
+
+            return result
+
+        def format(self, options: Options, **kwargs) -> str:
+            fold = kwargs.get(EvaluationWriter.KWARG_FOLD)
+            percentage = options.get_bool(OPTION_PERCENTAGE, True)
+            decimals = options.get_int(OPTION_DECIMALS, 2)
+            enable_all = options.get_bool(OPTION_ENABLE_ALL, True)
+            rows = []
+
+            for measure in sorted(self.measures):
+                if options.get_bool(measure.option, enable_all) and measure != EVALUATION_MEASURE_TRAINING_TIME \
+                    and measure != EVALUATION_MEASURE_PREDICTION_TIME:
                     if fold is None:
-                        score, std_dev = evaluation_result.avg(measure)
-                        text += (measure + ': ' + str(score))
-
-                        if total_folds > 1:
-                            text += (' ±' + str(std_dev))
+                        score, std_dev = self.avg(measure, percentage=percentage, decimals=decimals)
+                        rows.append([str(measure), score, '±' + std_dev])
                     else:
-                        score = evaluation_result.get(measure, fold)
-                        text += (measure + ': ' + str(score))
+                        score = self.get(measure, fold, percentage=percentage, decimals=decimals)
+                        rows.append([str(measure), score])
 
-            msg = ('Overall evaluation result for experiment \"' + experiment_name + '\"' if fold is None else
-                   'Evaluation result for experiment \"' + experiment_name + '\" (Fold ' + str(
-                       fold + 1) + ')') + ':\n\n%s\n'
-            log.info(msg, text)
-
-    def write_predictions(self, experiment_name: str, meta_data: MetaData, predictions, ground_truth, total_folds: int,
-                          fold: int = None):
-        if self.output_predictions:
-            text = 'Ground truth:\n\n' + np.array2string(ground_truth) + '\n\nPredictions:\n\n' + np.array2string(
-                predictions)
-            msg = ('Predictions for experiment \"' + experiment_name + '\"' if fold is None else
-                   'Predictions for experiment \"' + experiment_name + '\" (Fold ' + str(fold + 1) + ')') + ':\n\n%s\n'
-            log.info(msg, text)
+            return format_table(rows)
 
+        def tabularize(self, options: Options, **kwargs) -> Optional[List[Dict[str, str]]]:
+            fold = kwargs.get(EvaluationWriter.KWARG_FOLD)
+            percentage = options.get_bool(OPTION_PERCENTAGE, True)
+            decimals = options.get_int(OPTION_DECIMALS, 0)
+            enable_all = options.get_bool(OPTION_ENABLE_ALL, True)
 
-class EvaluationCsvOutput(EvaluationOutput):
-    """
-    Writes evaluation results to CSV files.
-    """
-
-    def __init__(self, output_dir: str, clear_dir: bool = True, output_predictions: bool = False,
-                 output_individual_folds: bool = True):
-        """
-        :param output_dir:  The path of the directory, the CSV files should be written to
-        :param clear_dir:   True, if the directory, the CSV files should be written to, should be cleared
-        """
-        super().__init__(output_predictions, output_individual_folds)
-        self.output_dir = output_dir
-        self.clear_dir = clear_dir
-
-    def write_evaluation_results(self, experiment_name: str, evaluation_result: EvaluationResult, total_folds: int,
-                                 fold: int = None):
-        if fold is None or self.output_individual_folds:
-            self.__clear_dir_if_necessary()
-            columns = evaluation_result.avg_dict() if fold is None else evaluation_result.dict(fold)
-            header = sorted(columns.keys())
-            header.insert(0, 'Approach')
-            columns['Approach'] = experiment_name
-
-            with open_writable_csv_file(self.output_dir, 'evaluation', fold, append=True) as csv_file:
-                csv_writer = create_csv_dict_writer(csv_file, header)
-                csv_writer.writerow(columns)
-
-    def write_predictions(self, experiment_name: str, meta_data: MetaData, predictions, ground_truth, total_folds: int,
-                          fold: int = None):
-        if self.output_predictions:
-            self.__clear_dir_if_necessary()
-            file_name = get_file_name_per_fold('predictions_' + experiment_name, SUFFIX_ARFF, fold)
-            attributes = [Label('Ground Truth ' + label.attribute_name) for label in meta_data.labels]
-            labels = [Label('Prediction ' + label.attribute_name) for label in meta_data.labels]
-            prediction_meta_data = MetaData(attributes, labels, labels_at_start=False)
-            save_arff_file(self.output_dir, file_name, ground_truth, predictions, prediction_meta_data)
+            if fold is None:
+                columns = self.avg_dict(percentage=percentage, decimals=decimals)
+            else:
+                columns = self.dict(fold, percentage=percentage, decimals=decimals)
 
-    def __clear_dir_if_necessary(self):
-        """
-        Clears the output directory, if necessary.
-        """
-        if self.clear_dir:
-            clear_directory(self.output_dir)
-            self.clear_dir = False
+            filtered_columns = {}
 
+            for measure, value in columns.items():
+                if options.get_bool(measure.option, enable_all):
+                    filtered_columns[measure.name] = value
 
-class AbstractEvaluation(Evaluation):
-    """
-    An abstract base class for all classes that evaluate the predictions provided by a classifier or ranker and allow to
-    write the results to one or several outputs.
-    """
+            return [filtered_columns]
 
-    def __init__(self, *args: EvaluationOutput):
+    class LogSink(OutputWriter.LogSink):
         """
-        :param args: The outputs, the evaluation results should be written to
+        Allows to write evaluation results to the console.
         """
-        self.outputs = args
-        self.results: Dict[str, EvaluationResult] = {}
 
-    def evaluate(self, experiment_name: str, meta_data: MetaData, predictions, ground_truth, first_fold: int,
-                 current_fold: int, last_fold: int, num_folds: int, train_time: float, predict_time: float):
-        result = self.results[experiment_name] if experiment_name in self.results else EvaluationResult()
-        self.results[experiment_name] = result
-        result.put(TIME_TRAIN, train_time, current_fold, num_folds)
-        result.put(TIME_PREDICT, predict_time, current_fold, num_folds)
-        self._populate_result(result, predictions, ground_truth, current_fold=current_fold, num_folds=num_folds)
-        self.__write_predictions(experiment_name, meta_data, predictions, ground_truth, current_fold=current_fold,
-                                 num_folds=num_folds)
-        self.__write_evaluation_result(experiment_name, result, first_fold=first_fold, current_fold=current_fold,
-                                       last_fold=last_fold, num_folds=num_folds)
-
-    @abstractmethod
-    def _populate_result(self, result: EvaluationResult, predictions, ground_truth, current_fold: int, num_folds: int):
-        pass
+        def __init__(self, options: Options = Options()):
+            super().__init__(title='Evaluation result', options=options)
 
-    def __write_predictions(self, experiment_name: str, meta_data: MetaData, predictions, ground_truth,
-                            current_fold: int, num_folds: int):
-        """
-        Writes predictions to the outputs.
+        def write_output(self, meta_data: MetaData, data_split: DataSplit, data_type: Optional[DataType],
+                         prediction_scope: Optional[PredictionScope], output_data, **kwargs):
+            fold = data_split.get_fold() if data_split.is_cross_validation_used() else 0
+            new_kwargs = {**kwargs, **{EvaluationWriter.KWARG_FOLD: fold}}
+            super().write_output(meta_data, data_split, data_type, prediction_scope, output_data, **new_kwargs)
 
-        :param experiment_name: The name of the experiment
-        :param meta_data:       The meta data of the data set
-        :param predictions:     The predictions
-        :param ground_truth:    The ground truth
-        :param current_fold:    The current cross validation fold or 0, if no cross validation is used
-        :param num_folds:       The total number of cross validation folds or 1, if no cross validation is used
+            if data_split.is_cross_validation_used() and data_split.is_last_fold():
+                super().write_output(meta_data, CrossValidationOverall(data_split.get_num_folds()), data_type,
+                                     prediction_scope, output_data, **kwargs)
+
+    class CsvSink(OutputWriter.CsvSink):
+        """
+        Allows to write evaluation results to CSV files.
         """
 
-        for output in self.outputs:
-            output.write_predictions(experiment_name, meta_data, predictions, ground_truth, num_folds,
-                                     current_fold if num_folds > 1 else None)
+        def __init__(self, output_dir: str, options: Options = Options()):
+            super().__init__(output_dir=output_dir, file_name='evaluation', options=options)
 
-    def __write_evaluation_result(self, experiment_name: str, result: EvaluationResult, first_fold: int,
-                                  current_fold: int, last_fold: int, num_folds: int):
-        """
-        Writes an evaluation result to the outputs.
+        def write_output(self, meta_data: MetaData, data_split: DataSplit, data_type: Optional[DataType],
+                         prediction_scope: Optional[PredictionScope], output_data, **kwargs):
+            fold = data_split.get_fold() if data_split.is_cross_validation_used() else 0
+            new_kwargs = {**kwargs, **{EvaluationWriter.KWARG_FOLD: fold}}
+            super().write_output(meta_data, data_split, data_type, prediction_scope, output_data, **new_kwargs)
 
-        :param experiment_name: The name of the experiment
-        :param result:          The evaluation result
-        :param first_fold:      The first cross validation fold or 0, if no cross validation is used
-        :param current_fold:    The current cross validation fold or 0, if no cross validation is used
-        :param last_fold        The last cross validation fold or 0, if no cross validation is used
-        :param num_folds:       The total number of cross validation folds or 1, if no cross validation is used
-        """
+            if data_split.is_cross_validation_used() and data_split.is_last_fold():
+                super().write_output(meta_data, CrossValidationOverall(data_split.get_num_folds()), data_type,
+                                     prediction_scope, output_data, **kwargs)
 
-        if num_folds > 1:
-            for output in self.outputs:
-                output.write_evaluation_results(experiment_name, result, num_folds, current_fold)
+    def __init__(self, sinks: List[OutputWriter.Sink]):
+        super().__init__(sinks)
+        self.results: Dict[str, EvaluationWriter.EvaluationResult] = {}
 
-        if num_folds == 1 or (current_fold == last_fold and abs(last_fold - first_fold) > 0):
-            for output in self.outputs:
-                output.write_evaluation_results(experiment_name, result, num_folds)
+    def _generate_output_data(self, meta_data: MetaData, x, y, data_split: DataSplit, learner,
+                              data_type: Optional[DataType], prediction_type: Optional[PredictionType],
+                              prediction_scope: Optional[PredictionScope], predictions: Optional[Any],
+                              train_time: float, predict_time: float) -> Optional[Any]:
+        result = self.results[data_type] if data_type in self.results else EvaluationWriter.EvaluationResult()
+        self.results[data_type] = result
+        num_folds = data_split.get_num_folds()
+        fold = data_split.get_fold()
+        result.put(EVALUATION_MEASURE_TRAINING_TIME, train_time, num_folds=num_folds, fold=fold)
+        result.put(EVALUATION_MEASURE_PREDICTION_TIME, predict_time, num_folds=num_folds, fold=fold)
+        self._populate_result(data_split, result, predictions, y)
+        return result
 
 
-class ClassificationEvaluation(AbstractEvaluation):
+class BinaryEvaluationWriter(EvaluationWriter):
     """
-    Evaluates the predictions of a single- or multi-label classifier according to commonly used bipartition measures.
+    Evaluates the quality of binary predictions provided by a single- or multi-label classifier according to commonly
+    used bipartition measures.
     """
 
-    def __init__(self, *args: EvaluationOutput):
-        super().__init__(*args)
+    def __init__(self, sinks: List[OutputWriter.Sink]):
+        super().__init__(sinks)
+        options = [sink.options for sink in sinks]
+        self.multi_Label_evaluation_functions = filter_formatters(MULTI_LABEL_EVALUATION_MEASURES, options)
+        self.single_Label_evaluation_functions = filter_formatters(SINGLE_LABEL_EVALUATION_MEASURES, options)
+
+    def _populate_result(self, data_split: DataSplit, result: EvaluationWriter.EvaluationResult, predictions,
+                         ground_truth):
+        num_folds = data_split.get_num_folds()
+        fold = data_split.get_fold()
 
-    def _populate_result(self, result: EvaluationResult, predictions, ground_truth, current_fold: int, num_folds: int):
         if is_multilabel(ground_truth):
-            hamming_loss = metrics.hamming_loss(ground_truth, predictions)
-            result.put(HAMMING_LOSS, hamming_loss, current_fold, num_folds)
-            result.put(HAMMING_ACCURACY, 1 - hamming_loss, current_fold, num_folds)
-            subset_accuracy = metrics.accuracy_score(ground_truth, predictions)
-            result.put(SUBSET_ACCURACY, subset_accuracy, current_fold, num_folds)
-            result.put(SUBSET_ZERO_ONE_LOSS, 1 - subset_accuracy, current_fold, num_folds)
-            result.put(MICRO_PRECISION, metrics.precision_score(ground_truth, predictions, average='micro',
-                                                                zero_division=1), current_fold, num_folds)
-            result.put(MICRO_RECALL, metrics.recall_score(ground_truth, predictions, average='micro', zero_division=1),
-                       current_fold, num_folds)
-            result.put(MICRO_F1, metrics.f1_score(ground_truth, predictions, average='micro', zero_division=1),
-                       current_fold, num_folds)
-            result.put(MACRO_PRECISION, metrics.precision_score(ground_truth, predictions, average='macro',
-                                                                zero_division=1), current_fold, num_folds)
-            result.put(MACRO_RECALL, metrics.recall_score(ground_truth, predictions, average='macro', zero_division=1),
-                       current_fold, num_folds)
-            result.put(MACRO_F1, metrics.f1_score(ground_truth, predictions, average='macro', zero_division=1),
-                       current_fold, num_folds)
-            result.put(EX_BASED_PRECISION, metrics.precision_score(ground_truth, predictions, average='samples',
-                                                                   zero_division=1), current_fold, num_folds)
-            result.put(EX_BASED_RECALL, metrics.recall_score(ground_truth, predictions, average='samples',
-                                                             zero_division=1), current_fold, num_folds)
-            result.put(EX_BASED_F1, metrics.f1_score(ground_truth, predictions, average='samples', zero_division=1),
-                       current_fold, num_folds)
+            evaluation_functions = self.multi_Label_evaluation_functions
         else:
             predictions = np.ravel(enforce_dense(predictions, order='C', dtype=DTYPE_UINT8))
             ground_truth = np.ravel(enforce_dense(ground_truth, order='C', dtype=DTYPE_UINT8))
-            accuracy = metrics.accuracy_score(ground_truth, predictions)
-            result.put(ACCURACY, accuracy, current_fold, num_folds)
-            result.put(ZERO_ONE_LOSS, 1 - accuracy, current_fold, num_folds)
-            result.put(PRECISION, metrics.precision_score(ground_truth, predictions, zero_division=1), current_fold,
-                       num_folds)
-            result.put(RECALL, metrics.recall_score(ground_truth, predictions, zero_division=1), current_fold,
-                       num_folds)
-            result.put(F1, metrics.f1_score(ground_truth, predictions, zero_division=1), current_fold, num_folds)
+            evaluation_functions = self.single_Label_evaluation_functions
+
+        for evaluation_function in evaluation_functions:
+            if isinstance(evaluation_function, EvaluationFunction):
+                score = evaluation_function.evaluate(ground_truth, predictions)
+                result.put(evaluation_function, score, num_folds=num_folds, fold=fold)
 
 
-class RankingEvaluation(AbstractEvaluation):
+class ScoreEvaluationWriter(EvaluationWriter):
     """
-    Evaluates the predictions of a multi-label ranker according to commonly used ranking measures.
+    Evaluates the quality of regression scores provided by a single- or multi-output regressor according to commonly
+    used regression and ranking measures.
     """
 
-    def __init__(self, *args: EvaluationOutput):
-        super().__init__(*args)
+    def __init__(self, sinks: List[OutputWriter.Sink]):
+        super().__init__(sinks)
+        options = [sink.options for sink in sinks]
+        self.regression_evaluation_functions = filter_formatters(REGRESSION_EVALUATION_MEASURES, options)
+        self.ranking_evaluation_functions = filter_formatters(RANKING_EVALUATION_MEASURES, options)
+
+    def _populate_result(self, data_split: DataSplit, result: EvaluationWriter.EvaluationResult, predictions,
+                         ground_truth):
+        num_folds = data_split.get_num_folds()
+        fold = data_split.get_fold()
+        ground_truth = enforce_dense(ground_truth, order='C', dtype=DTYPE_UINT8)
+
+        if is_multilabel(ground_truth):
+            evaluation_functions = self.ranking_evaluation_functions + self.regression_evaluation_functions
+        else:
+            evaluation_functions = self.regression_evaluation_functions
+
+            if predictions.shape[1] > 1:
+                predictions = predictions[:, -1]
+
+        for evaluation_function in evaluation_functions:
+            if isinstance(evaluation_function, EvaluationFunction):
+                score = evaluation_function.evaluate(ground_truth, predictions)
+                result.put(evaluation_function, score, num_folds=num_folds, fold=fold)
+
+
+class ProbabilityEvaluationWriter(ScoreEvaluationWriter):
+    """
+    Evaluates the quality of probability estimates provided by a single- or multi-label classifier according to commonly
+    used regression and ranking measures.
+    """
 
-    def _populate_result(self, result: EvaluationResult, predictions, ground_truth, current_fold: int, num_folds: int):
-        result.put(RANK_LOSS, metrics.label_ranking_loss(ground_truth, predictions), current_fold, num_folds)
+    def __init__(self, sinks: List[OutputWriter.Sink]):
+        super().__init__(sinks)
```

## mlrl/testbed/experiments.py

```diff
@@ -1,172 +1,409 @@
-#!/usr/bin/python
-
-
 """
 Author: Michael Rapp (michael.rapp.ml@gmail.com)
 
 Provides classes for performing experiments.
 """
 import logging as log
-from abc import ABC
+
+from abc import ABC, abstractmethod
+from functools import reduce
 from timeit import default_timer as timer
+from typing import List, Optional
+
+from sklearn.base import BaseEstimator, RegressorMixin, clone
 
-from mlrl.common.learners import Learner, NominalAttributeLearner
-from mlrl.testbed.data import MetaData, AttributeType
-from mlrl.testbed.data_characteristics import DataCharacteristicsPrinter
-from mlrl.testbed.evaluation import Evaluation
-from mlrl.testbed.model_characteristics import ModelPrinter, ModelCharacteristicsPrinter
+from mlrl.common.learners import IncrementalLearner, Learner, NominalAttributeLearner, OrdinalAttributeLearner
+
+from mlrl.testbed.data import AttributeType, MetaData
+from mlrl.testbed.data_splitting import DataSplit, DataSplitter, DataType
+from mlrl.testbed.format import format_duration
+from mlrl.testbed.output_writer import OutputWriter
 from mlrl.testbed.parameters import ParameterInput
 from mlrl.testbed.persistence import ModelPersistence
-from mlrl.testbed.training import CrossValidation, DataSet
-from sklearn.base import clone
+from mlrl.testbed.prediction_scope import GlobalPrediction, IncrementalPrediction, PredictionScope, PredictionType
+
+
+class Evaluation(ABC):
+    """
+    An abstract base class for all classes that allow to evaluate predictions that are obtained from a previously
+    trained model.
+    """
 
+    def __init__(self, prediction_type: PredictionType, output_writers: List[OutputWriter]):
+        """
+        :param prediction_type: The type of the predictions to be obtained
+        :param output_writers:  A list that contains all output writers to be invoked after predictions have been
+                                obtained
+        """
+        self.prediction_type = prediction_type
+        self.output_writers = output_writers
 
-class Experiment(CrossValidation, ABC):
+    def _invoke_prediction_function(self, learner, predict_function, predict_proba_function, x):
+        """
+        May be used by subclasses in order to invoke the correct prediction function, depending on the type of
+        result that should be obtained.
+
+        :param learner:                 The learner, the result should be obtained from
+        :param predict_function:        The function to be invoked if binary result or regression scores should be
+                                        obtained
+        :param predict_proba_function:  The function to be invoked if probability estimates should be obtained
+        :param x:                       A `numpy.ndarray` or `scipy.sparse` matrix, shape
+                                        `(num_examples, num_features)`, that stores the feature values of the query
+                                        examples
+        :return:                        The return value of the invoked function
+        """
+        prediction_type = self.prediction_type
+
+        if prediction_type == PredictionType.SCORES:
+            try:
+                if isinstance(learner, Learner):
+                    result = predict_function(x, predict_scores=True)
+                elif isinstance(learner, RegressorMixin):
+                    result = predict_function(x)
+                else:
+                    raise RuntimeError()
+            except RuntimeError:
+                log.error('Prediction of regression scores not supported')
+                result = None
+        elif prediction_type == PredictionType.PROBABILITIES:
+            try:
+                result = predict_proba_function(x)
+            except RuntimeError:
+                log.error('Prediction of probabilities not supported')
+                result = None
+        else:
+            result = predict_function(x)
+
+        return result
+
+    def _evaluate_predictions(self, meta_data: MetaData, data_split: DataSplit, data_type: DataType,
+                              prediction_scope: PredictionScope, train_time: float, predict_time: float, x, y,
+                              predictions, learner):
+        """
+        May be used by subclasses in order to evaluate predictions that have been obtained from a previously trained
+        model.
+
+        :param meta_data:           The meta-data of the data set
+        :param data_split:          The split of the available data, the predictions and ground truth labels correspond
+                                    to
+        :param data_type:           Specifies whether the predictions and ground truth labels correspond to the training
+                                    or test data
+        :param prediction_scope:    Specifies whether the predictions have been obtained from a global model or
+                                    incrementally
+        :param train_time:          The time needed to train the model
+        :param predict_time:        The time needed to obtain the predictions
+        :param x:                   A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_features)`,
+                                    that stores the feature values of the query examples
+        :param y:                   A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_labels)`, that
+                                    stores the ground truth labels of the query examples
+        :param predictions:         A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_labels)`, that
+                                    stores the predictions for the query examples
+        :param learner:             The learner, the predictions have been obtained from
+        """
+        for output_writer in self.output_writers:
+            output_writer.write_output(meta_data, x, y, data_split, learner, data_type, self.prediction_type,
+                                       prediction_scope, predictions, train_time, predict_time)
+
+    @abstractmethod
+    def predict_and_evaluate(self, meta_data: MetaData, data_split: DataSplit, data_type: DataType, train_time: float,
+                             learner, x, y):
+        """
+        Must be implemented by subclasses in order to obtain and evaluate predictions for given query examples from a
+        previously trained model.
+
+        :param meta_data:   The meta-data of the data set
+        :param data_split:  The split of the available data, the predictions and ground truth labels correspond to
+        :param data_type:   Specifies whether the predictions and ground truth labels correspond to the training or test
+                            data
+        :param train_time:  The time needed to train the model
+        :param learner:     The learner, the predictions should be obtained from
+        :param x:           A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_features)`, that
+                            stores the feature values of the query examples
+        :param y:           A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_labels)`, that stores
+                            the ground truth labels of the query examples
+        """
+        pass
+
+
+class GlobalEvaluation(Evaluation):
+    """
+    Obtains and evaluates predictions from a previously trained global model.
+    """
+
+    def __init__(self, prediction_type: PredictionType, output_writers: List[OutputWriter]):
+        super().__init__(prediction_type, output_writers)
+
+    def predict_and_evaluate(self, meta_data: MetaData, data_split: DataSplit, data_type: DataType, train_time: float,
+                             learner, x, y):
+        log.info('Predicting for %s ' + data_type.value + ' examples...', x.shape[0])
+        start_time = timer()
+        predictions = self._invoke_prediction_function(learner, learner.predict, learner.predict_proba, x)
+        end_time = timer()
+        predict_time = end_time - start_time
+
+        if predictions is not None:
+            log.info('Successfully predicted in %s', format_duration(predict_time))
+            self._evaluate_predictions(meta_data=meta_data,
+                                       data_split=data_split,
+                                       data_type=data_type,
+                                       prediction_scope=GlobalPrediction(),
+                                       train_time=train_time,
+                                       predict_time=predict_time,
+                                       x=x,
+                                       y=y,
+                                       predictions=predictions,
+                                       learner=learner)
+
+
+class IncrementalEvaluation(Evaluation):
+    """
+    Repeatedly obtains and evaluates predictions from a previously trained ensemble model, e.g., a model consisting of
+    several rules, using only a subset of the ensemble members with increasing size.
+    """
+
+    def __init__(self, prediction_type: PredictionType, output_writers: List[OutputWriter], min_size: int,
+                 max_size: int, step_size: int):
+        """
+        :param min_size:    The minimum number of ensemble members to be evaluated. Must be at least 0
+        :param max_size:    The maximum number of ensemble members to be evaluated. Must be greater than `min_size` or
+                            0, if all ensemble members should be evaluated
+        :param step_size:   The number of additional ensemble members to be considered at each repetition. Must be at
+                            least 1
+        """
+        super().__init__(prediction_type, output_writers)
+        self.min_size = min_size
+        self.max_size = max_size
+        self.step_size = step_size
+
+    def predict_and_evaluate(self, meta_data: MetaData, data_split: DataSplit, data_type: DataType, train_time: float,
+                             learner, x, y):
+        if not isinstance(learner, IncrementalLearner):
+            raise ValueError('Cannot obtain incremental predictions from a model of type ' + type(learner.__name__))
+
+        incremental_predictor = self._invoke_prediction_function(learner, learner.predict_incrementally,
+                                                                 learner.predict_proba_incrementally, x)
+
+        if incremental_predictor is not None:
+            step_size = self.step_size
+            total_size = incremental_predictor.get_num_next()
+            max_size = self.max_size
+
+            if max_size > 0:
+                total_size = min(max_size, total_size)
+
+            min_size = self.min_size
+            next_step_size = min_size if min_size > 0 else step_size
+            current_size = min(next_step_size, total_size)
+
+            while incremental_predictor.has_next():
+                log.info('Predicting for %s ' + data_type.value + ' examples using a model of size %s...', x.shape[0],
+                         current_size)
+                start_time = timer()
+                predictions = incremental_predictor.apply_next(next_step_size)
+                end_time = timer()
+                predict_time = end_time - start_time
+
+                if predictions is not None:
+                    log.info('Successfully predicted in %s', format_duration(predict_time))
+                    self._evaluate_predictions(meta_data=meta_data,
+                                               data_split=data_split,
+                                               data_type=data_type,
+                                               prediction_scope=IncrementalPrediction(current_size),
+                                               train_time=train_time,
+                                               predict_time=predict_time,
+                                               x=x,
+                                               y=y,
+                                               predictions=predictions,
+                                               learner=learner)
+
+                next_step_size = step_size
+                current_size = min(current_size + next_step_size, total_size)
+
+
+class Experiment(DataSplitter.Callback):
     """
     An experiment that trains and evaluates a single multi-label classifier or ranker on a specific data set using cross
     validation or separate training and test sets.
     """
 
-    def __init__(self, base_learner: Learner, data_set: DataSet, num_folds: int = 1, current_fold: int = -1,
-                 train_evaluation: Evaluation = None, test_evaluation: Evaluation = None,
-                 parameter_input: ParameterInput = None, model_printer: ModelPrinter = None,
-                 model_characteristics_printer: ModelCharacteristicsPrinter = None,
-                 data_characteristics_printer: DataCharacteristicsPrinter = None, persistence: ModelPersistence = None):
+    class ExecutionHook(ABC):
+        """
+        An abstract base class for all operations that may be executed before or after an experiment.
+        """
+
+        @abstractmethod
+        def execute(self):
+            """
+            Must be overridden by subclasses in order to execute the operation.
+            """
+            pass
+
+    def __init__(self,
+                 base_learner: BaseEstimator,
+                 learner_name: str,
+                 data_splitter: DataSplitter,
+                 pre_training_output_writers: List[OutputWriter],
+                 post_training_output_writers: List[OutputWriter],
+                 pre_execution_hook: Optional[ExecutionHook] = None,
+                 train_evaluation: Optional[Evaluation] = None,
+                 test_evaluation: Optional[Evaluation] = None,
+                 parameter_input: Optional[ParameterInput] = None,
+                 persistence: Optional[ModelPersistence] = None):
         """
         :param base_learner:                    The classifier or ranker to be trained
-        :param train_evaluation:                The evaluation to be used for evaluating the predictions for the
-                                                training data or None, if the predictions should not be evaluated
-        :param test_evaluation:                 The evaluation to be used for evaluating the predictions for the test
+        :param learner_name:                    The name of the classifier or ranker
+        :param data_splitter:                   The method to be used for splitting the available data into training and
+                                                test sets
+        :param pre_training_output_writers:     A list that contains all output writers to be invoked before training
+        :param post_training_output_writers:    A list that contains all output writers to be invoked after training
+        :param pre_execution_hook:              An operation that should be executed before the experiment
+        :param train_evaluation:                The method to be used for evaluating the predictions for the training
                                                 data or None, if the predictions should not be evaluated
+        :param test_evaluation:                 The method to be used for evaluating the predictions for the test data
+                                                or None, if the predictions should not be evaluated
         :param parameter_input:                 The input that should be used to read the parameter settings
-        :param model_printer:                   The printer that should be used to print textual representations of
-                                                models or None, if no textual representations should be printed
-        :param model_characteristics_printer:   The printer that should be used to print the characteristics of models
-                                                or None, if the characteristics should not be printed
-        :param data_characteristics_printer:    The printer that should be used to print the characteristics of the
-                                                training data or None, if the characteristics should not be printed
         :param persistence:                     The `ModelPersistence` that should be used for loading and saving models
         """
-        super().__init__(data_set, num_folds, current_fold)
         self.base_learner = base_learner
+        self.learner_name = learner_name
+        self.data_splitter = data_splitter
+        self.pre_training_output_writers = pre_training_output_writers
+        self.post_training_output_writers = post_training_output_writers
+        self.pre_execution_hook = pre_execution_hook
         self.train_evaluation = train_evaluation
         self.test_evaluation = test_evaluation
         self.parameter_input = parameter_input
-        self.model_printer = model_printer
-        self.model_characteristics_printer = model_characteristics_printer
-        self.data_characteristics_printer = data_characteristics_printer
         self.persistence = persistence
 
     def run(self):
-        log.info('Starting experiment \"' + self.base_learner.get_name() + '\"...')
-        super().run()
+        log.info('Starting experiment...')
+
+        # Run pre-execution hook, if necessary...
+        if self.pre_execution_hook is not None:
+            self.pre_execution_hook.execute()
 
-    def _train_and_evaluate(self, meta_data: MetaData, train_indices, train_x, train_y, test_indices, test_x, test_y,
-                            first_fold: int, current_fold: int, last_fold: int, num_folds: int):
+        self.data_splitter.run(self)
+
+    def train_and_evaluate(self, meta_data: MetaData, data_split: DataSplit, train_x, train_y, test_x, test_y):
         base_learner = self.base_learner
         current_learner = clone(base_learner)
 
         # Apply parameter setting, if necessary...
         parameter_input = self.parameter_input
 
         if parameter_input is not None:
-            params = parameter_input.read_parameters(current_fold)
+            params = parameter_input.read_parameters(data_split)
             current_learner.set_params(**params)
             log.info('Successfully applied parameter setting: %s', params)
 
-        learner_name = current_learner.get_name()
-
-        # Print data characteristics, if necessary...
-        data_characteristics_printer = self.data_characteristics_printer
-
-        if data_characteristics_printer is not None:
-            data_characteristics_printer.print(learner_name, train_x, train_y, meta_data, current_fold=current_fold,
-                                               num_folds=num_folds)
+        # Write output data before model is trained...
+        for output_writer in self.pre_training_output_writers:
+            output_writer.write_output(meta_data, train_x, train_y, data_split, current_learner)
+
+        # Set the indices of ordinal attributes, if supported...
+        if isinstance(current_learner, OrdinalAttributeLearner):
+            current_learner.ordinal_attribute_indices = meta_data.get_attribute_indices({AttributeType.ORDINAL})
 
         # Set the indices of nominal attributes, if supported...
         if isinstance(current_learner, NominalAttributeLearner):
-            current_learner.nominal_attribute_indices = meta_data.get_attribute_indices(AttributeType.NOMINAL)
+            current_learner.nominal_attribute_indices = meta_data.get_attribute_indices({AttributeType.NOMINAL})
 
         # Load model from disc, if possible, otherwise train a new model...
-        loaded_learner = self.__load_model(model_name=learner_name, current_fold=current_fold, num_folds=num_folds)
+        loaded_learner = self.__load_model(data_split)
 
-        if isinstance(loaded_learner, Learner):
+        if isinstance(loaded_learner, type(current_learner)):
+            current_params = current_learner.get_params()
+            self.__check_for_parameter_changes(expected_params=current_params,
+                                               actual_params=loaded_learner.get_params())
+            loaded_learner.set_params(**current_params)
             current_learner = loaded_learner
+            train_time = 0
         else:
             log.info('Fitting model to %s training examples...', train_x.shape[0])
-            current_learner.fit(train_x, train_y)
-            log.info('Successfully fit model in %s seconds', current_learner.train_time_)
+            train_time = self.__train(current_learner, train_x, train_y)
+            log.info('Successfully fit model in %s', format_duration(train_time))
 
             # Save model to disk...
-            self.__save_model(current_learner, current_fold=current_fold, num_folds=num_folds)
+            self.__save_model(current_learner, data_split)
 
         # Obtain and evaluate predictions for training data, if necessary...
         evaluation = self.train_evaluation
 
-        if evaluation is not None:
-            log.info('Predicting for %s training examples...', train_x.shape[0])
-            start_time = timer()
-            predictions = current_learner.predict(train_x)
-            end_time = timer()
-            predict_time = end_time - start_time
-            log.info('Successfully predicted in %s seconds', predict_time)
-            evaluation.evaluate('train_' + learner_name, meta_data, predictions, train_y, first_fold=first_fold,
-                                current_fold=current_fold, last_fold=last_fold, num_folds=num_folds,
-                                train_time=current_learner.train_time_, predict_time=predict_time)
+        if evaluation is not None and data_split.is_train_test_separated():
+            data_type = DataType.TRAINING
+            evaluation.predict_and_evaluate(meta_data, data_split, data_type, train_time, current_learner, train_x,
+                                            train_y)
 
         # Obtain and evaluate predictions for test data, if necessary...
         evaluation = self.test_evaluation
 
         if evaluation is not None:
-            log.info('Predicting for %s test examples...', test_x.shape[0])
-            start_time = timer()
-            predictions = current_learner.predict(test_x)
-            end_time = timer()
-            predict_time = end_time - start_time
-            log.info('Successfully predicted in %s seconds', predict_time)
-            evaluation.evaluate('test_' + learner_name, meta_data, predictions, test_y, first_fold=first_fold,
-                                current_fold=current_fold, last_fold=last_fold, num_folds=num_folds,
-                                train_time=current_learner.train_time_, predict_time=predict_time)
-
-        # Print model characteristics, if necessary...
-        model_characteristics_printer = self.model_characteristics_printer
-
-        if model_characteristics_printer is not None:
-            model_characteristics_printer.print(learner_name, current_learner, current_fold=current_fold,
-                                                num_folds=num_folds)
-
-        # Print model, if necessary...
-        model_printer = self.model_printer
-
-        if model_printer is not None:
-            model_printer.print(learner_name, meta_data, current_learner, current_fold=current_fold,
-                                num_folds=num_folds)
+            data_type = DataType.TEST if data_split.is_train_test_separated() else DataType.TRAINING
+            evaluation.predict_and_evaluate(meta_data, data_split, data_type, train_time, current_learner, test_x,
+                                            test_y)
+
+        # Write output data after model was trained...
+        for output_writer in self.post_training_output_writers:
+            output_writer.write_output(meta_data, train_x, train_y, data_split, current_learner, train_time=train_time)
+
+    @staticmethod
+    def __train(learner, x, y):
+        """
+        Fits a learner to training data.
 
-    def __load_model(self, model_name: str, current_fold: int, num_folds: int):
+        :param learner: The learner
+        :param x:       A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_features)`, that stores
+                        the feature values of the training examples
+        :param y:       A `numpy.ndarray` or `scipy.sparse` matrix, shape `(num_examples, num_labels)`, that stores the
+                        labels of the training examples according to the ground truth
+        :return:        The time needed for training
+        """
+        start_time = timer()
+        learner.fit(x, y)
+        end_time = timer()
+        return end_time - start_time
+
+    def __load_model(self, data_split: DataSplit):
         """
         Loads the model from disk, if available.
 
-        :param model_name:      The name of the model to be loaded
-        :param current_fold:    The current fold starting at 0, or 0 if no cross validation is used
-        :param num_folds:       The total number of cross validation folds or 1, if no cross validation is used
-        :return: The loaded model
+        :param data_split:  Information about the split of the available data, the model corresponds to
+        :return:            The loaded model
         """
         persistence = self.persistence
 
         if persistence is not None:
-            return persistence.load_model(model_name=model_name, fold=(current_fold if num_folds > 1 else None))
+            return persistence.load_model(self.learner_name, data_split)
 
         return None
 
-    def __save_model(self, model: Learner, current_fold: int, num_folds: int):
+    def __save_model(self, model, data_split: DataSplit):
         """
         Saves a model to disk.
 
-        :param model:           The model to be saved
-        :param current_fold:    The current fold starting at 0, or 0 if no cross validation is used
-        :param num_folds:       The total number of cross validation folds or 1, if no cross validation is used
+        :param model:       The model to be saved
+        :param data_split:  Information about the split of the available data, the model corresponds to
         """
         persistence = self.persistence
 
         if persistence is not None:
-            persistence.save_model(model, model_name=model.get_name(), fold=(current_fold if num_folds > 1 else None))
+            persistence.save_model(model, self.learner_name, data_split)
+
+    @staticmethod
+    def __check_for_parameter_changes(expected_params, actual_params):
+        changes = []
+
+        for key, expected_value in expected_params.items():
+            expected_value = str(expected_value)
+            actual_value = str(actual_params[key])
+
+            if actual_value != expected_value:
+                changes.append((key, expected_value, actual_value))
+
+        if len(changes) > 0:
+            log.warning(
+                'The loaded model\'s values for the following parameters differ from the expected configuration: %s',
+                reduce(
+                    lambda a, b: a +
+                    (', ' if len(a) > 0 else '') + '"' + b[0] + '" is "' + b[2] + '" instead of "' + b[1] + '"',
+                    changes, ''))
```

## mlrl/testbed/io.py

```diff
@@ -1,19 +1,18 @@
-#!/usr/bin/python
-
 """
 Author Michael Rapp (michael.rapp.ml@gmail.com)
 
 Provides functions for writing and reading files.
 """
 import os
 import os.path as path
 import xml.etree.ElementTree as XmlTree
-from csv import DictReader, DictWriter, QUOTE_MINIMAL
 
+from csv import QUOTE_MINIMAL, DictReader, DictWriter
+from typing import Optional
 from xml.dom import minidom
 
 # The delimiter used to separate the columns in a CSV file
 CSV_DELIMITER = ','
 
 # The character used for quotations in a CSV file
 CSV_QUOTE_CHAR = '"'
@@ -23,43 +22,43 @@
 
 # The suffix of a CSV file
 SUFFIX_CSV = 'csv'
 
 # The suffix of an ARFF file
 SUFFIX_ARFF = 'arff'
 
-# The suffix of a XML file
+# The suffix of an XML file
 SUFFIX_XML = 'xml'
 
 
-def get_file_name(name: str, suffix: str):
+def get_file_name(name: str, suffix: str) -> str:
     """
     Returns a file name, including a suffix.
 
     :param name:    The name of the file (without suffix)
     :param suffix:  The suffix of the file
     :return:        The file name
     """
     return name + '.' + suffix
 
 
-def get_file_name_per_fold(name: str, suffix: str, fold: int):
+def get_file_name_per_fold(name: str, suffix: str, fold: Optional[int]) -> str:
     """
     Returns a file name, including a suffix, that corresponds to a certain fold.
 
     :param name:    The name of the file (without suffix)
     :param suffix:  The suffix of the file
     :param fold:    The cross validation fold, the file corresponds to, or None, if the file does not correspond to a
                     specific fold
     :return:        The file name
     """
-    return get_file_name(name + '_' + ('overall' if fold is None else 'fold_' + str(fold + 1)), suffix)
+    return get_file_name(name + '_' + ('overall' if fold is None else 'fold-' + str(fold + 1)), suffix)
 
 
-def open_writable_txt_file(directory: str, file_name: str, fold: int = None, append: bool = False):
+def open_writable_txt_file(directory: str, file_name: str, fold: Optional[int] = None, append: bool = False):
     """
     Opens a text file to be written to.
 
     :param directory:   The directory where the file is located
     :param file_name:   The name of the file to be opened (without suffix)
     :param fold:        The cross validation fold, the file corresponds to, or None, if the file does not correspond to
                         a specific fold
@@ -67,29 +66,29 @@
     :return:            The file that has been opened
     """
     file = path.join(directory, get_file_name_per_fold(file_name, SUFFIX_TEXT, fold))
     write_mode = 'a' if append and path.isfile(file) else 'w'
     return open(file, mode=write_mode)
 
 
-def open_readable_csv_file(directory: str, file_name: str, fold: int):
+def open_readable_csv_file(directory: str, file_name: str, fold: Optional[int] = None):
     """
     Opens a CSV file to be read from.
 
     :param directory:   The directory where the file is located
     :param file_name:   The name of the file to be opened (without suffix)
     :param fold:        The cross validation fold, the file corresponds to, or None, if the file does not correspond to
                         a specific fold
     :return:            The file that has been opened
     """
     file = path.join(directory, get_file_name_per_fold(file_name, SUFFIX_CSV, fold))
     return open(file, mode='r', newline='')
 
 
-def open_writable_csv_file(directory: str, file_name: str, fold: int = None, append: bool = False):
+def open_writable_csv_file(directory: str, file_name: str, fold: Optional[int] = None, append: bool = False):
     """
     Opens a CSV file to be written to.
 
     :param directory:   The directory where the file is located
     :param file_name:   The name of the file to be opened (without suffix)
     :param fold:        The cross validation fold, the file corresponds to, or None, if the file does not correspond to
                         a specific fold
@@ -116,26 +115,29 @@
     Creates and returns a `DictWriter` that allows to write a dictionary to a CSV file.
 
     :param csv_file:    The CSV file
     :param header:      A list that contains the headers of the CSV file. They must correspond to the keys in the
                         directory that should be written to the file
     :return:            The `DictWriter` that has been created
     """
-    csv_writer = DictWriter(csv_file, delimiter=CSV_DELIMITER, quotechar=CSV_QUOTE_CHAR, quoting=QUOTE_MINIMAL,
+    csv_writer = DictWriter(csv_file,
+                            delimiter=CSV_DELIMITER,
+                            quotechar=CSV_QUOTE_CHAR,
+                            quoting=QUOTE_MINIMAL,
                             fieldnames=header)
 
     if csv_file.mode == 'w':
         csv_writer.writeheader()
 
     return csv_writer
 
 
 def write_xml_file(xml_file, root_element: XmlTree.Element, encoding='utf-8'):
     """
-    Writes a XML structure to a file.
+    Writes an XML structure to a file.
 
     :param xml_file:        The XML file
     :param root_element:    The root element of the XML structure
     :param encoding:        The encoding to be used
     """
     with open(xml_file, mode='w') as file:
         xml_string = minidom.parseString(XmlTree.tostring(root_element)).toprettyxml(encoding=encoding)
```

## mlrl/testbed/main_boomer.py

```diff
@@ -1,123 +1,20 @@
-#!/usr/bin/python
-
 """
 Author: Michael Rapp (michael.rapp.ml@gmail.com)
 """
-from argparse import ArgumentParser
+from mlrl.boosting.boosting_learners import Boomer
+from mlrl.boosting.config import BOOSTING_RULE_LEARNER_PARAMETERS
+from mlrl.boosting.cython.learner_boomer import BoomerConfig
 
-from mlrl.common.rule_learners import AUTOMATIC, RULE_MODEL_ASSEMBLAGE_VALUES
-from mlrl.common.strings import format_dict_keys, format_string_set
-from mlrl.testbed.args import add_rule_learner_arguments, PARAM_HEAD_TYPE, PARAM_PARALLEL_RULE_REFINEMENT, \
-    PARAM_PARALLEL_STATISTIC_UPDATE
 from mlrl.testbed.runnables import RuleLearnerRunnable
 
-from mlrl.boosting.boosting_learners import Boomer, HEAD_TYPE_VALUES, EARLY_STOPPING_VALUES, LABEL_BINNING_VALUES, \
-    LOSS_VALUES, PREDICTOR_VALUES, PARALLEL_VALUES, FEATURE_BINNING_VALUES
-
-PARAM_RULE_MODEL_ASSEMBLAGE = '--rule-model-assemblage'
-
-PARAM_EARLY_STOPPING = '--early-stopping'
-
-PARAM_FEATURE_BINNING = '--feature-binning'
-
-PARAM_LABEL_BINNING = '--label-binning'
-
-PARAM_LOSS = '--loss'
-
-PARAM_SHRINKAGE = '--shrinkage'
-
-PARAM_PREDICTOR = '--predictor'
-
-PARAM_L1_REGULARIZATION_WEIGHT = '--l1-regularization-weight'
-
-PARAM_L2_REGULARIZATION_WEIGHT = '--l2-regularization-weight'
-
-
-class BoomerRunnable(RuleLearnerRunnable):
-
-    def _create_learner(self, args):
-        return Boomer(random_state=args.random_state,
-                      feature_format=args.feature_format,
-                      label_format=args.label_format,
-                      prediction_format=args.prediction_format,
-                      rule_model_assemblage=args.rule_model_assemblage,
-                      rule_induction=args.rule_induction,
-                      max_rules=args.max_rules,
-                      time_limit=args.time_limit,
-                      early_stopping=args.early_stopping,
-                      loss=args.loss,
-                      predictor=args.predictor,
-                      pruning=args.pruning,
-                      label_sampling=args.label_sampling,
-                      instance_sampling=args.instance_sampling,
-                      shrinkage=args.shrinkage,
-                      feature_sampling=args.feature_sampling,
-                      holdout=args.holdout,
-                      feature_binning=args.feature_binning,
-                      label_binning=args.label_binning,
-                      head_type=args.head_type,
-                      l1_regularization_weight=args.l1_regularization_weight,
-                      l2_regularization_weight=args.l2_regularization_weight,
-                      parallel_rule_refinement=args.parallel_rule_refinement,
-                      parallel_statistic_update=args.parallel_statistic_update,
-                      parallel_prediction=args.parallel_prediction)
-
-
-def __add_arguments(parser: ArgumentParser):
-    add_rule_learner_arguments(parser)
-    parser.add_argument(PARAM_RULE_MODEL_ASSEMBLAGE, type=str,
-                        help='The name of the algorithm to be used for the induction of several rule. Must be one of '
-                             + format_string_set(RULE_MODEL_ASSEMBLAGE_VALUES) + '. For additional options refer to '
-                             + 'the documentation.')
-    parser.add_argument(PARAM_EARLY_STOPPING, type=str,
-                        help='The name of the strategy to be used for early stopping. Must be one of '
-                             + format_dict_keys(EARLY_STOPPING_VALUES) + '. For additional options refer to the '
-                             + 'documentation.')
-    parser.add_argument(PARAM_FEATURE_BINNING, type=str,
-                        help='The name of the strategy to be used for feature binning. Must be one of '
-                             + format_dict_keys(FEATURE_BINNING_VALUES) + '. If set to "' + AUTOMATIC + '", the most '
-                             + 'suitable strategy is chosen automatically based on the characteristics of the feature '
-                             + 'matrix. For additional options refer to the documentation.')
-    parser.add_argument(PARAM_LABEL_BINNING, type=str,
-                        help='The name of the strategy to be used for gradient-based label binning (GBLB). Must be one '
-                             + 'of ' + format_dict_keys(LABEL_BINNING_VALUES) + '. If set to "' + AUTOMATIC + '", the '
-                             + 'most suitable strategy is chosen automatically based on the parameters ' + PARAM_LOSS
-                             + ' and ' + PARAM_HEAD_TYPE + '. For additional options refer to the documentation.')
-    parser.add_argument(PARAM_SHRINKAGE, type=float,
-                        help='The shrinkage parameter, a.k.a. the learning rate, to be used. Must be in (0, 1].')
-    parser.add_argument(PARAM_LOSS, type=str,
-                        help='The name of the loss function to be minimized during training. Must be one of '
-                             + format_string_set(LOSS_VALUES) + '.')
-    parser.add_argument(PARAM_PREDICTOR, type=str,
-                        help='The name of the strategy to be used for making predictions. Must be one of '
-                             + format_string_set(PREDICTOR_VALUES) + '. If set to "' + AUTOMATIC + '", the most '
-                             + 'suitable strategy is chosen automatically based on the parameter ' + PARAM_LOSS + '.')
-    parser.add_argument(PARAM_L1_REGULARIZATION_WEIGHT, type=float,
-                        help='The weight of the L1 regularization. Must be at least 0.')
-    parser.add_argument(PARAM_L2_REGULARIZATION_WEIGHT, type=float,
-                        help='The weight of the L2 regularization. Must be at least 0.')
-    parser.add_argument(PARAM_HEAD_TYPE, type=str,
-                        help='The type of the rule heads that should be used. Must be one of '
-                             + format_string_set(HEAD_TYPE_VALUES) + '. If set to "' + AUTOMATIC + '", the most '
-                             + 'suitable type is chosen automatically based on the parameter ' + PARAM_LOSS + '.')
-    parser.add_argument(PARAM_PARALLEL_RULE_REFINEMENT, type=str,
-                        help='Whether potential refinements of rules should be searched for in parallel or not. Must '
-                             + 'be one of ' + format_dict_keys(PARALLEL_VALUES) + '. If set to "' + AUTOMATIC
-                             + '", the most suitable strategy is chosen automatically based on the parameter '
-                             + PARAM_LOSS + '. For additional options refer to the documentation.')
-    parser.add_argument(PARAM_PARALLEL_STATISTIC_UPDATE, type=str,
-                        help='Whether the gradients and Hessians for different examples should be calculated in '
-                             + 'parallel or not. Must be one of ' + format_dict_keys(PARALLEL_VALUES) + '. If set '
-                             + 'to "' + AUTOMATIC + '", the most suitable strategy is chosen automatically based on '
-                             + 'the parameter ' + PARAM_LOSS + '. For additional options refer to the documentation.')
-
 
 def main():
-    parser = ArgumentParser(description='Allows to run experiments using the BOOMER algorithm')
-    __add_arguments(parser)
-    runnable = BoomerRunnable()
-    runnable.run(parser)
+    RuleLearnerRunnable(description='Allows to run experiments using the BOOMER algorithm',
+                        learner_name='boomer',
+                        learner_type=Boomer,
+                        config_type=BoomerConfig,
+                        parameters=BOOSTING_RULE_LEARNER_PARAMETERS).run()
 
 
 if __name__ == '__main__':
     main()
```

## mlrl/testbed/model_characteristics.py

```diff
@@ -1,581 +1,316 @@
-#!/usr/bin/python
-
 """
 Author: Michael Rapp (michael.rapp.ml@gmail.com)
 
-Provides classes for printing textual representations of models. The models can be written to one or several outputs,
-e.g. to the console or to a file.
+Provides classes for printing certain characteristics of models. The characteristics can be written to one or several
+outputs, e.g., to the console or to a file.
 """
 import logging as log
-from _io import StringIO
-from abc import ABC, abstractmethod
-from typing import List, Set
+
+from abc import ABC
+from typing import Any, Dict, List, Optional
 
 import numpy as np
-from mlrl.common.cython.rule_model import RuleModelVisitor, EmptyBody, ConjunctiveBody, CompleteHead, PartialHead
+
+from mlrl.common.cython.rule_model import CompleteHead, ConjunctiveBody, EmptyBody, PartialHead, RuleModel, \
+    RuleModelVisitor
 from mlrl.common.learners import Learner
 from mlrl.common.options import Options
-from mlrl.testbed.data import Attribute, MetaData
-from mlrl.testbed.io import clear_directory, open_writable_txt_file, open_writable_csv_file, create_csv_dict_writer
-
-ARGUMENT_PRINT_FEATURE_NAMES = 'print_feature_names'
 
-ARGUMENT_PRINT_LABEL_NAMES = 'print_label_names'
+from mlrl.testbed.data import MetaData
+from mlrl.testbed.data_splitting import DataSplit, DataType
+from mlrl.testbed.format import format_float, format_percentage, format_table
+from mlrl.testbed.output_writer import Formattable, OutputWriter, Tabularizable
+from mlrl.testbed.prediction_scope import PredictionScope, PredictionType
 
-ARGUMENT_PRINT_NOMINAL_VALUES = 'print_nominal_values'
 
-PRINT_OPTION_VALUES: Set[str] = {ARGUMENT_PRINT_FEATURE_NAMES, ARGUMENT_PRINT_LABEL_NAMES,
-                                 ARGUMENT_PRINT_NOMINAL_VALUES}
-
-
-class RuleModelFormatter(RuleModelVisitor):
+class ModelCharacteristicsWriter(OutputWriter, ABC):
     """
-    Allows to create textual representation of the rules in a `RuleModel`.
+    An abstract base class for all classes that allow to write the characteristics of a model to one or several sinks.
     """
 
-    def __init__(self, attributes: List[Attribute], labels: List[Attribute], print_feature_names: bool,
-                 print_label_names: bool, print_nominal_values: bool):
-        """
-        :param attributes:              A list that contains the attributes
-        :param labels:                  A list that contains the labels
-        :param print_feature_names:     True, if the names of features should be printed, False otherwise
-        :param print_label_names:       True, if the names of labels should be printed, False otherwise
-        :param print_nominal_values:    True, if the values of nominal values should be printed, False otherwise
-        """
-        self.print_feature_names = print_feature_names
-        self.print_label_names = print_label_names
-        self.print_nominal_values = print_nominal_values
-        self.attributes = attributes
-        self.labels = labels
-        self.text = StringIO()
-
-    def visit_empty_body(self, _: EmptyBody):
-        self.text.write('{}')
-
-    def __format_conditions(self, num_conditions: int, indices: np.ndarray, thresholds: np.ndarray,
-                            operator: str) -> int:
-        result = num_conditions
-
-        if indices is not None and thresholds is not None:
-            text = self.text
-            attributes = self.attributes
-            print_feature_names = self.print_feature_names
-            print_nominal_values = self.print_nominal_values
-
-            for i in range(indices.shape[0]):
-                if result > 0:
-                    text.write(' & ')
-
-                feature_index = indices[i]
-                threshold = thresholds[i]
-                attribute = attributes[feature_index] if len(attributes) > feature_index else None
-
-                if print_feature_names and attribute is not None:
-                    text.write(attribute.attribute_name)
-                else:
-                    text.write(str(feature_index))
-
-                text.write(' ')
-                text.write(operator)
-                text.write(' ')
-
-                if attribute is not None and attribute.nominal_values is not None:
-                    nominal_value = int(threshold)
-
-                    if print_nominal_values and len(attribute.nominal_values) > nominal_value:
-                        text.write('"' + attribute.nominal_values[nominal_value] + '"')
-                    else:
-                        text.write(str(nominal_value))
-                else:
-                    text.write(str(threshold))
-
-                result += 1
-
-        return result
-
-    def visit_conjunctive_body(self, body: ConjunctiveBody):
-        text = self.text
-        text.write('{')
-        num_conditions = self.__format_conditions(0, body.leq_indices, body.leq_thresholds, '<=')
-        num_conditions = self.__format_conditions(num_conditions, body.gr_indices, body.gr_thresholds, '>')
-        num_conditions = self.__format_conditions(num_conditions, body.eq_indices, body.eq_thresholds, '==')
-        self.__format_conditions(num_conditions, body.neq_indices, body.neq_thresholds, '!=')
-        text.write('}')
-
-    def visit_complete_head(self, head: CompleteHead):
-        text = self.text
-        print_label_names = self.print_label_names
-        labels = self.labels
-        scores = head.scores
-        text.write(' => (')
-
-        for i in range(scores.shape[0]):
-            if i > 0:
-                text.write(', ')
-
-            if print_label_names and len(labels) > i:
-                text.write(labels[i].attribute_name)
-            else:
-                text.write(str(i))
-
-            text.write(' = ')
-            text.write('{0:.2f}'.format(scores[i]))
-
-        text.write(')\n')
-
-    def visit_partial_head(self, head: PartialHead):
-        text = self.text
-        print_label_names = self.print_label_names
-        labels = self.labels
-        indices = head.indices
-        scores = head.scores
-        text.write(' => (')
-
-        for i in range(indices.shape[0]):
-            if i > 0:
-                text.write(', ')
-
-            label_index = indices[i]
-
-            if print_label_names and len(labels) > label_index:
-                text.write(labels[label_index].attribute_name)
-            else:
-                text.write(str(label_index))
-
-            text.write(' = ')
-            text.write('{0:.2f}'.format(scores[i]))
-
-        text.write(')\n')
-
-    def get_text(self) -> str:
+    class LogSink(OutputWriter.LogSink):
         """
-        Returns the textual representation that has been created via the `format` method.
-
-        :return: The textual representation
+        Allows to write the characteristics of a model to the console.
         """
-        return self.text.getvalue()
-
-
-class ModelPrinterOutput(ABC):
-    """
-    An abstract base class for all outputs, textual representations of models may be written to.
-    """
-
-    @abstractmethod
-    def write_model(self, experiment_name: str, model: str, total_folds: int, fold: int = None):
-        """
-        Write a textual representation of a model to the output.
-
-        :param experiment_name:     The name of the experiment
-        :param model:               The textual representation of the model
-        :param total_folds:         The total number of folds
-        :param fold:                The fold for which the results should be written or None, if no cross validation is
-                                    used or if the overall results, averaged over all folds, should be written
-        """
-        pass
-
-
-class ModelPrinter(ABC):
-    """
-    An abstract base class for all classes that allow to print a textual representation of a `Learner`'s model.
-    """
-
-    def __init__(self, print_options: str, outputs: List[ModelPrinterOutput]):
-        """
-        :param print_options:   The options to be used for printing models
-        :param outputs:         The outputs, the textual representations of models should be written to
-        """
-        self.outputs = outputs
-
-        try:
-            self.print_options = Options.create(print_options, PRINT_OPTION_VALUES)
-        except ValueError as e:
-            raise ValueError('Invalid value given for parameter "print_options". ' + str(e))
-
-    def print(self, experiment_name: str, meta_data: MetaData, learner: Learner, current_fold: int, num_folds: int):
-        """
-        Prints a textual representation of a `Learner`'s model.
-
-        :param experiment_name: The name of the experiment
-        :param meta_data:       The meta data of the training data set
-        :param learner:         The learner
-        :param current_fold:    The current cross validation fold starting at 0, or 0 if no cross validation is used
-        :param num_folds:       The total number of cross validation folds or 1, if no cross validation is used
-        """
-        model = learner.model_
-        text = self._format_model(meta_data, model)
-
-        for output in self.outputs:
-            output.write_model(experiment_name, text, num_folds, current_fold if num_folds > 1 else None)
-
-    @abstractmethod
-    def _format_model(self, meta_data: MetaData, model) -> str:
-        """
-        Must be implemented by subclasses in order to create a textual representation of a model.
-
-        :param meta_data:   The meta data of the training data set
-        :param model:       The model
-        :return:            The textual representation of the given model
-        """
-        pass
-
-
-class ModelPrinterLogOutput(ModelPrinterOutput):
-    """
-    Outputs the textual representation of a model using the logger.
-    """
-
-    def write_model(self, experiment_name: str, model: str, total_folds: int, fold: int = None):
-        msg = 'Model for experiment \"' + experiment_name + '\"' + (
-            ' (Fold ' + str(fold + 1) + ')' if fold is not None else '') + ':\n\n%s'
-        log.info(msg, model)
-
 
-class ModelPrinterTxtOutput(ModelPrinterOutput):
-    """
-    Writes the textual representation of a model to a text file.
-    """
+        def __init__(self):
+            super().__init__(title='Model characteristics')
 
-    def __init__(self, output_dir: str, clear_dir: bool = True):
-        self.output_dir = output_dir
-        self.clear_dir = clear_dir
-
-    def write_model(self, experiment_name: str, model: str, total_folds: int, fold: int = None):
-        with open_writable_txt_file(self.output_dir, 'rules', fold, append=False) as text_file:
-            text_file.write(model)
-
-    def __clear_dir_if_necessary(self):
+    class CsvSink(OutputWriter.CsvSink):
         """
-        Clears the output directory, if necessary.
+        Allows to write the characteristics of a model to CSV files.
         """
-        if self.clear_dir:
-            clear_directory(self.output_dir)
-            self.clear_dir = False
-
 
-class RulePrinter(ModelPrinter):
-    """
-    Allows to print a textual representation of a `MLRuleLearner`'s rule-based model.
-    """
+        def __init__(self, output_dir: str):
+            super().__init__(output_dir=output_dir, file_name='model_characteristics')
 
-    def __init__(self, print_options: str, outputs: List[ModelPrinterOutput]):
-        super().__init__(print_options, outputs)
+    def __init__(self, sinks: List[OutputWriter.Sink]):
+        super().__init__(sinks)
 
-    def _format_model(self, meta_data: MetaData, model) -> str:
-        print_options = self.print_options
-        print_feature_names = print_options.get_bool(ARGUMENT_PRINT_FEATURE_NAMES, True)
-        print_label_names = print_options.get_bool(ARGUMENT_PRINT_LABEL_NAMES, True)
-        print_nominal_values = print_options.get_bool(ARGUMENT_PRINT_NOMINAL_VALUES, True)
-        formatter = RuleModelFormatter(attributes=meta_data.attributes, labels=meta_data.labels,
-                                       print_feature_names=print_feature_names, print_label_names=print_label_names,
-                                       print_nominal_values=print_nominal_values)
-        model.visit(formatter)
-        return formatter.get_text()
 
-
-class RuleModelCharacteristics:
+class RuleModelCharacteristicsWriter(ModelCharacteristicsWriter):
     """
-    Stores the characteristics of a `RuleModel`.
+    Allows to write the characteristics of a `RuleModel` to one or several sinks.
     """
 
-    def __init__(self, default_rule_index: int, default_rule_pos_predictions: int, default_rule_neg_predictions: int,
-                 num_leq: np.ndarray, num_gr: np.ndarray, num_eq: np.ndarray, num_neq: np.ndarray,
-                 num_pos_predictions: np.ndarray, num_neg_predictions: np.ndarray):
-        """
-        :param default_rule_index:              The index of the default rule or None, if no default rule is used
-        :param default_rule_pos_predictions:    The number of positive predictions of the default rule, if any
-        :param default_rule_neg_predictions:    The number of negative predictions of the default rule, if any
-        :param num_leq:                         A `np.ndarray`, shape `(num_rules)` that stores the number of conditions
-                                                that use the <= operator per rule
-        :param num_gr:                          A `np.ndarray`, shape `(num_rules)` that stores the number of conditions
-                                                that use the > operator per rule
-        :param num_eq:                          A `np.ndarray`, shape `(num_rules)` that stores the number of conditions
-                                                that use the == operator per rule
-        :param num_neq:                         A `np.ndarray`, shape `(num_rules)` that stores the number of conditions
-                                                that use the != operator per rule
-        :param num_pos_predictions:             A `np.ndarray`, shape `(num_rules)` that stores the number of positive
-                                                predictions per rule
-        :param num_neg_predictions:             A `np.ndarray`, shape `(num_rules)` that stores the number of negative
-                                                predictions per rule
+    class RuleModelCharacteristics(Formattable, Tabularizable):
         """
-        self.default_rule_index = default_rule_index
-        self.default_rule_pos_predictions = default_rule_pos_predictions
-        self.default_rule_neg_predictions = default_rule_neg_predictions
-        self.num_leq = num_leq
-        self.num_gr = num_gr
-        self.num_eq = num_eq
-        self.num_neq = num_neq
-        self.num_pos_predictions = num_pos_predictions
-        self.num_neg_predictions = num_neg_predictions
-
-
-class RuleModelCharacteristicsOutput(ABC):
-    """
-    An abstract base class for all outputs, the characteristics of a `MLRuleLearner`'s model may be written to.
-    """
-
-    @abstractmethod
-    def write_model_characteristics(self, experiment_name: str, characteristics: RuleModelCharacteristics,
-                                    total_folds: int, fold: int = None):
-        """
-        Writes the characteristics of a `RuleModel` to the output.
-
-        :param experiment_name: The name of the experiment
-        :param characteristics: The characteristics of the model
-        :param total_folds:     The total number of folds
-        :param fold:            The fold for which the characteristics should be written or None, if no cross validation
-                                is used
+        Stores the characteristics of a `RuleModel`.
         """
-        pass
-
-
-class RuleModelCharacteristicsVisitor(RuleModelVisitor):
-    """
-    A visitor that allows to determine the characteristics of a `RuleModel`.
-    """
-
-    def __init__(self):
-        self.num_leq = []
-        self.num_gr = []
-        self.num_eq = []
-        self.num_neq = []
-        self.num_pos_predictions = []
-        self.num_neg_predictions = []
-        self.default_rule_index = None
-        self.default_rule_pos_predictions = 0
-        self.default_rule_neg_predictions = 0
-        self.index = -1
-
-    def visit_empty_body(self, _: EmptyBody):
-        self.index += 1
-        self.default_rule_index = self.index
-
-    def visit_conjunctive_body(self, body: ConjunctiveBody):
-        self.index += 1
-        self.num_leq.append(body.leq_indices.shape[0] if body.leq_indices is not None else 0)
-        self.num_gr.append(body.gr_indices.shape[0] if body.gr_indices is not None else 0)
-        self.num_eq.append(body.eq_indices.shape[0] if body.eq_indices is not None else 0)
-        self.num_neq.append(body.neq_indices.shape[0] if body.neq_indices is not None else 0)
-
-    def visit_complete_head(self, head: CompleteHead):
-        num_pos_predictions = np.count_nonzero(head.scores > 0)
-        num_neg_predictions = head.scores.shape[0] - num_pos_predictions
-
-        if self.index == self.default_rule_index:
-            self.default_rule_pos_predictions = num_pos_predictions
-            self.default_rule_neg_predictions = num_neg_predictions
-        else:
-            self.num_pos_predictions.append(num_pos_predictions)
-            self.num_neg_predictions.append(num_neg_predictions)
-
-    def visit_partial_head(self, head: PartialHead):
-        num_pos_predictions = np.count_nonzero(head.scores > 0)
-        num_neg_predictions = head.scores.shape[0] - num_pos_predictions
-
-        if self.index == self.default_rule_index:
-            self.default_rule_pos_predictions = num_pos_predictions
-            self.default_rule_neg_predictions = num_neg_predictions
-        else:
-            self.num_pos_predictions.append(num_pos_predictions)
-            self.num_neg_predictions.append(num_neg_predictions)
-
-
-class RuleModelCharacteristicsLogOutput(RuleModelCharacteristicsOutput):
-    """
-    Outputs the characteristics of a `RuleModel` using the logger.
-    """
-
-    def write_model_characteristics(self, experiment_name: str, characteristics: RuleModelCharacteristics,
-                                    total_folds: int, fold: int = None):
-        default_rule_index = characteristics.default_rule_index
-        num_pos_predictions = characteristics.num_pos_predictions
-        num_neg_predictions = characteristics.num_neg_predictions
-        num_predictions = num_pos_predictions + num_neg_predictions
-        num_leq = characteristics.num_leq
-        num_gr = characteristics.num_gr
-        num_eq = characteristics.num_eq
-        num_neq = characteristics.num_neq
-        num_conditions = num_leq + num_gr + num_eq + num_neq
-        num_total_conditions = np.sum(num_conditions)
-        frac_leq = np.sum(num_leq) / num_total_conditions * 100
-        frac_gr = np.sum(num_gr) / num_total_conditions * 100
-        frac_eq = np.sum(num_eq) / num_total_conditions * 100
-        frac_neq = 100 - frac_leq - frac_gr - frac_eq
-        num_total_predictions = np.sum(num_predictions)
-        frac_pos = np.sum(num_pos_predictions) / num_total_predictions * 100
-        frac_neg = 100 - frac_pos
-        num_rules = num_predictions.shape[0]
-        msg = 'Model characteristics for experiment \"' + experiment_name + '\"' + (
-            ' (Fold ' + str(fold + 1) + ')' if fold is not None else '') + ':\n\n'
-        msg += 'Rules: ' + str(num_rules)
-        if default_rule_index is not None:
-            msg += ' (plus a default rule with ' + str(
-                characteristics.default_rule_pos_predictions) + ' positive and ' + str(
-                characteristics.default_rule_neg_predictions) + ' negative predictions that is excluded from the ' \
-                   + 'following statistics)'
-        msg += '\n'
-        msg += 'Conditions per rule: avg. ' + str(np.mean(num_conditions)) + ', min. ' + str(
-            np.min(num_conditions)) + ', max. ' + str(np.max(num_conditions)) + '\n'
-        msg += 'Conditions total: ' + str(num_total_conditions) + ' (' + str(frac_leq) + '% use <= operator, ' + str(
-            frac_gr) + '% use > operator, ' + str(frac_eq) + '% use == operator, ' + str(
-            frac_neq) + '% use != operator)\n'
-        msg += 'Predictions per rule: avg. ' + str(np.mean(num_predictions)) + ', min. ' + str(
-            np.min(num_predictions)) + ', max. ' + str(np.max(num_predictions)) + '\n'
-        msg += 'Predictions total: ' + str(num_total_predictions) + ' (' + str(frac_pos) + '% positive, ' + str(
-            frac_neg) + '% negative)\n'
-        log.info(msg)
-
-
-class RuleModelCharacteristicsCsvOutput(RuleModelCharacteristicsOutput):
-    """
-    Writes the characteristics of a `RuleModel` to a CSV file.
-    """
-
-    COL_RULE_NAME = 'Rule'
 
-    COL_CONDITIONS = 'conditions'
+        def __init__(self, default_rule_index: int, default_rule_pos_predictions: int,
+                     default_rule_neg_predictions: int, num_leq: np.ndarray, num_gr: np.ndarray, num_eq: np.ndarray,
+                     num_neq: np.ndarray, num_pos_predictions: np.ndarray, num_neg_predictions: np.ndarray):
+            """
+            :param default_rule_index:              The index of the default rule or None, if no default rule is used
+            :param default_rule_pos_predictions:    The number of positive predictions of the default rule, if any
+            :param default_rule_neg_predictions:    The number of negative predictions of the default rule, if any
+            :param num_leq:                         A `np.ndarray`, shape `(num_rules)` that stores the number of
+                                                    conditions that use the <= operator per rule
+            :param num_gr:                          A `np.ndarray`, shape `(num_rules)` that stores the number of
+                                                    conditions that use the > operator per rule
+            :param num_eq:                          A `np.ndarray`, shape `(num_rules)` that stores the number of
+                                                    conditions that use the == operator per rule
+            :param num_neq:                         A `np.ndarray`, shape `(num_rules)` that stores the number of
+                                                    conditions that use the != operator per rule
+            :param num_pos_predictions:             A `np.ndarray`, shape `(num_rules)` that stores the number of
+                                                    positive predictions per rule
+            :param num_neg_predictions:             A `np.ndarray`, shape `(num_rules)` that stores the number of
+                                                    negative predictions per rule
+            """
+            self.default_rule_index = default_rule_index
+            self.default_rule_pos_predictions = default_rule_pos_predictions
+            self.default_rule_neg_predictions = default_rule_neg_predictions
+            self.num_leq = num_leq
+            self.num_gr = num_gr
+            self.num_eq = num_eq
+            self.num_neq = num_neq
+            self.num_pos_predictions = num_pos_predictions
+            self.num_neg_predictions = num_neg_predictions
 
-    COL_NUMERICAL_CONDITIONS = 'numerical conditions'
+        def format(self, _: Options, **kwargs):
+            num_predictions = self.num_pos_predictions + self.num_neg_predictions
+            num_conditions = self.num_leq + self.num_gr + self.num_eq + self.num_neq
+            num_total_conditions = np.sum(num_conditions)
 
-    COL_LEQ_CONDITIONS = 'conditions using <= operator'
+            if num_total_conditions > 0:
+                frac_leq = np.sum(self.num_leq) / num_total_conditions * 100
+                frac_gr = np.sum(self.num_gr) / num_total_conditions * 100
+                frac_eq = np.sum(self.num_eq) / num_total_conditions * 100
+                frac_neq = np.sum(self.num_neq) / num_total_conditions * 100
+                num_conditions_mean = np.mean(num_conditions)
+                num_conditions_min = np.min(num_conditions)
+                num_conditions_max = np.max(num_conditions)
 
-    COL_GR_CONDITIONS = 'conditions using > operator'
-
-    COL_NOMINAL_CONDITIONS = 'nominal conditions'
-
-    COL_EQ_CONDITIONS = 'conditions using == operator'
-
-    COL_NEQ_CONDITIONS = 'conditions using != operator'
-
-    COL_PREDICTIONS = 'predictions'
-
-    COL_POS_PREDICTIONS = 'pos. predictions'
-
-    COL_NEG_PREDICTIONS = 'neg. predictions'
-
-    def __init__(self, output_dir: str, clear_dir: bool = True):
-        """
-        :param output_dir:  The path of the directory, the CSV files should be written to
-        :param clear_dir:   True, if the directory, the CSV files should be written to, should be cleared
-        """
-        self.output_dir = output_dir
-        self.clear_dir = clear_dir
-
-    def write_model_characteristics(self, experiment_name: str, characteristics: RuleModelCharacteristics,
-                                    total_folds: int, fold: int = None):
-        if fold is not None:
-            self.__clear_dir_if_necessary()
-            header = [
-                RuleModelCharacteristicsCsvOutput.COL_RULE_NAME,
-                RuleModelCharacteristicsCsvOutput.COL_CONDITIONS,
-                RuleModelCharacteristicsCsvOutput.COL_NUMERICAL_CONDITIONS,
-                RuleModelCharacteristicsCsvOutput.COL_LEQ_CONDITIONS,
-                RuleModelCharacteristicsCsvOutput.COL_GR_CONDITIONS,
-                RuleModelCharacteristicsCsvOutput.COL_NOMINAL_CONDITIONS,
-                RuleModelCharacteristicsCsvOutput.COL_EQ_CONDITIONS,
-                RuleModelCharacteristicsCsvOutput.COL_NEQ_CONDITIONS,
-                RuleModelCharacteristicsCsvOutput.COL_PREDICTIONS,
-                RuleModelCharacteristicsCsvOutput.COL_POS_PREDICTIONS,
-                RuleModelCharacteristicsCsvOutput.COL_NEG_PREDICTIONS
-            ]
-            default_rule_index = characteristics.default_rule_index
-            num_rules = len(characteristics.num_pos_predictions)
+            else:
+                frac_leq = 0.0
+                frac_gr = 0.0
+                frac_eq = 0.0
+                frac_neq = 0.0
+                num_conditions_mean = 0.0
+                num_conditions_min = 0.0
+                num_conditions_max = 0.0
+
+            num_total_predictions = np.sum(num_predictions)
+
+            if num_total_predictions > 0:
+                frac_pos = np.sum(self.num_pos_predictions) / num_total_predictions * 100
+                frac_neg = np.sum(self.num_neg_predictions) / num_total_predictions * 100
+                num_predictions_mean = np.mean(num_predictions)
+                num_predictions_min = np.min(num_predictions)
+                num_predictions_max = np.max(num_predictions)
+            else:
+                frac_pos = 0.0
+                frac_neg = 0.0
+                num_predictions_mean = 0.0
+                num_predictions_min = 0.0
+                num_predictions_max = 0.0
+
+            num_rules = num_predictions.shape[0]
+
+            header = ['Statistics about conditions', 'Total', '<= operator', '> operator', '== operator', '!= operator']
+            alignment = ['left', 'right', 'right', 'right', 'right', 'right']
+            rows = []
+
+            if self.default_rule_index is not None:
+                rows.append([
+                    'Default rule',
+                    str(0),
+                    format_percentage(0),
+                    format_percentage(0),
+                    format_percentage(0),
+                    format_percentage(0)
+                ])
+
+            rows.append([
+                str(num_rules) + ' local rules',
+                str(num_total_conditions),
+                format_percentage(frac_leq),
+                format_percentage(frac_gr),
+                format_percentage(frac_eq),
+                format_percentage(frac_neq)
+            ])
+            text = format_table(rows, header=header, alignment=alignment) + '\n\n'
+
+            header = ['Statistics about predictions', 'Total', 'Positive', 'Negative']
+            alignment = ['left', 'right', 'right', 'right']
+            rows = []
+
+            if self.default_rule_index is not None:
+                default_rule_num_predictions = self.default_rule_pos_predictions + self.default_rule_neg_predictions
+                default_rule_frac_pos = self.default_rule_pos_predictions / default_rule_num_predictions * 100
+                default_rule_frac_neg = self.default_rule_neg_predictions / default_rule_num_predictions * 100
+                rows.append([
+                    'Default rule',
+                    str(default_rule_num_predictions),
+                    format_percentage(default_rule_frac_pos),
+                    format_percentage(default_rule_frac_neg)
+                ])
+
+            rows.append([
+                str(num_rules) + ' local rules',
+                str(num_total_predictions),
+                format_percentage(frac_pos),
+                format_percentage(frac_neg)
+            ])
+            text += format_table(rows, header=header, alignment=alignment) + '\n\n'
+
+            header = ['Statistics per local rule', 'Minimum', 'Average', 'Maximum']
+            rows = []
+            rows.append([
+                'Conditions',
+                format_float(num_conditions_min),
+                format_float(num_conditions_mean),
+                format_float(num_conditions_max)
+            ])
+            rows.append([
+                'Predictions',
+                format_float(num_predictions_min),
+                format_float(num_predictions_mean),
+                format_float(num_predictions_max)
+            ])
+            return text + format_table(rows, header=header)
+
+        def tabularize(self, _: Options, **kwargs) -> Optional[List[Dict[str, str]]]:
+            rows = []
+            default_rule_index = self.default_rule_index
+            num_rules = len(self.num_pos_predictions)
             num_total_rules = num_rules if default_rule_index is None else num_rules + 1
+            n = 0
 
-            with open_writable_csv_file(self.output_dir, 'model_characteristics', fold) as csv_file:
-                csv_writer = create_csv_dict_writer(csv_file, header)
-                n = 0
-
-                for i in range(num_total_rules):
-                    rule_name = 'Rule ' + str(i + 1)
-
-                    if i == default_rule_index:
-                        rule_name += ' (Default rule)'
-                        num_leq = 0
-                        num_gr = 0
-                        num_eq = 0
-                        num_neq = 0
-                        num_pos_predictions = characteristics.default_rule_pos_predictions
-                        num_neg_predictions = characteristics.default_rule_neg_predictions
-                    else:
-                        num_leq = characteristics.num_leq[n]
-                        num_gr = characteristics.num_gr[n]
-                        num_eq = characteristics.num_eq[n]
-                        num_neq = characteristics.num_neq[n]
-                        num_pos_predictions = characteristics.num_pos_predictions[n]
-                        num_neg_predictions = characteristics.num_neg_predictions[n]
-                        n += 1
-
-                    num_numerical = num_leq + num_gr
-                    num_nominal = num_eq + num_neq
-                    num_conditions = num_numerical + num_nominal
-                    num_predictions = num_pos_predictions + num_neg_predictions
-                    columns = {
-                        RuleModelCharacteristicsCsvOutput.COL_RULE_NAME: rule_name,
-                        RuleModelCharacteristicsCsvOutput.COL_CONDITIONS: num_conditions,
-                        RuleModelCharacteristicsCsvOutput.COL_NUMERICAL_CONDITIONS: num_numerical,
-                        RuleModelCharacteristicsCsvOutput.COL_LEQ_CONDITIONS: num_leq,
-                        RuleModelCharacteristicsCsvOutput.COL_GR_CONDITIONS: num_gr,
-                        RuleModelCharacteristicsCsvOutput.COL_NOMINAL_CONDITIONS: num_nominal,
-                        RuleModelCharacteristicsCsvOutput.COL_EQ_CONDITIONS: num_eq,
-                        RuleModelCharacteristicsCsvOutput.COL_NEQ_CONDITIONS: num_neq,
-                        RuleModelCharacteristicsCsvOutput.COL_PREDICTIONS: num_predictions,
-                        RuleModelCharacteristicsCsvOutput.COL_POS_PREDICTIONS: num_pos_predictions,
-                        RuleModelCharacteristicsCsvOutput.COL_NEG_PREDICTIONS: num_neg_predictions
-                    }
-                    csv_writer.writerow(columns)
-
-    def __clear_dir_if_necessary(self):
-        """
-        Clears the output directory, if necessary.
-        """
-        if self.clear_dir:
-            clear_directory(self.output_dir)
-            self.clear_dir = False
+            for i in range(num_total_rules):
+                rule_name = 'Rule ' + str(i + 1)
 
+                if i == default_rule_index:
+                    rule_name += ' (Default rule)'
+                    num_leq = 0
+                    num_gr = 0
+                    num_eq = 0
+                    num_neq = 0
+                    num_pos_predictions = self.default_rule_pos_predictions
+                    num_neg_predictions = self.default_rule_neg_predictions
+                else:
+                    num_leq = self.num_leq[n]
+                    num_gr = self.num_gr[n]
+                    num_eq = self.num_eq[n]
+                    num_neq = self.num_neq[n]
+                    num_pos_predictions = self.num_pos_predictions[n]
+                    num_neg_predictions = self.num_neg_predictions[n]
+                    n += 1
+
+                num_numerical = num_leq + num_gr
+                num_nominal = num_eq + num_neq
+                num_conditions = num_numerical + num_nominal
+                num_predictions = num_pos_predictions + num_neg_predictions
+                rows.append({
+                    'Rule': rule_name,
+                    'conditions': num_conditions,
+                    'numerical conditions': num_numerical,
+                    'conditions using <= operator': num_leq,
+                    'conditions using > operator': num_gr,
+                    'nominal conditions': num_nominal,
+                    'conditions using == operator': num_eq,
+                    'conditions using != operator': num_neq,
+                    'predictions': num_predictions,
+                    'pos. predictions': num_pos_predictions,
+                    'neg. predictions': num_neg_predictions
+                })
+
+            return rows
+
+    class RuleModelCharacteristicsVisitor(RuleModelVisitor):
+        """
+        A visitor that allows to determine the characteristics of a `RuleModel`.
+        """
+
+        def __init__(self):
+            self.num_leq = []
+            self.num_gr = []
+            self.num_eq = []
+            self.num_neq = []
+            self.num_pos_predictions = []
+            self.num_neg_predictions = []
+            self.default_rule_index = None
+            self.default_rule_pos_predictions = 0
+            self.default_rule_neg_predictions = 0
+            self.index = -1
+
+        def visit_empty_body(self, _: EmptyBody):
+            self.index += 1
+            self.default_rule_index = self.index
+
+        def visit_conjunctive_body(self, body: ConjunctiveBody):
+            self.index += 1
+            self.num_leq.append(body.leq_indices.shape[0] if body.leq_indices is not None else 0)
+            self.num_gr.append(body.gr_indices.shape[0] if body.gr_indices is not None else 0)
+            self.num_eq.append(body.eq_indices.shape[0] if body.eq_indices is not None else 0)
+            self.num_neq.append(body.neq_indices.shape[0] if body.neq_indices is not None else 0)
+
+        def visit_complete_head(self, head: CompleteHead):
+            num_pos_predictions = np.count_nonzero(head.scores > 0)
+            num_neg_predictions = head.scores.shape[0] - num_pos_predictions
+
+            if self.index == self.default_rule_index:
+                self.default_rule_pos_predictions = num_pos_predictions
+                self.default_rule_neg_predictions = num_neg_predictions
+            else:
+                self.num_pos_predictions.append(num_pos_predictions)
+                self.num_neg_predictions.append(num_neg_predictions)
 
-class ModelCharacteristicsPrinter(ABC):
-    """
-    A class that allows to print the characteristics of a `Learner`'s model.
-    """
-
-    def print(self, experiment_name: str, learner: Learner, current_fold: int, num_folds: int):
-        model = learner.model_
-        self._print_model(experiment_name, current_fold, num_folds, model)
-
-    def _print_model(self, experiment_name: str, current_fold: int, num_folds: int, model):
-        """
-        :param experiment_name: The name of the experiment
-        :param current_fold:    The current fold
-        :param num_folds:       The total number of folds
-        :param model:           The model
-        """
-        pass
-
+        def visit_partial_head(self, head: PartialHead):
+            num_pos_predictions = np.count_nonzero(head.scores > 0)
+            num_neg_predictions = head.scores.shape[0] - num_pos_predictions
+
+            if self.index == self.default_rule_index:
+                self.default_rule_pos_predictions = num_pos_predictions
+                self.default_rule_neg_predictions = num_neg_predictions
+            else:
+                self.num_pos_predictions.append(num_pos_predictions)
+                self.num_neg_predictions.append(num_neg_predictions)
 
-class RuleModelCharacteristicsPrinter(ModelCharacteristicsPrinter):
-    """
-    A class that allows to print the characteristics of `MLRuleLearner`'s model.
-    """
+    def __init__(self, sinks: List[OutputWriter.Sink]):
+        super().__init__(sinks)
 
-    def __init__(self, outputs: List[RuleModelCharacteristicsOutput]):
-        """
-        :param outputs: The outputs, the characteristics of `RuleModel`s should be written to
-        """
-        self.outputs = outputs
+    def _generate_output_data(self, meta_data: MetaData, x, y, data_split: DataSplit, learner,
+                              data_type: Optional[DataType], prediction_type: Optional[PredictionType],
+                              prediction_scope: Optional[PredictionScope], predictions: Optional[Any],
+                              train_time: float, predict_time: float) -> Optional[Any]:
+        if isinstance(learner, Learner):
+            model = learner.model_
+
+            if isinstance(model, RuleModel):
+                visitor = RuleModelCharacteristicsWriter.RuleModelCharacteristicsVisitor()
+                model.visit_used(visitor)
+                return RuleModelCharacteristicsWriter.RuleModelCharacteristics(
+                    default_rule_index=visitor.default_rule_index,
+                    default_rule_pos_predictions=visitor.default_rule_pos_predictions,
+                    default_rule_neg_predictions=visitor.default_rule_neg_predictions,
+                    num_leq=np.asarray(visitor.num_leq),
+                    num_gr=np.asarray(visitor.num_gr),
+                    num_eq=np.asarray(visitor.num_eq),
+                    num_neq=np.asarray(visitor.num_neq),
+                    num_pos_predictions=np.asarray(visitor.num_pos_predictions),
+                    num_neg_predictions=np.asarray(visitor.num_neg_predictions))
 
-    def _print_model(self, experiment_name: str, current_fold: int, num_folds: int, model):
-        if len(self.outputs) > 0:
-            visitor = RuleModelCharacteristicsVisitor()
-            model.visit(visitor)
-            characteristics = RuleModelCharacteristics(
-                default_rule_index=visitor.default_rule_index,
-                default_rule_pos_predictions=visitor.default_rule_pos_predictions,
-                default_rule_neg_predictions=visitor.default_rule_neg_predictions, num_leq=np.asarray(visitor.num_leq),
-                num_gr=np.asarray(visitor.num_gr), num_eq=np.asarray(visitor.num_eq),
-                num_neq=np.asarray(visitor.num_neq), num_pos_predictions=np.asarray(visitor.num_pos_predictions),
-                num_neg_predictions=np.asarray(visitor.num_neg_predictions))
-
-            for output in self.outputs:
-                output.write_model_characteristics(experiment_name, characteristics, num_folds,
-                                                   current_fold if num_folds > 1 else None)
+        log.error('The learner does not support to obtain model characteristics')
+        return None
```

## mlrl/testbed/parameters.py

```diff
@@ -1,139 +1,35 @@
-#!/usr/bin/python
-
 """
 Author Michael Rapp (michael.rapp.ml@gmail.com)
 
-Provides classes for parameter tuning.
+Provides classes for loading and printing parameter settings that are used by a learner. The parameter settings can be
+written to one or several outputs, e.g., to the console or to a file. They can also be loaded from CSV files.
 """
-import logging as log
-from abc import ABC
-from abc import abstractmethod
-
-from mlrl.testbed.data import MetaData
-from mlrl.testbed.interfaces import Randomized
-from mlrl.testbed.io import clear_directory
-from mlrl.testbed.io import open_readable_csv_file, create_csv_dict_writer
-from mlrl.testbed.io import open_writable_csv_file, create_csv_dict_reader
-from mlrl.testbed.training import CrossValidation, DataSet
-from sklearn.model_selection import KFold
+from abc import ABC, abstractmethod
+from typing import Any, Dict, List, Optional
 
+from mlrl.common.options import Options
 
-class ParameterSearch(Randomized, ABC):
-    """
-    A base class for all classes that implement strategies to search for optimal parameters given a training data set.
-    """
-
-    @abstractmethod
-    def search(self, meta_data: MetaData, x, y, first_fold: int, current_fold: int, last_fold: int, num_folds: int):
-        """
-        Tests different parameter settings given a training data set.
-
-        :param meta_data:       The meta data of the training data set
-        :param x:               The feature matrix of the training examples
-        :param y:               The label matrix of the training examples
-        :param first_fold:      The first fold or 0, if no cross validation is used
-        :param current_fold:    The current fold starting at 0, or 0 if no cross validation is used
-        :param last_fold:       The last fold or 0, if no cross validation is used
-        :param num_folds:       The total number of cross validation folds or 1, if no cross validation is used
-        """
-        pass
-
-    @abstractmethod
-    def get_params(self):
-        """
-        Returns the best parameter setting tested so far.
-
-        :return: A dictionary that stores the parameters
-        """
-        pass
-
-    @abstractmethod
-    def get_score(self):
-        """
-        Returns the evaluation score that has been achieved using the best parameter setting.
-
-        :return: An evaluation score
-        """
-
-
-class NestedCrossValidation(ParameterSearch):
-    """
-    Allows to search for optimal parameters using (nested) cross validation.
-
-    """
-
-    def __init__(self, num_nested_folds: int):
-        """
-        :param num_nested_folds: The total number of folds to be used by the (nested) cross validation
-        """
-        self.num_nested_folds = num_nested_folds
-
-    def search(self, meta_data: MetaData, x, y, first_fold: int, current_fold: int, last_fold: int, num_folds: int):
-        num_nested_folds = self.num_nested_folds
-        random_state = self.random_state
-        first_nested_fold = 0
-        last_nested_fold = num_nested_folds - 1
-        i = 0
-        k_fold = KFold(n_splits=num_nested_folds, random_state=random_state, shuffle=True)
-
-        for train, test in k_fold.split(x, y):
-            log.info('Nested fold %s / %s:', (i + 1), num_nested_folds)
-
-            # Create training set for current fold
-            train_x = x[train]
-            train_y = y[train]
-
-            # Create test set for current fold
-            test_x = x[test]
-            test_y = y[test]
-
-            self._test_parameters(meta_data, train_x, train_y, test_x, test_y, first_outer_fold=first_fold,
-                                  current_outer_fold=current_fold, last_outer_fold=last_fold, num_outer_folds=num_folds,
-                                  first_nested_fold=first_nested_fold, current_nested_fold=i,
-                                  last_nested_fold=last_nested_fold, num_nested_folds=num_nested_folds)
-            i += 1
-
-    @abstractmethod
-    def _test_parameters(self, meta_data: MetaData, train_x, train_y, test_x, test_y, first_outer_fold: int,
-                         current_outer_fold: int, last_outer_fold: int, num_outer_folds: int, first_nested_fold: int,
-                         current_nested_fold: int, last_nested_fold: int, num_nested_folds: int):
-        """
-        Must be implemented by subclasses in order to test different parameter settings on a given training data set and
-        evaluate them on a test data set.
-
-        :param meta_data:       The meta data of the training data set
-        :param train_x:                The feature matrix of the training examples
-        :param train_y:                The label matrix of the training examples
-        :param test_x:                 The feature matrix of the test examples
-        :param test_y:                 The label matrix of the test examples
-        :param first_outer_fold:       The first (outer) fold or 0, if no cross validation is used
-        :param current_outer_fold:     The current (outer) fold starting at 0, or 0 if no cross validation is used
-        :param last_outer_fold:        The last (outer) fold or 0, if no cross validation is used
-        :param num_outer_folds:        The total number of (outer) cross validation folds or 1, if no cross validation
-                                       is used
-        :param first_nested_fold:      The first (nested) fold or 0, if no cross validation is used
-        :param current_nested_fold:    The current (nested) fold starting at 0, or 0 if no cross validation is used
-        :param last_nested_fold:       The last (nested) fold or 0, if no cross validation is used
-        :param num_nested_folds:       The total number of (nested) cross validation folds or 1, if no cross validation
-                                       is used
-        """
-        pass
+from mlrl.testbed.data import MetaData
+from mlrl.testbed.data_splitting import DataSplit, DataType
+from mlrl.testbed.format import format_table
+from mlrl.testbed.io import create_csv_dict_reader, open_readable_csv_file
+from mlrl.testbed.output_writer import Formattable, OutputWriter, Tabularizable
+from mlrl.testbed.prediction_scope import PredictionScope, PredictionType
 
 
 class ParameterInput(ABC):
 
     @abstractmethod
-    def read_parameters(self, fold: int = None) -> dict:
+    def read_parameters(self, data_split: DataSplit) -> dict:
         """
         Reads a parameter setting from the input.
 
-        :param fold:    The fold, the parameter setting corresponds to, or None, if the parameter setting does not
-                        correspond to a specific fold
-        :return:        A dictionary that stores the parameters
+        :param data_split:  Information about the split of the available data, the parameter setting corresponds to
+        :return:            A dictionary that stores the parameters
         """
         pass
 
 
 class ParameterCsvInput(ParameterInput):
     """
     Reads parameter settings from CSV files.
@@ -141,106 +37,75 @@
 
     def __init__(self, input_dir: str):
         """
         :param input_dir: The path of the directory, the CSV files should be read from
         """
         self.input_dir = input_dir
 
-    def read_parameters(self, fold: int = None) -> dict:
-        with open_readable_csv_file(self.input_dir, 'parameters', fold) as csv_file:
+    def read_parameters(self, data_split: DataSplit) -> dict:
+        with open_readable_csv_file(self.input_dir, 'parameters', data_split.get_fold()) as csv_file:
             csv_reader = create_csv_dict_reader(csv_file)
             return dict(next(csv_reader))
 
 
-class ParameterOutput(ABC):
+class ParameterWriter(OutputWriter):
     """
-    An abstract base class for all outputs, parameter settings may be written to.
+    Allows to write parameter settings to one or several sinks.
     """
 
-    @abstractmethod
-    def write_parameters(self, parameters: dict, score: float, total_folds: int, fold: int = None):
+    class Parameters(Formattable, Tabularizable):
         """
-        Writes a parameter setting to the output.
-
-        :param parameters:  A dictionary that stores the parameters
-        :param score:       The evaluation score that has been achieved using the parameter setting
-        :param total_folds: The total number of folds
-        :param fold:        The fold, the parameter setting corresponds to, or None, if the parameter setting does not
-                            correspond to a specific fold
+        Stores the parameter settings of a learner.
         """
-        pass
 
+        def __init__(self, learner):
+            """
+            :param learner: A learner
+            """
+            self.params = learner.get_params()
 
-class ParameterLogOutput(ParameterOutput):
-    """
-    Outputs parameter settings using the logger.
-    """
+        def format(self, _: Options, **kwargs):
+            params = self.params
+            rows = []
 
-    def write_parameters(self, parameters: dict, score: float, total_folds: int, fold: int = None):
-        param_text = ''
+            for key in sorted(params):
+                value = params[key]
 
-        for parameter, value in parameters.items():
-            if len(param_text) > 0:
-                param_text += '\n'
+                if value is not None:
+                    rows.append([str(key), str(value)])
 
-            param_text += (parameter + ': ' + str(value))
+            return format_table(rows)
 
-        score_text = 'Evaluation score: ' + str(score)
-        msg = 'Optimal parameter setting' + ('' if fold is None else ' (Fold ' + str(fold + 1) + ')') + ':\n\n%s\n%s\n'
-        log.info(msg, param_text, score_text)
+        def tabularize(self, _: Options, **kwargs) -> Optional[List[Dict[str, str]]]:
+            params = self.params
+            columns = {}
 
+            for key, value in params.items():
+                if value is not None:
+                    columns[key] = value
 
-class ParameterCsvOutput(ParameterOutput):
-    """
-    Writes parameter settings to CSV files.
-    """
+            return [columns]
 
-    def __init__(self, output_dir: str, clear_dir: bool = True):
+    class LogSink(OutputWriter.LogSink):
         """
-        :param output_dir: The path of the directory, the CSV files should be written to
+        Allows to write parameter settings to the console.
         """
-        self.output_dir = output_dir
-        self.clear_dir = clear_dir
 
-    def write_parameters(self, parameters: dict, score: float, total_folds: int, fold: int = None):
-        header = parameters.keys()
+        def __init__(self):
+            super().__init__(title='Custom parameters')
 
-        with open_writable_csv_file(self.output_dir, 'parameters', fold) as csv_file:
-            csv_writer = create_csv_dict_writer(csv_file, header)
-            csv_writer.writerow(parameters)
-
-    def __clear_dir_if_necessary(self):
+    class CsvSink(OutputWriter.CsvSink):
         """
-        Clears the output directory, if necessary.
+        Allows to write parameter settings to CSV files.
         """
-        if self.clear_dir:
-            clear_directory(self.output_dir)
-            self.clear_dir = False
-
 
-class ParameterTuning(CrossValidation):
-    """
-    Allows to tune parameters for a single training data set or all training data sets that are used in cross validation
-    using a `ParameterSearch` and writes the optimal parameters to one or several outputs.
-    """
+        def __init__(self, output_dir: str):
+            super().__init__(output_dir=output_dir, file_name='parameters')
 
-    def __init__(self, data_set: DataSet, num_folds: int, current_fold: int,
-                 parameter_search: ParameterSearch, *args: ParameterOutput):
-        """
-        :param parameter_search:    The strategy to be used to search for optimal parameters
-        :param args:                The outputs, the parameter settings should be written to
-        """
-        super().__init__(data_set, num_folds, current_fold)
-        self.parameter_search = parameter_search
-        self.outputs = args
-
-    def _train_and_evaluate(self, meta_data: MetaData, train_indices, train_x, train_y, test_indices, test_x, test_y,
-                            first_fold: int, current_fold: int, last_fold: int, num_folds: int):
-        parameter_search = self.parameter_search
-        parameter_search.random_state = self.random_state
-        parameter_search.search(meta_data, train_x, train_y, first_fold=first_fold, current_fold=current_fold,
-                                last_fold=last_fold, num_folds=num_folds)
-        parameters = parameter_search.get_params()
-        score = parameter_search.get_score()
+    def __init__(self, sinks: List[OutputWriter.Sink]):
+        super().__init__(sinks)
 
-        for output in self.outputs:
-            output.write_parameters(parameters, score, num_folds, current_fold if num_folds > 1 else None)
+    def _generate_output_data(self, meta_data: MetaData, x, y, data_split: DataSplit, learner,
+                              data_type: Optional[DataType], prediction_type: Optional[PredictionType],
+                              prediction_scope: Optional[PredictionScope], predictions: Optional[Any],
+                              train_time: float, predict_time: float) -> Optional[Any]:
+        return ParameterWriter.Parameters(learner)
```

## mlrl/testbed/persistence.py

```diff
@@ -1,84 +1,66 @@
-#!/usr/bin/python
-
 """
 Author: Michael Rapp (michael.rapp.ml@gmail.com)
 
 Provides classes for saving/loading models to/from disk.
 """
-import _pickle as pickle
 import logging as log
 import os.path as path
 
+import _pickle as pickle
+
+from mlrl.testbed.data_splitting import DataSplit
+from mlrl.testbed.io import get_file_name_per_fold
+
+SUFFIX_MODEL = 'model'
+
 
 class ModelPersistence:
     """
     Allows to save a model in a file and load it later.
     """
 
     def __init__(self, model_dir: str):
         """
         :param model_dir: The path of the directory where models should be saved
         """
         self.model_dir = model_dir
 
-    def save_model(self, model, model_name: str, fold: int = None):
+    def save_model(self, model, model_name: str, data_split: DataSplit):
         """
         Saves a model to a file.
 
         :param model:       The model to be persisted
         :param model_name:  The name of the model to be persisted
-        :param fold:        The fold, the model corresponds to, or None if no cross validation is used
+        :param data_split:  Information about the split of the available data, the model corresponds to
         """
-
-        file_path = path.join(self.model_dir, ModelPersistence.__get_file_name(model_name, fold))
+        file_name = get_file_name_per_fold(model_name, SUFFIX_MODEL, data_split.get_fold())
+        file_path = path.join(self.model_dir, file_name)
         log.debug('Saving model to file \"%s\"...', file_path)
 
         try:
             with open(file_path, mode='wb') as output_stream:
                 pickle.dump(model, output_stream, -1)
                 log.info('Successfully saved model to file \"%s\"', file_path)
         except IOError:
-            log.exception('Failed to save model to file \"%s\"', file_path)
+            log.error('Failed to save model to file \"%s\"', file_path)
 
-    def load_model(self, model_name: str, fold: int = None, raise_exception: bool = False):
+    def load_model(self, model_name: str, data_split: DataSplit):
         """
         Loads a model from a file.
 
-        :param model_name:      The name of the model to be loaded
-        :param fold:            The fold, the model corresponds to, or None if no cross validation is used
-        :param raise_exception: True, if an exception should be raised if an error occurs, False, if None should be
-                                returned in such case
-        :return:                The loaded model
+        :param model_name:  The name of the model to be loaded
+        :param data_split:  Information about the split of the available data, the model corresponds to
+        :return:            The loaded model
         """
-
-        file_path = path.join(self.model_dir, ModelPersistence.__get_file_name(model_name, fold))
+        file_name = get_file_name_per_fold(model_name, SUFFIX_MODEL, data_split.get_fold())
+        file_path = path.join(self.model_dir, file_name)
         log.debug("Loading model from file \"%s\"...", file_path)
 
         try:
             with open(file_path, mode='rb') as input_stream:
                 model = pickle.load(input_stream)
                 log.info('Successfully loaded model from file \"%s\"', file_path)
                 return model
-        except IOError as e:
+        except IOError:
             log.error('Failed to load model from file \"%s\"', file_path)
-
-            if raise_exception:
-                raise e
-            else:
-                return None
-
-    @staticmethod
-    def __get_file_name(model_name: str, fold: int):
-        """
-        Returns the name of the file that is used to persist a model.
-
-        :param model_name:          The name of the model to be persisted
-        :param fold:                The fold, the model corresponds to, or None if no cross validation is used
-        :return:                    The name of the file
-        """
-        file_name = model_name
-
-        if fold is not None:
-            file_name += ('_fold-' + str(fold + 1))
-
-        return file_name + '.model'
+            return None
```

## mlrl/testbed/runnables.py

```diff
@@ -1,133 +1,1000 @@
-#!/usr/bin/python
-
 """
 Author: Michael Rapp (michael.rapp.ml@gmail.com)
 
 Provides base classes for programs that can be configured via command line arguments.
 """
 import logging as log
 import sys
+
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser
+from enum import Enum
+from typing import Dict, List, Optional, Set
 
-from mlrl.testbed.data_characteristics import DataCharacteristicsPrinter, DataCharacteristicsLogOutput, \
-    DataCharacteristicsCsvOutput
-from mlrl.testbed.evaluation import ClassificationEvaluation, EvaluationLogOutput, EvaluationCsvOutput
-from mlrl.testbed.experiments import Experiment
-from mlrl.testbed.model_characteristics import RulePrinter, ModelPrinterLogOutput, ModelPrinterTxtOutput, \
-    RuleModelCharacteristicsPrinter, RuleModelCharacteristicsLogOutput, RuleModelCharacteristicsCsvOutput
-from mlrl.testbed.parameters import ParameterCsvInput
+from mlrl.common.config import NONE, Parameter, configure_argument_parser, create_kwargs_from_parameters
+from mlrl.common.cython.validation import assert_greater, assert_greater_or_equal, assert_less, assert_less_or_equal
+from mlrl.common.format import format_dict_keys, format_enum_values
+from mlrl.common.options import BooleanOption, parse_param_and_options
+from mlrl.common.rule_learners import SparsePolicy
+
+from mlrl.testbed.characteristics import OPTION_DISTINCT_LABEL_VECTORS, OPTION_LABEL_CARDINALITY, \
+    OPTION_LABEL_DENSITY, OPTION_LABEL_IMBALANCE_RATIO, OPTION_LABEL_SPARSITY, OPTION_LABELS
+from mlrl.testbed.data_characteristics import OPTION_EXAMPLES, OPTION_FEATURE_DENSITY, OPTION_FEATURE_SPARSITY, \
+    OPTION_FEATURES, OPTION_NOMINAL_FEATURES, OPTION_NUMERICAL_FEATURES, DataCharacteristicsWriter
+from mlrl.testbed.data_splitting import CrossValidationSplitter, DataSet, DataSplitter, NoSplitter, TrainTestSplitter
+from mlrl.testbed.evaluation import OPTION_ACCURACY, OPTION_COVERAGE_ERROR, OPTION_DISCOUNTED_CUMULATIVE_GAIN, \
+    OPTION_ENABLE_ALL, OPTION_EXAMPLE_WISE_F1, OPTION_EXAMPLE_WISE_JACCARD, OPTION_EXAMPLE_WISE_PRECISION, \
+    OPTION_EXAMPLE_WISE_RECALL, OPTION_F1, OPTION_HAMMING_ACCURACY, OPTION_HAMMING_LOSS, OPTION_JACCARD, \
+    OPTION_LABEL_RANKING_AVERAGE_PRECISION, OPTION_MACRO_F1, OPTION_MACRO_JACCARD, OPTION_MACRO_PRECISION, \
+    OPTION_MACRO_RECALL, OPTION_MEAN_ABSOLUTE_ERROR, OPTION_MEAN_ABSOLUTE_PERCENTAGE_ERROR, OPTION_MEAN_SQUARED_ERROR, \
+    OPTION_MEDIAN_ABSOLUTE_ERROR, OPTION_MICRO_F1, OPTION_MICRO_JACCARD, OPTION_MICRO_PRECISION, OPTION_MICRO_RECALL, \
+    OPTION_NORMALIZED_DISCOUNTED_CUMULATIVE_GAIN, OPTION_PRECISION, OPTION_PREDICTION_TIME, OPTION_RANK_LOSS, \
+    OPTION_RECALL, OPTION_SUBSET_ACCURACY, OPTION_SUBSET_ZERO_ONE_LOSS, OPTION_TRAINING_TIME, OPTION_ZERO_ONE_LOSS, \
+    BinaryEvaluationWriter, EvaluationWriter, ProbabilityEvaluationWriter, ScoreEvaluationWriter
+from mlrl.testbed.experiments import Evaluation, Experiment, GlobalEvaluation, IncrementalEvaluation
+from mlrl.testbed.format import OPTION_DECIMALS, OPTION_PERCENTAGE
+from mlrl.testbed.io import clear_directory
+from mlrl.testbed.label_vectors import OPTION_SPARSE, LabelVectorSetWriter, LabelVectorWriter
+from mlrl.testbed.model_characteristics import ModelCharacteristicsWriter, RuleModelCharacteristicsWriter
+from mlrl.testbed.models import OPTION_DECIMALS_BODY, OPTION_DECIMALS_HEAD, OPTION_PRINT_BODIES, \
+    OPTION_PRINT_FEATURE_NAMES, OPTION_PRINT_HEADS, OPTION_PRINT_LABEL_NAMES, OPTION_PRINT_NOMINAL_VALUES, \
+    ModelWriter, RuleModelWriter
+from mlrl.testbed.output_writer import OutputWriter
+from mlrl.testbed.parameters import ParameterCsvInput, ParameterInput, ParameterWriter
 from mlrl.testbed.persistence import ModelPersistence
-from mlrl.testbed.training import DataSet
+from mlrl.testbed.prediction_characteristics import PredictionCharacteristicsWriter
+from mlrl.testbed.prediction_scope import PredictionType
+from mlrl.testbed.predictions import PredictionWriter
+from mlrl.testbed.probability_calibration import JointProbabilityCalibrationModelWriter, \
+    MarginalProbabilityCalibrationModelWriter
 
 LOG_FORMAT = '%(levelname)s %(message)s'
 
 
+class LogLevel(Enum):
+    DEBUG = 'debug'
+    INFO = 'info'
+    WARN = 'warn'
+    WARNING = 'warning'
+    ERROR = 'error'
+    CRITICAL = 'critical'
+    FATAL = 'fatal'
+    NOTSET = 'notset'
+
+    def parse(s):
+        s = s.lower()
+        if s == LogLevel.DEBUG.value:
+            return log.DEBUG
+        elif s == LogLevel.INFO.value:
+            return log.INFO
+        elif s == LogLevel.WARN.value or s == LogLevel.WARNING.value:
+            return log.WARN
+        elif s == LogLevel.ERROR.value:
+            return log.ERROR
+        elif s == LogLevel.CRITICAL.value or s == LogLevel.FATAL.value:
+            return log.CRITICAL
+        elif s == LogLevel.NOTSET.value:
+            return log.NOTSET
+        raise ValueError('Invalid log level given. Must be one of ' + format_enum_values(LogLevel) + ', but is "'
+                         + str(s) + '".')
+
+
 class Runnable(ABC):
     """
     A base class for all programs that can be configured via command line arguments.
     """
 
-    def run(self, parser: ArgumentParser):
+    def __init__(self, description: str):
+        """
+        :param description: A description of the program
+        """
+        self.parser = ArgumentParser(description=description)
+
+    def run(self):
+        parser = self.parser
+        self._configure_arguments(parser)
         args = parser.parse_args()
 
         # Configure the logger...
         log_level = args.log_level
         root = log.getLogger()
         root.setLevel(log_level)
         out_handler = log.StreamHandler(sys.stdout)
         out_handler.setLevel(log_level)
         out_handler.setFormatter(log.Formatter(LOG_FORMAT))
         root.addHandler(out_handler)
 
-        log.info('Configuration: %s', args)
         self._run(args)
 
+    def _configure_arguments(self, parser: ArgumentParser):
+        """
+        May be overridden by subclasses in order to configure the command line arguments of the program.
+
+        :param parser:  An `ArgumentParser` that is used for parsing command line arguments
+        """
+        parser.add_argument('--log-level',
+                            type=LogLevel.parse,
+                            default=LogLevel.INFO.value,
+                            help='The log level to be used. Must be one of ' + format_enum_values(LogLevel) + '.')
+
     @abstractmethod
     def _run(self, args):
         """
         Must be implemented by subclasses in order to run the program.
 
         :param args: The command line arguments
         """
         pass
 
 
-class RuleLearnerRunnable(Runnable, ABC):
+class LearnerRunnable(Runnable, ABC):
     """
-    A base class for all programs that perform an experiment that involves training and evaluation of a rule learner.
+    A base class for all programs that perform an experiment that involves training and evaluation of a learner.
     """
 
-    def _run(self, args):
-        parameter_input = None if args.parameter_dir is None else ParameterCsvInput(input_dir=args.parameter_dir)
-        evaluation_outputs = []
-        data_characteristics_printer_outputs = []
-        model_characteristics_printer_outputs = []
-        model_printer_outputs = []
-        output_dir = args.output_dir
+    class ClearOutputDirHook(Experiment.ExecutionHook):
+        """
+        Deletes all files from the output directory before an experiment starts.
+        """
 
-        if args.print_data_characteristics:
-            data_characteristics_printer_outputs.append(DataCharacteristicsLogOutput())
+        def __init__(self, output_dir: str):
+            self.output_dir = output_dir
 
-        if args.print_evaluation:
-            evaluation_outputs.append(EvaluationLogOutput())
+        def execute(self):
+            clear_directory(self.output_dir)
 
-        if args.print_model_characteristics:
-            model_characteristics_printer_outputs.append(RuleModelCharacteristicsLogOutput())
+    PARAM_DATA_SPLIT = '--data-split'
+
+    DATA_SPLIT_TRAIN_TEST = 'train-test'
+
+    OPTION_TEST_SIZE = 'test_size'
+
+    DATA_SPLIT_CROSS_VALIDATION = 'cross-validation'
+
+    OPTION_NUM_FOLDS = 'num_folds'
+
+    OPTION_CURRENT_FOLD = 'current_fold'
+
+    DATA_SPLIT_VALUES: Dict[str, Set[str]] = {
+        NONE: {},
+        DATA_SPLIT_TRAIN_TEST: {OPTION_TEST_SIZE},
+        DATA_SPLIT_CROSS_VALIDATION: {OPTION_NUM_FOLDS, OPTION_CURRENT_FOLD}
+    }
+
+    PARAM_PRINT_EVALUATION = '--print-evaluation'
+
+    PRINT_EVALUATION_VALUES: Dict[str, Set[str]] = {
+        BooleanOption.TRUE.value: {
+            OPTION_ENABLE_ALL, OPTION_HAMMING_LOSS, OPTION_HAMMING_ACCURACY, OPTION_SUBSET_ZERO_ONE_LOSS,
+            OPTION_SUBSET_ACCURACY, OPTION_MICRO_PRECISION, OPTION_MICRO_RECALL, OPTION_MICRO_F1, OPTION_MICRO_JACCARD,
+            OPTION_MACRO_PRECISION, OPTION_MACRO_RECALL, OPTION_MACRO_F1, OPTION_MACRO_JACCARD,
+            OPTION_EXAMPLE_WISE_PRECISION, OPTION_EXAMPLE_WISE_RECALL, OPTION_EXAMPLE_WISE_F1,
+            OPTION_EXAMPLE_WISE_JACCARD, OPTION_ACCURACY, OPTION_ZERO_ONE_LOSS, OPTION_PRECISION, OPTION_RECALL,
+            OPTION_F1, OPTION_JACCARD, OPTION_MEAN_ABSOLUTE_ERROR, OPTION_MEAN_SQUARED_ERROR,
+            OPTION_MEDIAN_ABSOLUTE_ERROR, OPTION_MEAN_ABSOLUTE_PERCENTAGE_ERROR, OPTION_RANK_LOSS,
+            OPTION_COVERAGE_ERROR, OPTION_LABEL_RANKING_AVERAGE_PRECISION, OPTION_DISCOUNTED_CUMULATIVE_GAIN,
+            OPTION_NORMALIZED_DISCOUNTED_CUMULATIVE_GAIN, OPTION_DECIMALS, OPTION_PERCENTAGE
+        },
+        BooleanOption.FALSE.value: {}
+    }
+
+    PARAM_STORE_EVALUATION = '--store-evaluation'
+
+    STORE_EVALUATION_VALUES: Dict[str, Set[str]] = {
+        BooleanOption.TRUE.value: {
+            OPTION_ENABLE_ALL, OPTION_HAMMING_LOSS, OPTION_HAMMING_ACCURACY, OPTION_SUBSET_ZERO_ONE_LOSS,
+            OPTION_SUBSET_ACCURACY, OPTION_MICRO_PRECISION, OPTION_MICRO_RECALL, OPTION_MICRO_F1, OPTION_MICRO_JACCARD,
+            OPTION_MACRO_PRECISION, OPTION_MACRO_RECALL, OPTION_MACRO_F1, OPTION_MACRO_JACCARD,
+            OPTION_EXAMPLE_WISE_PRECISION, OPTION_EXAMPLE_WISE_RECALL, OPTION_EXAMPLE_WISE_F1,
+            OPTION_EXAMPLE_WISE_JACCARD, OPTION_ACCURACY, OPTION_ZERO_ONE_LOSS, OPTION_PRECISION, OPTION_RECALL,
+            OPTION_F1, OPTION_JACCARD, OPTION_MEAN_ABSOLUTE_ERROR, OPTION_MEAN_SQUARED_ERROR,
+            OPTION_MEDIAN_ABSOLUTE_ERROR, OPTION_MEAN_ABSOLUTE_PERCENTAGE_ERROR, OPTION_RANK_LOSS,
+            OPTION_COVERAGE_ERROR, OPTION_LABEL_RANKING_AVERAGE_PRECISION, OPTION_DISCOUNTED_CUMULATIVE_GAIN,
+            OPTION_NORMALIZED_DISCOUNTED_CUMULATIVE_GAIN, OPTION_TRAINING_TIME, OPTION_PREDICTION_TIME, OPTION_DECIMALS,
+            OPTION_PERCENTAGE
+        },
+        BooleanOption.FALSE.value: {}
+    }
+
+    PARAM_PRINT_PREDICTIONS = '--print-predictions'
+
+    PRINT_PREDICTIONS_VALUES: Dict[str, Set[str]] = {
+        BooleanOption.TRUE.value: {OPTION_DECIMALS},
+        BooleanOption.FALSE.value: {}
+    }
 
-        if args.print_rules:
-            model_printer_outputs.append(ModelPrinterLogOutput())
+    PARAM_STORE_PREDICTIONS = '--store-predictions'
 
-        if output_dir is not None:
-            clear_dir = args.current_fold == -1
+    STORE_PREDICTIONS_VALUES = PRINT_PREDICTIONS_VALUES
 
-            if args.store_data_characteristics:
-                data_characteristics_printer_outputs.append(
-                    DataCharacteristicsCsvOutput(output_dir=output_dir, clear_dir=clear_dir))
-                clear_dir = False
-
-            if args.store_evaluation:
-                evaluation_outputs.append(
-                    EvaluationCsvOutput(output_dir=output_dir, output_predictions=args.store_predictions,
-                                        clear_dir=clear_dir))
-                clear_dir = False
-
-            if args.store_model_characteristics:
-                model_characteristics_printer_outputs.append(RuleModelCharacteristicsCsvOutput(output_dir=output_dir,
-                                                                                               clear_dir=clear_dir))
-                clear_dir = False
-
-            if args.store_rules:
-                model_printer_outputs.append(ModelPrinterTxtOutput(output_dir=output_dir, clear_dir=clear_dir))
-
-        model_dir = args.model_dir
-        persistence = None if model_dir is None else ModelPersistence(model_dir)
-        learner = self._create_learner(args)
-
-        data_characteristics_printer = DataCharacteristicsPrinter(data_characteristics_printer_outputs) if len(
-            data_characteristics_printer_outputs) > 0 else None
-        model_printer = RulePrinter(args.print_options, model_printer_outputs) if len(
-            model_printer_outputs) > 0 else None
-        model_characteristics_printer = RuleModelCharacteristicsPrinter(model_characteristics_printer_outputs) if len(
-            model_characteristics_printer_outputs) > 0 else None
-        train_evaluation = ClassificationEvaluation(*evaluation_outputs) if args.evaluate_training_data else None
-        test_evaluation = ClassificationEvaluation(*evaluation_outputs)
-        data_set = DataSet(data_dir=args.data_dir, data_set_name=args.dataset,
+    PARAM_PRINT_PREDICTION_CHARACTERISTICS = '--print-prediction-characteristics'
+
+    PRINT_PREDICTION_CHARACTERISTICS_VALUES: Dict[str, Set[str]] = {
+        BooleanOption.TRUE.value: {
+            OPTION_LABELS, OPTION_LABEL_DENSITY, OPTION_LABEL_SPARSITY, OPTION_LABEL_IMBALANCE_RATIO,
+            OPTION_LABEL_CARDINALITY, OPTION_DISTINCT_LABEL_VECTORS, OPTION_DECIMALS, OPTION_PERCENTAGE
+        },
+        BooleanOption.FALSE.value: {}
+    }
+
+    PARAM_STORE_PREDICTION_CHARACTERISTICS = '--store-prediction-characteristics'
+
+    STORE_PREDICTION_CHARACTERISTICS_VALUES = PRINT_PREDICTION_CHARACTERISTICS_VALUES
+
+    PARAM_PRINT_DATA_CHARACTERISTICS = '--print-data-characteristics'
+
+    PRINT_DATA_CHARACTERISTICS_VALUES: Dict[str, Set[str]] = {
+        BooleanOption.TRUE.value: {
+            OPTION_EXAMPLES, OPTION_FEATURES, OPTION_NUMERICAL_FEATURES, OPTION_NOMINAL_FEATURES,
+            OPTION_FEATURE_DENSITY, OPTION_FEATURE_SPARSITY, OPTION_LABELS, OPTION_LABEL_DENSITY, OPTION_LABEL_SPARSITY,
+            OPTION_LABEL_IMBALANCE_RATIO, OPTION_LABEL_CARDINALITY, OPTION_DISTINCT_LABEL_VECTORS, OPTION_DECIMALS,
+            OPTION_PERCENTAGE
+        },
+        BooleanOption.FALSE.value: {}
+    }
+
+    PARAM_STORE_DATA_CHARACTERISTICS = '--store-data-characteristics'
+
+    STORE_DATA_CHARACTERISTICS_VALUES = PRINT_DATA_CHARACTERISTICS_VALUES
+
+    PARAM_PRINT_LABEL_VECTORS = '--print-label-vectors'
+
+    PRINT_LABEL_VECTORS_VALUES: Dict[str, Set[str]] = {
+        BooleanOption.TRUE.value: {OPTION_SPARSE},
+        BooleanOption.FALSE.value: {}
+    }
+
+    PARAM_STORE_LABEL_VECTORS = '--store-label-vectors'
+
+    STORE_LABEL_VECTORS_VALUES = PRINT_LABEL_VECTORS_VALUES
+
+    PARAM_OUTPUT_DIR = '--output-dir'
+
+    PARAM_PREDICTION_TYPE = '--prediction-type'
+
+    def __init__(self, description: str, learner_name: str):
+        """
+        :param learner_name: The name of the learner
+        """
+        super().__init__(description)
+        self.learner_name = learner_name
+
+    def __create_prediction_type(self, args) -> PredictionType:
+        prediction_type = args.prediction_type
+
+        try:
+            return PredictionType(prediction_type)
+        except ValueError:
+            raise ValueError('Invalid value given for parameter "' + self.PARAM_PREDICTION_TYPE + '": Must be one of '
+                             + format_enum_values(PredictionType) + ', but is "' + str(prediction_type) + '"')
+
+    def __create_data_splitter(self, args) -> DataSplitter:
+        data_set = DataSet(data_dir=args.data_dir,
+                           data_set_name=args.dataset,
                            use_one_hot_encoding=args.one_hot_encoding)
-        experiment = Experiment(learner, test_evaluation=test_evaluation, train_evaluation=train_evaluation,
-                                data_set=data_set, num_folds=args.folds, current_fold=args.current_fold,
-                                parameter_input=parameter_input, model_printer=model_printer,
-                                model_characteristics_printer=model_characteristics_printer,
-                                data_characteristics_printer=data_characteristics_printer, persistence=persistence)
-        experiment.random_state = args.random_state
+        value, options = parse_param_and_options(self.PARAM_DATA_SPLIT, args.data_split, self.DATA_SPLIT_VALUES)
+
+        if value == self.DATA_SPLIT_CROSS_VALIDATION:
+            num_folds = options.get_int(self.OPTION_NUM_FOLDS, 10)
+            assert_greater_or_equal(self.OPTION_NUM_FOLDS, num_folds, 2)
+            current_fold = options.get_int(self.OPTION_CURRENT_FOLD, 0)
+            if current_fold != 0:
+                assert_greater_or_equal(self.OPTION_CURRENT_FOLD, current_fold, 1)
+                assert_less_or_equal(self.OPTION_CURRENT_FOLD, current_fold, num_folds)
+            return CrossValidationSplitter(data_set,
+                                           num_folds=num_folds,
+                                           current_fold=current_fold - 1,
+                                           random_state=args.random_state)
+        elif value == self.DATA_SPLIT_TRAIN_TEST:
+            test_size = options.get_float(self.OPTION_TEST_SIZE, 0.33)
+            assert_greater(self.OPTION_TEST_SIZE, test_size, 0)
+            assert_less(self.OPTION_TEST_SIZE, test_size, 1)
+            return TrainTestSplitter(data_set, test_size=test_size, random_state=args.random_state)
+        else:
+            return NoSplitter(data_set)
+
+    @staticmethod
+    def __create_pre_execution_hook(args, data_splitter: DataSplitter) -> Optional[Experiment.ExecutionHook]:
+        current_fold = data_splitter.current_fold if isinstance(data_splitter, CrossValidationSplitter) else -1
+        return None if args.output_dir is None or current_fold >= 0 else LearnerRunnable.ClearOutputDirHook(
+            output_dir=args.output_dir)
+
+    def _configure_arguments(self, parser: ArgumentParser):
+        super()._configure_arguments(parser)
+        parser.add_argument('--random-state',
+                            type=int,
+                            default=1,
+                            help='The seed to be used by random number generators. Must be at least 1.')
+        parser.add_argument('--data-dir',
+                            type=str,
+                            required=True,
+                            help='The path of the directory where the data set files are located.')
+        parser.add_argument('--dataset', type=str, required=True, help='The name of the data set files without suffix.')
+        parser.add_argument(self.PARAM_DATA_SPLIT,
+                            type=str,
+                            default=self.DATA_SPLIT_TRAIN_TEST,
+                            help='The strategy to be used for splitting the available data into training and test '
+                            + 'sets. Must be one of ' + format_dict_keys(self.DATA_SPLIT_VALUES) + '. For additional '
+                            + 'options refer to the documentation.')
+        parser.add_argument(self.PARAM_PRINT_EVALUATION,
+                            type=str,
+                            default=BooleanOption.TRUE.value,
+                            help='Whether the evaluation results should be printed on the console or not. Must be one '
+                            + 'of ' + format_dict_keys(self.PRINT_EVALUATION_VALUES) + '. For additional options refer '
+                            + 'to the documentation.')
+        parser.add_argument(self.PARAM_STORE_EVALUATION,
+                            type=str,
+                            default=BooleanOption.TRUE.value,
+                            help='Whether the evaluation results should be written into output files or not. Must be '
+                            + 'one of ' + format_dict_keys(self.STORE_EVALUATION_VALUES) + '. Does only have an effect '
+                            + 'if the parameter ' + self.PARAM_OUTPUT_DIR + ' is specified. For additional options '
+                            + 'refer to the documentation.')
+        parser.add_argument('--evaluate-training-data',
+                            type=BooleanOption.parse,
+                            default=False,
+                            help='Whether the models should not only be evaluated on the test data, but also on the '
+                            + 'training data. Must be one of ' + format_enum_values(BooleanOption) + '.')
+        parser.add_argument(self.PARAM_PRINT_PREDICTION_CHARACTERISTICS,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the characteristics of binary predictions should be printed on the console '
+                            + 'or not. Must be one of ' + format_dict_keys(self.PRINT_PREDICTION_CHARACTERISTICS_VALUES)
+                            + '. Does only have an effect if the parameter ' + self.PARAM_PREDICTION_TYPE + ' is set '
+                            + 'to ' + PredictionType.BINARY.value + '. For additional options refer to the '
+                            + 'documentation.')
+        parser.add_argument(self.PARAM_STORE_PREDICTION_CHARACTERISTICS,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the characteristics of binary predictions should be written into output '
+                            + 'files or not. Must be one of '
+                            + format_dict_keys(self.STORE_PREDICTION_CHARACTERISTICS_VALUES) + '. Does only have an '
+                            + 'effect if the parameter ' + self.PARAM_PREDICTION_TYPE + ' is set to '
+                            + PredictionType.BINARY.value + '. For additional options refer to the documentation.')
+        parser.add_argument(self.PARAM_PRINT_DATA_CHARACTERISTICS,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the characteristics of the training data should be printed on the console or '
+                            + 'not. Must be one of ' + format_dict_keys(self.PRINT_DATA_CHARACTERISTICS_VALUES) + '. '
+                            + 'For additional options refer to the documentation.')
+        parser.add_argument(self.PARAM_STORE_DATA_CHARACTERISTICS,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the characteristics of the training data should be written into output files '
+                            + 'or not. Must be one of ' + format_dict_keys(self.STORE_DATA_CHARACTERISTICS_VALUES)
+                            + '. Does only have an effect if the parameter ' + self.PARAM_OUTPUT_DIR + ' is specified. '
+                            + 'For additional options refer to the documentation.')
+        parser.add_argument(self.PARAM_PRINT_LABEL_VECTORS,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the unique label vectors contained in the training data should be printed on '
+                            + 'the console or not. Must be one of ' + format_dict_keys(self.PRINT_LABEL_VECTORS_VALUES)
+                            + '. For additional options refer to the documentation.')
+        parser.add_argument(self.PARAM_STORE_LABEL_VECTORS,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the unique label vectors contained in the training data should be written '
+                            + 'into output files or not. Must be one of '
+                            + format_dict_keys(self.STORE_LABEL_VECTORS_VALUES) + '. Does only have an effect if the '
+                            + 'parameter ' + self.PARAM_OUTPUT_DIR + ' is specified. For additional options refer to '
+                            + 'the documentation.')
+        parser.add_argument('--one-hot-encoding',
+                            type=BooleanOption.parse,
+                            default=False,
+                            help='Whether one-hot-encoding should be used to encode nominal attributes or not. Must be '
+                            + 'one of ' + format_enum_values(BooleanOption) + '.')
+        parser.add_argument('--model-dir', type=str, help='The path of the directory where models should be stored.')
+        parser.add_argument('--parameter-dir',
+                            type=str,
+                            help='The path of the directory where configuration files, which specify the parameters to '
+                            + 'be used by the algorithm, are located.')
+        parser.add_argument(self.PARAM_OUTPUT_DIR,
+                            type=str,
+                            help='The path of the directory where experimental results should be saved.')
+        parser.add_argument('--print-parameters',
+                            type=BooleanOption.parse,
+                            default=False,
+                            help='Whether the parameter setting should be printed on the console or not. Must be one '
+                            + 'of ' + format_enum_values(BooleanOption) + '.')
+        parser.add_argument('--store-parameters',
+                            type=BooleanOption.parse,
+                            default=False,
+                            help='Whether the parameter setting should be written into output files or not. Must be '
+                            + 'one of ' + format_enum_values(BooleanOption) + '. Does only have an effect, if the '
+                            + 'parameter ' + self.PARAM_OUTPUT_DIR + ' is specified.')
+        parser.add_argument(self.PARAM_PRINT_PREDICTIONS,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the predictions for individual examples and labels should be printed on the '
+                            + 'console or not. Must be one of ' + format_dict_keys(self.PRINT_PREDICTIONS_VALUES) + '. '
+                            + 'For additional options refer to the documentation.')
+        parser.add_argument(self.PARAM_STORE_PREDICTIONS,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the predictions for individual examples and labels should be written into '
+                            + 'output files or not. Must be one of ' + format_dict_keys(self.STORE_PREDICTIONS_VALUES)
+                            + '. Does only have an effect, if the parameter ' + self.PARAM_OUTPUT_DIR + ' is '
+                            + 'specified. For additional options refer to the documentation.')
+        parser.add_argument(self.PARAM_PREDICTION_TYPE,
+                            type=str,
+                            default=PredictionType.BINARY.value,
+                            help='The type of predictions that should be obtained from the learner. Must be one of '
+                            + format_enum_values(PredictionType) + '.')
+
+    def _run(self, args):
+        prediction_type = self.__create_prediction_type(args)
+        train_evaluation = self._create_evaluation(
+            args, prediction_type,
+            self._create_evaluation_output_writers(args, prediction_type) if args.evaluate_training_data else [])
+        test_evaluation = self._create_evaluation(args, prediction_type,
+                                                  self._create_evaluation_output_writers(args, prediction_type))
+        data_splitter = self.__create_data_splitter(args)
+        experiment = Experiment(base_learner=self._create_learner(args),
+                                learner_name=self.learner_name,
+                                data_splitter=data_splitter,
+                                pre_training_output_writers=self._create_pre_training_output_writers(args),
+                                post_training_output_writers=self._create_post_training_output_writers(args),
+                                pre_execution_hook=self.__create_pre_execution_hook(args, data_splitter),
+                                train_evaluation=train_evaluation,
+                                test_evaluation=test_evaluation,
+                                parameter_input=self._create_parameter_input(args),
+                                persistence=self._create_persistence(args))
         experiment.run()
 
+    def _create_pre_training_output_writers(self, args) -> List[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter`s that should be invoked before training a
+        model.
+
+        :param args:    The command line arguments
+        :return:        A list that contains the `OutputWriter`s that have been created
+        """
+        output_writers = []
+        output_writer = self._create_data_characteristics_writer(args)
+
+        if output_writer is not None:
+            output_writers.append(output_writer)
+
+        output_writer = self._create_parameter_writer(args)
+
+        if output_writer is not None:
+            output_writers.append(output_writer)
+
+        return output_writers
+
+    def _create_post_training_output_writers(self, args) -> List[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter`s that should be invoked after training a
+        model.
+
+        :param args:    The command line arguments
+        :return:        A list that contains the `OutputWriters`s that have been created
+        """
+        output_writers = []
+        output_writer = self._create_label_vector_writer(args)
+
+        if output_writer is not None:
+            output_writers.append(output_writer)
+
+        return output_writers
+
+    def _create_evaluation_output_writers(self, args, prediction_type: PredictionType) -> List[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter`s that should be invoked after evaluating a
+        model.
+
+        :param args:            The command line arguments
+        :param prediction_type: The type of the predictions
+        :return:                A list that contains the `OutputWriter`s that have been created
+        """
+        output_writers = []
+        output_writer = self._create_evaluation_writer(args, prediction_type)
+
+        if output_writer is not None:
+            output_writers.append(output_writer)
+
+        output_writer = self._create_prediction_writer(args)
+
+        if output_writer is not None:
+            output_writers.append(output_writer)
+
+        output_writer = self._create_prediction_characteristics_writer(args)
+
+        if output_writer is not None:
+            output_writers.append(output_writer)
+
+        return output_writers
+
+    def _create_persistence(self, args) -> Optional[ModelPersistence]:
+        """
+        May be overridden by subclasses in order to create the `ModelPersistence` that should be used to save and load
+        models.
+
+        :param args:    The command line arguments
+        :return:        The `ModelPersistence` that has been created
+        """
+        return None if args.model_dir is None else ModelPersistence(model_dir=args.model_dir)
+
+    def _create_evaluation(self, args, prediction_type: PredictionType,
+                           output_writers: List[OutputWriter]) -> Optional[Evaluation]:
+        """
+        May be overridden by subclasses in order to create the `Evaluation` that should be used to evaluate predictions
+        that are obtained from a previously trained model.
+
+        :param args:            The command line arguments
+        :param prediction_type: The type of the predictions to be obtained
+        :param output_writers:  A list that contains all output writers to be invoked after predictions have been
+                                obtained
+        :return:                The `Evaluation` that has been created
+        """
+        return GlobalEvaluation(prediction_type, output_writers) if len(output_writers) > 0 else None
+
+    def _create_evaluation_writer(self, args, prediction_type: PredictionType) -> Optional[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter` that should be used to output evaluation
+        results.
+
+        :param args:            The command line arguments
+        :param prediction_type: The type of the predictions
+        :return:                The `OutputWriter` that has been created
+        """
+        sinks = []
+        value, options = parse_param_and_options(self.PARAM_PRINT_EVALUATION, args.print_evaluation,
+                                                 self.PRINT_EVALUATION_VALUES)
+
+        if value == BooleanOption.TRUE.value:
+            sinks.append(EvaluationWriter.LogSink(options=options))
+
+        value, options = parse_param_and_options(self.PARAM_STORE_EVALUATION, args.store_evaluation,
+                                                 self.STORE_EVALUATION_VALUES)
+
+        if value == BooleanOption.TRUE.value and args.output_dir is not None:
+            sinks.append(EvaluationWriter.CsvSink(output_dir=args.output_dir, options=options))
+
+        if len(sinks) == 0:
+            return None
+        elif prediction_type == PredictionType.SCORES:
+            return ScoreEvaluationWriter(sinks)
+        elif prediction_type == PredictionType.PROBABILITIES:
+            return ProbabilityEvaluationWriter(sinks)
+        else:
+            return BinaryEvaluationWriter(sinks)
+
+    def _create_parameter_input(self, args) -> Optional[ParameterInput]:
+        """
+        May be overridden by subclasses in order to create the `ParameterInput` that should be used to load parameter
+        settings.
+
+        :param args:    The command line arguments
+        :return:        The `ParameterInput` that has been created
+        """
+        return None if args.parameter_dir is None else ParameterCsvInput(input_dir=args.parameter_dir)
+
+    def _create_parameter_writer(self, args) -> Optional[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter` that should be used to output parameter
+        settings.
+
+        :param args:    The command line arguments
+        :return:        The `OutputWriter` that has been created
+        """
+        sinks = []
+
+        if args.print_parameters:
+            sinks.append(ParameterWriter.LogSink())
+
+        if args.store_parameters and args.output_dir is not None:
+            sinks.append(ParameterWriter.CsvSink(output_dir=args.output_dir))
+
+        return ParameterWriter(sinks) if len(sinks) > 0 else None
+
+    def _create_prediction_writer(self, args) -> Optional[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter` that should be used to output predictions.
+
+        :param args:    The command line arguments
+        :return:        The `OutputWriter` that has been created
+        """
+        sinks = []
+        value, options = parse_param_and_options(self.PARAM_PRINT_PREDICTIONS, args.print_predictions,
+                                                 self.PRINT_PREDICTIONS_VALUES)
+
+        if value == BooleanOption.TRUE.value:
+            sinks.append(PredictionWriter.LogSink(options=options))
+
+        value, options = parse_param_and_options(self.PARAM_STORE_PREDICTIONS, args.store_predictions,
+                                                 self.STORE_PREDICTIONS_VALUES)
+
+        if value == BooleanOption.TRUE.value and args.output_dir is not None:
+            sinks.append(PredictionWriter.ArffSink(output_dir=args.output_dir, options=options))
+
+        return PredictionWriter(sinks) if len(sinks) > 0 else None
+
+    def _create_prediction_characteristics_writer(self, args) -> Optional[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter` that should be used to output prediction
+        characteristics.
+
+        :param args:    The command line arguments
+        :return:        The `OutputWriter` that has been created
+        """
+        sinks = []
+        value, options = parse_param_and_options(self.PARAM_PRINT_PREDICTION_CHARACTERISTICS,
+                                                 args.print_prediction_characteristics,
+                                                 self.PRINT_PREDICTION_CHARACTERISTICS_VALUES)
+
+        if value == BooleanOption.TRUE.value:
+            sinks.append(PredictionCharacteristicsWriter.LogSink(options=options))
+
+        value, options = parse_param_and_options(self.PARAM_STORE_PREDICTION_CHARACTERISTICS,
+                                                 args.store_prediction_characteristics,
+                                                 self.STORE_PREDICTION_CHARACTERISTICS_VALUES)
+
+        if value == BooleanOption.TRUE.value and args.output_dir is not None:
+            sinks.append(PredictionCharacteristicsWriter.CsvSink(output_dir=args.output_dir, options=options))
+
+        return PredictionCharacteristicsWriter(sinks) if len(sinks) > 0 else None
+
+    def _create_data_characteristics_writer(self, args) -> Optional[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter` that should be used to output data
+        characteristics.
+
+        :param args:    The command line arguments
+        :return:        The `OutputWriter` that has been created
+        """
+        sinks = []
+        value, options = parse_param_and_options(self.PARAM_PRINT_DATA_CHARACTERISTICS, args.print_data_characteristics,
+                                                 self.PRINT_DATA_CHARACTERISTICS_VALUES)
+
+        if value == BooleanOption.TRUE.value:
+            sinks.append(DataCharacteristicsWriter.LogSink(options=options))
+
+        value, options = parse_param_and_options(self.PARAM_STORE_DATA_CHARACTERISTICS, args.store_data_characteristics,
+                                                 self.STORE_DATA_CHARACTERISTICS_VALUES)
+
+        if value == BooleanOption.TRUE.value and args.output_dir is not None:
+            sinks.append(DataCharacteristicsWriter.CsvSink(output_dir=args.output_dir, options=options))
+
+        return DataCharacteristicsWriter(sinks) if len(sinks) > 0 else None
+
+    def _create_label_vector_writer(self, args) -> Optional[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter` that should be used to output unique label
+        vectors contained in the training data.
+
+        :param args:    The command line arguments
+        :return:        The `OutputWriter` that has been created
+        """
+        sinks = []
+        value, options = parse_param_and_options(self.PARAM_PRINT_LABEL_VECTORS, args.print_label_vectors,
+                                                 self.PRINT_LABEL_VECTORS_VALUES)
+
+        if value == BooleanOption.TRUE.value:
+            sinks.append(LabelVectorWriter.LogSink(options=options))
+
+        value, options = parse_param_and_options(self.PARAM_STORE_LABEL_VECTORS, args.store_label_vectors,
+                                                 self.STORE_LABEL_VECTORS_VALUES)
+
+        if value == BooleanOption.TRUE.value and args.output_dir is not None:
+            sinks.append(LabelVectorWriter.CsvSink(output_dir=args.output_dir, options=options))
+
+        return LabelVectorWriter(sinks) if len(sinks) > 0 else None
+
     @abstractmethod
     def _create_learner(self, args):
         """
         Must be implemented by subclasses in order to create the learner.
 
         :param args:    The command line arguments
         :return:        The learner that has been created
         """
         pass
+
+
+class RuleLearnerRunnable(LearnerRunnable):
+    """
+    A base class for all programs that perform an experiment that involves training and evaluation of a rule learner.
+    """
+
+    PARAM_INCREMENTAL_EVALUATION = '--incremental-evaluation'
+
+    OPTION_MIN_SIZE = 'min_size'
+
+    OPTION_MAX_SIZE = 'max_size'
+
+    OPTION_STEP_SIZE = 'step_size'
+
+    INCREMENTAL_EVALUATION_VALUES: Dict[str, Set[str]] = {
+        BooleanOption.TRUE.value: {OPTION_MIN_SIZE, OPTION_MAX_SIZE, OPTION_STEP_SIZE},
+        BooleanOption.FALSE.value: {}
+    }
+
+    PARAM_PRINT_RULES = '--print-rules'
+
+    PRINT_RULES_VALUES: Dict[str, Set[str]] = {
+        BooleanOption.TRUE.value: {
+            OPTION_PRINT_FEATURE_NAMES, OPTION_PRINT_LABEL_NAMES, OPTION_PRINT_NOMINAL_VALUES, OPTION_PRINT_BODIES,
+            OPTION_PRINT_HEADS, OPTION_DECIMALS_BODY, OPTION_DECIMALS_HEAD
+        },
+        BooleanOption.FALSE.value: {}
+    }
+
+    PARAM_STORE_RULES = '--store-rules'
+
+    STORE_RULES_VALUES = PRINT_RULES_VALUES
+
+    PARAM_PRINT_MARGINAL_PROBABILITY_CALIBRATION_MODEL = '--print-marginal-probability-calibration-model'
+
+    PRINT_MARGINAL_PROBABILITY_CALIBRATION_MODEL_VALUES: Dict[str, Set[str]] = {
+        BooleanOption.TRUE.value: {OPTION_DECIMALS},
+        BooleanOption.FALSE.value: {}
+    }
+
+    PARAM_STORE_MARGINAL_PROBABILITY_CALIBRATION_MODEL = '--store-marginal-probability-calibration-model'
+
+    STORE_MARGINAL_PROBABILITY_CALIBRATION_MODEL_VALUES = PRINT_MARGINAL_PROBABILITY_CALIBRATION_MODEL_VALUES
+
+    PARAM_PRINT_JOINT_PROBABILITY_CALIBRATION_MODEL = '--print-joint-probability-calibration-model'
+
+    PRINT_JOINT_PROBABILITY_CALIBRATION_MODEL_VALUES: Dict[str, Set[str]] = {
+        BooleanOption.TRUE.value: {OPTION_DECIMALS},
+        BooleanOption.FALSE.value: {}
+    }
+
+    PARAM_STORE_JOINT_PROBABILITY_CALIBRATION_MODEL = '--store-joint-probability-calibration-model'
+
+    STORE_JOINT_PROBABILITY_CALIBRATION_MODEL_VALUES = PRINT_JOINT_PROBABILITY_CALIBRATION_MODEL_VALUES
+
+    def __init__(self, description: str, learner_name: str, learner_type: type, config_type: type,
+                 parameters: Set[Parameter]):
+        """
+        :param learner_type:    The type of the rule learner
+        :param config_type:     The type of the rule learner's configuration
+        :param parameters:      A set that contains the parameters that may be supported by the rule learner
+        """
+        super().__init__(description=description, learner_name=learner_name)
+        self.learner_type = learner_type
+        self.config_type = config_type
+        self.parameters = parameters
+
+    def _configure_arguments(self, parser: ArgumentParser):
+        super()._configure_arguments(parser)
+        parser.add_argument(self.PARAM_INCREMENTAL_EVALUATION,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether models should be evaluated repeatedly, using only a subset of the induced '
+                            + 'rules with increasing size, or not. Must be one of ' + format_enum_values(BooleanOption)
+                            + '. For additional options refer to the documentation.')
+        parser.add_argument('--print-model-characteristics',
+                            type=BooleanOption.parse,
+                            default=False,
+                            help='Whether the characteristics of models should be printed on the console or not. Must '
+                            + 'be one of ' + format_enum_values(BooleanOption) + '.')
+        parser.add_argument('--store-model-characteristics',
+                            type=BooleanOption.parse,
+                            default=False,
+                            help='Whether the characteristics of models should be written into output files or not. '
+                            + 'Must be one of ' + format_enum_values(BooleanOption) + '. Does only have an effect if '
+                            + 'the parameter ' + self.PARAM_OUTPUT_DIR + ' is specified.')
+        parser.add_argument(self.PARAM_PRINT_RULES,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the induced rules should be printed on the console or not. Must be one of '
+                            + format_dict_keys(self.PRINT_RULES_VALUES) + '. For additional options refer to the '
+                            + 'documentation.')
+        parser.add_argument(self.PARAM_STORE_RULES,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the induced rules should be written into a text file or not. Must be one of '
+                            + format_dict_keys(self.STORE_RULES_VALUES) + '. Does only have an effect if the parameter '
+                            + self.PARAM_OUTPUT_DIR + ' is specified. For additional options refer to the '
+                            + 'documentation.')
+        parser.add_argument(self.PARAM_PRINT_MARGINAL_PROBABILITY_CALIBRATION_MODEL,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the model for the calibration of marginal probabilities should be printed on '
+                            + 'the console or not. Must be one of ' + format_enum_values(BooleanOption) + '. For '
+                            + 'additional options refer to the documentation.')
+        parser.add_argument(self.PARAM_STORE_MARGINAL_PROBABILITY_CALIBRATION_MODEL,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the model for the calibration of marginal probabilities should be written '
+                            + 'into an output file or not. Must be one of ' + format_enum_values(BooleanOption) + '. '
+                            + 'Does only have an effect if the parameter ' + self.PARAM_OUTPUT_DIR + ' is specified. '
+                            + 'For additional options refer to the documentation.')
+        parser.add_argument(self.PARAM_PRINT_JOINT_PROBABILITY_CALIBRATION_MODEL,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the model for the calibration of joint probabilities should be printed on '
+                            + 'the console or not. Must be one of ' + format_enum_values(BooleanOption) + '. For '
+                            + 'additional options refer to the documentation.')
+        parser.add_argument(self.PARAM_STORE_JOINT_PROBABILITY_CALIBRATION_MODEL,
+                            type=str,
+                            default=BooleanOption.FALSE.value,
+                            help='Whether the model for the calibration of joint probabilities should be written into '
+                            + 'an output file or not. Must be one of ' + format_enum_values(BooleanOption) + '. Does '
+                            + 'only have an effect if the parameter ' + self.PARAM_OUTPUT_DIR + ' is specified. For '
+                            + 'additional options refer to the documentation.')
+        parser.add_argument('--feature-format',
+                            type=str,
+                            default=SparsePolicy.AUTO.value,
+                            help='The format to be used for the representation of the feature matrix. Must be one of '
+                            + format_enum_values(SparsePolicy) + '.')
+        parser.add_argument('--label-format',
+                            type=str,
+                            default=SparsePolicy.AUTO.value,
+                            help='The format to be used for the representation of the label matrix. Must be one of '
+                            + format_enum_values(SparsePolicy) + '.')
+        parser.add_argument('--prediction-format',
+                            type=str,
+                            default=SparsePolicy.AUTO.value,
+                            help='The format to be used for the representation of predictions. Must be one of '
+                            + format_enum_values(SparsePolicy) + '.')
+        configure_argument_parser(parser, self.config_type, self.parameters)
+
+    def _create_learner(self, args):
+        kwargs = create_kwargs_from_parameters(args, self.parameters)
+        kwargs['random_state'] = args.random_state
+        kwargs['feature_format'] = args.feature_format
+        kwargs['label_format'] = args.label_format
+        kwargs['prediction_format'] = args.prediction_format
+        return self.learner_type(**kwargs)
+
+    def _create_model_writer(self, args) -> Optional[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter` that should be used to output textual
+        representations of models.
+
+        :param args:    The command line arguments
+        :return:        The `OutputWriter` that has been created
+        """
+        sinks = []
+        value, options = parse_param_and_options(self.PARAM_PRINT_RULES, args.print_rules, self.PRINT_RULES_VALUES)
+
+        if value == BooleanOption.TRUE.value:
+            sinks.append(ModelWriter.LogSink(options=options))
+
+        value, options = parse_param_and_options(self.PARAM_STORE_RULES, args.store_rules, self.STORE_RULES_VALUES)
+
+        if value == BooleanOption.TRUE.value and args.output_dir is not None:
+            sinks.append(ModelWriter.TxtSink(output_dir=args.output_dir, options=options))
+
+        return RuleModelWriter(sinks) if len(sinks) > 0 else None
+
+    def _create_model_characteristics_writer(self, args) -> Optional[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter` that should be used to output the
+        characteristics of models.
+
+        :param args:    The command line arguments
+        :return:        The `OutputWriter` that has been created
+        """
+        sinks = []
+
+        if args.print_model_characteristics:
+            sinks.append(ModelCharacteristicsWriter.LogSink())
+
+        if args.store_model_characteristics and args.output_dir is not None:
+            sinks.append(ModelCharacteristicsWriter.CsvSink(output_dir=args.output_dir))
+
+        return RuleModelCharacteristicsWriter(sinks) if len(sinks) > 0 else None
+
+    def _create_marginal_probability_calibration_model_writer(self, args) -> Optional[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter` that should be used to output textual
+        representations of models for the calibration of marginal probabilities.
+
+        :param args:    The command line arguments
+        :return:        The `OutputWriter` that has been created
+        """
+        sinks = []
+        value, options = parse_param_and_options(self.PARAM_PRINT_MARGINAL_PROBABILITY_CALIBRATION_MODEL,
+                                                 args.print_marginal_probability_calibration_model,
+                                                 self.PRINT_MARGINAL_PROBABILITY_CALIBRATION_MODEL_VALUES)
+
+        if value == BooleanOption.TRUE.value:
+            sinks.append(MarginalProbabilityCalibrationModelWriter.LogSink(options=options))
+
+        value, options = parse_param_and_options(self.PARAM_STORE_MARGINAL_PROBABILITY_CALIBRATION_MODEL,
+                                                 args.store_marginal_probability_calibration_model,
+                                                 self.STORE_MARGINAL_PROBABILITY_CALIBRATION_MODEL_VALUES)
+
+        if value == BooleanOption.TRUE.value and args.output_dir is not None:
+            sinks.append(MarginalProbabilityCalibrationModelWriter.CsvSink(output_dir=args.output_dir, options=options))
+
+        return MarginalProbabilityCalibrationModelWriter(sinks) if len(sinks) > 0 else None
+
+    def _create_joint_probability_calibration_model_writer(self, args) -> Optional[OutputWriter]:
+        """
+        May be overridden by subclasses in order to create the `OutputWriter` that should be used to output textual
+        representations of models for the calibration of joint probabilities.
+
+        :param args:    The command line arguments
+        :return:        The `OutputWriter` that has been created
+        """
+        sinks = []
+        value, options = parse_param_and_options(self.PARAM_PRINT_JOINT_PROBABILITY_CALIBRATION_MODEL,
+                                                 args.print_joint_probability_calibration_model,
+                                                 self.PRINT_JOINT_PROBABILITY_CALIBRATION_MODEL_VALUES)
+
+        if value == BooleanOption.TRUE.value:
+            sinks.append(JointProbabilityCalibrationModelWriter.LogSink(options=options))
+
+        value, options = parse_param_and_options(self.PARAM_STORE_JOINT_PROBABILITY_CALIBRATION_MODEL,
+                                                 args.store_joint_probability_calibration_model,
+                                                 self.STORE_JOINT_PROBABILITY_CALIBRATION_MODEL_VALUES)
+
+        if value == BooleanOption.TRUE.value and args.output_dir is not None:
+            sinks.append(JointProbabilityCalibrationModelWriter.CsvSink(output_dir=args.output_dir, options=options))
+
+        return JointProbabilityCalibrationModelWriter(sinks) if len(sinks) > 0 else None
+
+    def _create_evaluation(self, args, prediction_type: PredictionType,
+                           output_writers: List[OutputWriter]) -> Optional[Evaluation]:
+        value, options = parse_param_and_options(self.PARAM_INCREMENTAL_EVALUATION, args.incremental_evaluation,
+                                                 self.INCREMENTAL_EVALUATION_VALUES)
+
+        if value == BooleanOption.TRUE.value:
+            min_size = options.get_int(self.OPTION_MIN_SIZE, 0)
+            assert_greater_or_equal(self.OPTION_MIN_SIZE, min_size, 0)
+            max_size = options.get_int(self.OPTION_MAX_SIZE, 0)
+            if max_size != 0:
+                assert_greater(self.OPTION_MAX_SIZE, max_size, min_size)
+            step_size = options.get_int(self.OPTION_STEP_SIZE, 1)
+            assert_greater_or_equal(self.OPTION_STEP_SIZE, step_size, 1)
+            return IncrementalEvaluation(
+                prediction_type, output_writers, min_size=min_size, max_size=max_size,
+                step_size=step_size) if len(output_writers) > 0 else None
+        else:
+            return super()._create_evaluation(args, prediction_type, output_writers)
+
+    def _create_label_vector_writer(self, args) -> Optional[OutputWriter]:
+        sinks = []
+        value, options = parse_param_and_options(self.PARAM_PRINT_LABEL_VECTORS, args.print_label_vectors,
+                                                 self.PRINT_LABEL_VECTORS_VALUES)
+
+        if value == BooleanOption.TRUE.value:
+            sinks.append(LabelVectorSetWriter.LogSink(options=options))
+
+        value, options = parse_param_and_options(self.PARAM_STORE_LABEL_VECTORS, args.store_label_vectors,
+                                                 self.STORE_LABEL_VECTORS_VALUES)
+
+        if value == BooleanOption.TRUE.value and args.output_dir is not None:
+            sinks.append(LabelVectorSetWriter.CsvSink(output_dir=args.output_dir, options=options))
+
+        return LabelVectorSetWriter(sinks) if len(sinks) > 0 else None
+
+    def _create_post_training_output_writers(self, args) -> List[OutputWriter]:
+        output_writers = super()._create_post_training_output_writers(args)
+        output_writer = self._create_model_writer(args)
+
+        if output_writer is not None:
+            output_writers.append(output_writer)
+
+        output_writer = self._create_model_characteristics_writer(args)
+
+        if output_writer is not None:
+            output_writers.append(output_writer)
+
+        output_writer = self._create_marginal_probability_calibration_model_writer(args)
+
+        if output_writer is not None:
+            output_writers.append(output_writer)
+
+        output_writer = self._create_joint_probability_calibration_model_writer(args)
+
+        if output_writer is not None:
+            output_writers.append(output_writer)
+
+        return output_writers
+
+    def _create_model_characteristics_writer(self, args) -> Optional[OutputWriter]:
+        sinks = []
+
+        if args.print_model_characteristics:
+            sinks.append(ModelCharacteristicsWriter.LogSink())
+
+        if args.store_model_characteristics and args.output_dir is not None:
+            sinks.append(ModelCharacteristicsWriter.CsvSink(output_dir=args.output_dir))
+
+        return RuleModelCharacteristicsWriter(sinks) if len(sinks) > 0 else None
```

## Comparing `mlrl_testbed-0.8.2.dist-info/METADATA` & `mlrl_testbed-0.9.0.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlrl-testbed
-Version: 0.8.2
+Version: 0.9.0
 Summary: Provides utilities for the training and evaluation of multi-label rule learning algorithms
 Home-page: https://github.com/mrapp-ke/Boomer
 Download-URL: https://github.com/mrapp-ke/Boomer/releases
 Author: Michael Rapp
 Author-email: michael.rapp.ml@gmail.com
 License: MIT
 Project-URL: Documentation, https://mlrl-boomer.readthedocs.io/en/latest
@@ -16,40 +16,44 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: liac-arff (>=2.5.0)
-Requires-Dist: mlrl-common (==0.8.2)
+Requires-Dist: mlrl-common (==0.9.0)
+Requires-Dist: liac-arff (<2.6,>=2.5)
+Requires-Dist: tabulate (<0.10,>=0.9)
 Provides-Extra: boomer
-Requires-Dist: mlrl-boomer (==0.8.2) ; extra == 'boomer'
-Provides-Extra: seco
-Requires-Dist: mlrl-seco (==0.8.2) ; extra == 'seco'
+Requires-Dist: mlrl-boomer (==0.9.0) ; extra == 'boomer'
 
-# "MLRL-Testbed": Utilities for the Evaluation of Multi-label Rule Learning Algorithms
+# "MLRL-Testbed": Utilities for Evaluating Multi-label Rule Learning Algorithms
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/mlrl-testbed.svg)](https://badge.fury.io/py/mlrl-testbed)
 [![Documentation Status](https://readthedocs.org/projects/mlrl-boomer/badge/?version=latest)](https://mlrl-boomer.readthedocs.io/en/latest/?badge=latest)
 
-This software package provides **utilities for the training and evaluation of multi-label rule learning algorithms** that have been implemented using the "MLRL-Common" library, including the following ones:
+This software package provides **utilities for training and evaluating single- and multi-label rule learning algorithms** that have been implemented using the "MLRL-Common" library, including the following ones:
 
 * **BOOMER (Gradient Boosted Multi-label Classification Rules)**: A state-of-the art algorithm that uses [gradient boosting](https://en.wikipedia.org/wiki/Gradient_boosting) to learn an ensemble of rules that is built with respect to a given multivariate loss function.
 
-## Features
+## Functionalities
 
-Most notably, the package includes command line APIs that allow to configure the aforementioned algorithms, apply them to different datasets  and evaluate their predictive performance in terms of commonly used measures (provided by the [scikit-learn](https://scikit-learn.org/) framework). In addition, it provides the following functionality:
+Most notably, the package includes command line APIs that allow configuring the algorithms mentioned above, applying them to different datasets, and evaluating their predictive performance in terms of commonly used measures (provided by the [scikit-learn](https://scikit-learn.org/) framework). In summary, it provides the following functionalities:
 
-* The package supports **multi-label datasets in the [Mulan format](http://mulan.sourceforge.net/format.html)**.
-* The predictive performance of algorithms can be evaluated using **predefined splits of a dataset** into training and test data or using **cross validation**.
-* **Models can be saved into files** and reloaded for later use.
-* **Parameter tuning can be used** to determine the optimal configuration of an algorithm and write it into a configuration file, which can afterwards be used for training a model.  
-* **[Bootstrap Bias-corrected Cross Validation (BBC-CV)](https://arxiv.org/pdf/1708.07180v2.pdf)** can be used to incorporate parameter tuning and evaluation of an algorithm  in a computationally efficient way.
-* **Textual representations of rule models**, as well as the **characteristics of models or datasets** can be written into output files.
+* **Sinle- and multi-label datasets in the [Mulan](http://mulan.sourceforge.net/format.html) and [Meka format](https://waikato.github.io/meka/datasets/)** are supported.
+* **Datasets can automatically be split into training and test data, including the possibility to use cross validation.** Alternatively, predefined splits can be used by supplying the data as separate files.
+* **One-hot-encoding** can be applied to nominal or binary features.
+* **Binary predictions, regression scores, or probability estimates** can be obtained from a model. Evaluation measures that are suited for the respective type of predictions are picked automatically.
+* **Evaluation scores can be saved** to output files and printed on the console.
+* **Rule models can be evaluated incrementally**, i.e., they can be evaluated repeatedly using a subset of the rules with increasing size.
+* **Textual representations of rule models can be saved** to output files and printed on the console. In addition, the **characteristics of models can also be saved** and printed.
+* **Characteristics of datasets can be saved** to output files and printed on the console.
+* **Unique label vectors contained in a dataset can be saved** to output files and printed on the console.
+* **Predictions can be saved** to output files and printed on the console. In addition, **characteristics of binary predictions can also be saved** and printed.
+* **Models for the calibration of probabilities can be saved** to output files and printed on the console.
+* **Models can be saved on disk** in order to be reused by future experiments.
+* **Algorithmic parameters can be read from configuration files** instead of providing them via command line arguments. When providing parameters via the command line, corresponding configuration files can automatically be saved on disk.
 
 ## License
 
-This project is open source software licensed under the terms of the [MIT license](https://github.com/mrapp-ke/Boomer/blob/master/LICENSE.txt). We welcome contributions to the project to enhance its functionality and make it more accessible to a broader audience. A frequently updated list of contributors is available [here](https://github.com/mrapp-ke/Boomer/blob/master/CONTRIBUTORS.md). 
-
-
+This project is open source software licensed under the terms of the [MIT license](../../../LICENSE.md). We welcome contributions to the project to enhance its functionality and make it more accessible to a broader audience. A frequently updated list of contributors is available [here](../../../CONTRIBUTORS.md).
```

