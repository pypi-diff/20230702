# Comparing `tmp/ome_types-0.3.4.tar.gz` & `tmp/ome_types-0.4.0a1.tar.gz`

## Comparing `ome_types-0.3.4.tar` & `ome_types-0.4.0a1.tar`

### file list

```diff
@@ -1,168 +1,40 @@
--rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.3.4/CHANGELOG.md
--rw-r--r--   0        0        0    40113 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_autogen.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/__init__.py
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/_base_type.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/_constants.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/_convenience.py
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/_lxml.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/_napari_plugin.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/_units.py
--rw-r--r--   0        0        0    11599 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/_xmlschema.py
--rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/ome-2016-06.xsd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/py.typed
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/schema.py
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/util.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/widgets.py
--rw-r--r--   0        0        0    42098 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/__init__.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/affine_transform.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/annotation.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/annotation_ref.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/arc.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/basic_annotation.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/bin_data.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/binary_file.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/boolean_annotation.py
--rw-r--r--   0        0        0     7641 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/channel.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/channel_ref.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/comment_annotation.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/dataset.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/dataset_ref.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/detector.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/detector_settings.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/dichroic.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/dichroic_ref.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/double_annotation.py
--rw-r--r--   0        0        0     2795 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/ellipse.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/experiment.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/experiment_ref.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/experimenter.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/experimenter_group.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/experimenter_group_ref.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/experimenter_ref.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/external.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/filament.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/file_annotation.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/filter.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/filter_ref.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/filter_set.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/filter_set_ref.py
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/folder.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/folder_ref.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/generic_excitation_source.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/image.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/image_ref.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/imaging_environment.py
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/instrument.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/instrument_ref.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/label.py
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/laser.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/leader.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/light_emitting_diode.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/light_path.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/light_source.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/light_source_group.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/light_source_settings.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/line.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/list_annotation.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/long_annotation.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/manufacturer_spec.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/map.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/map_annotation.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/mask.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/microbeam_manipulation.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/microbeam_manipulation_ref.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/microscope.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/numeric_annotation.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/objective.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/objective_settings.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/ome.py
--rw-r--r--   0        0        0     5752 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/pixels.py
--rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/plane.py
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/plate.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/plate_acquisition.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/point.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/polygon.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/polyline.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/project.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/project_ref.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/pump.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/reagent.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/reagent_ref.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/rectangle.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/reference.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/rights.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/roi.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/roi_ref.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/screen.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/settings.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/shape.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/shape_group.py
--rw-r--r--   0        0        0    10674 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/simple_types.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/stage_label.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/structured_annotations.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/tag_annotation.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/term_annotation.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/text_annotation.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/tiff_data.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/timestamp_annotation.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/transmittance_range.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/type_annotation.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/well.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/well_sample.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/well_sample_ref.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 ome_types-0.3.4/src/ome_types/model/xml_annotation.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/test_autogen.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/test_invalid_schema.py
--rw-r--r--   0        0        0     8197 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/test_model.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/test_serialization.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/test_units.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/test_widget.py
--rw-r--r--   0        0        0    12646 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/util.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/OverViewScan.ome.xml
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/ROI.ome.xml
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/bad.ome.xml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/commentannotation.ome.xml
--rw-r--r--   0        0        0    47901 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/example.ome.xml
--rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/fake-plate-rows-2.ome.xml
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/filter.ome.xml
--rw-r--r--   0        0        0   267379 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/folders-larger-taxonomy.ome.xml
--rw-r--r--   0        0        0   264656 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/folders-simple-taxonomy.ome.xml
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/hcs.ome.xml
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/instrument-units-alternate.ome.xml
--rw-r--r--   0        0        0     4388 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/instrument-units-default.ome.xml
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/instrument.ome.xml
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/invalid_xml_annotation.ome.xml
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/mapannotation.ome.xml
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/metadata-only.ome.xml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/minimum-specification.ome.xml
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/multi-channel-time-series.ome.xml
--rw-r--r--   0        0        0    33349 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/multi-channel-z-series-time-series.ome.xml
--rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/multi-channel-z-series.ome.xml
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/multi-channel.ome.xml
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/no-date.ome.xml
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/ome.tiff
--rw-r--r--   0        0        0    12159 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/ome_ns.ome.xml
--rw-r--r--   0        0        0     8221 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/one-screen-one-plate-four-wells.ome.xml
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/shape-union.ome.xml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/single-image.ome.xml
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/small.ome.xml
--rw-r--r--   0        0        0    23160 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/spim.ome.xml
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/tagannotation.ome.xml
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/time-series.ome.xml
--rw-r--r--   0        0        0     8804 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/timestampannotation-posix-only.ome.xml
--rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/timestampannotation.ome.xml
--rw-r--r--   0        0        0     8041 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/transformations-downgrade.ome.xml
--rw-r--r--   0        0        0     8348 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/transformations-upgrade.ome.xml
--rw-r--r--   0        0        0    13260 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/tubhiswt.ome.xml
--rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/two-screens-two-plates-four-wells.ome.xml
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/xmlannotation-body-space.ome.xml
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/xmlannotation-multi-value.ome.xml
--rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/xmlannotation-svg.ome.xml
--rw-r--r--   0        0        0    16972 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/z-series-time-series.ome.xml
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 ome_types-0.3.4/tests/data/z-series.ome.xml
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 ome_types-0.3.4/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.3.4/LICENSE
--rw-r--r--   0        0        0     9466 2020-02-02 00:00:00.000000 ome_types-0.3.4/README.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 ome_types-0.3.4/hatch_build.py
--rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 ome_types-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 ome_types-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    16554 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/__main__.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/_config.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/_generator.py
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/_transformer.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/_util.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_autogen/main.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/__init__.py
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_conversion.py
+-rw-r--r--   0        0        0   285655 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/ome-2016-06.xsd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/py.typed
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/units.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/__init__.py
+-rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_base_type.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_bin_data.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_instrument.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_ome.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_reference.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/_mixins/_structured_annotations.py
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/model/__init__.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/model/_color.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/model/_shape_union.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/model/_user_sequence.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/ome_types/model/simple_types.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/__init__.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/bindings.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/compat.py
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/hooks/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/hooks/class_type.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/src/xsdata_pydantic_basemodel/hooks/cli.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/LICENSE
+-rw-r--r--   0        0        0     9347 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/README.md
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/hatch_build.py
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 ome_types-0.4.0a1/PKG-INFO
```

### Comparing `ome_types-0.3.4/CHANGELOG.md` & `ome_types-0.4.0a1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ome_types-0.3.4/src/ome_types/_base_type.py` & `ome_types-0.4.0a1/src/ome_types/_mixins/_base_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,97 @@
-from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional, Sequence, Set
+import contextlib
+import re
+import warnings
+from datetime import datetime
+from enum import Enum
+from textwrap import indent
+from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional, Sequence, Set, cast
 
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, PrivateAttr, validator
+
+from ome_types.units import ureg
 
 if TYPE_CHECKING:
     import pint
 
 
-class Sentinel:
-    """Create singleton sentinel objects with a readable repr."""
-
-    def __init__(self, name: str) -> None:
-        self.name = name
-
-    def __repr__(self) -> str:
-        return f"{__name__}.{self.name}.{id(self)}"
-
-
-def quantity_property(field: str) -> property:
-    """Create property that returns a ``pint.Quantity`` combining value and unit."""
-
-    def quantity(self: Any) -> Optional["pint.Quantity"]:
-        from ome_types._units import ureg
+# Default value to support automatic numbering for id field values.
+AUTO_SEQUENCE = "__auto_sequence__"
 
-        value = getattr(self, field)
-        if value is None:
-            return None
-        unit = getattr(self, f"{field}_unit").value.replace(" ", "_")
-        return ureg.Quantity(value, unit)
-
-    return property(quantity)
+_COUNTERS: Dict[str, int] = {}
+_UNIT_FIELD = "{}_unit"
+_QUANTITY_FIELD = "{}_quantity"
+DEPRECATED_NAMES = {
+    "annotation_ref": "annotation_refs",
+    "bin_data": "bin_data_blocks",
+    "dataset_ref": "dataset_refs",
+    "emission_filter_ref": "emission_filters",
+    "excitation_filter_ref": "excitation_filters",
+    "experimenter_ref": "experimenter_refs",
+    "folder_ref": "folder_refs",
+    "image_ref": "image_refs",
+    "leader": "leaders",
+    "light_source_settings": "light_source_settings_combinations",
+    "m": "ms",
+    "microbeam_manipulation_ref": "microbeam_manipulation_refs",
+    "plate_ref": "plate_refs",
+    "roi_ref": "roi_refs",
+    "well_sample_ref": "well_sample_refs",
+}
 
 
 class OMEType(BaseModel):
     """The base class that all OME Types inherit from.
 
     This provides some global conveniences around auto-setting ids. (i.e., making them
     optional in the class constructor, but never ``None`` after initialization.).
     It provides a nice __repr__ that hides things that haven't been changed from
     defaults.  It adds ``*_quantity`` property for fields that have both a value and a
     unit, where ``*_quantity`` is a pint ``Quantity``.  It also provides pickling
     support.
     """
 
-    # Default value to support automatic numbering for id field values.
-    _AUTO_SEQUENCE = Sentinel("AUTO_SEQUENCE")
+    # pydantic BaseModel configuration.
+    # see: https://pydantic-docs.helpmanual.io/usage/model_config/
+    class Config:
+        arbitrary_types_allowed = False
+        validate_assignment = True
+        underscore_attrs_are_private = True
+        use_enum_values = False
+        validate_all = True
+        validation_mode: str = "strict"
+
     # allow use with weakref
     __slots__: ClassVar[Set[str]] = {"__weakref__"}  # type: ignore
+    _validation_mode: str = PrivateAttr("strict")
 
     def __init__(__pydantic_self__, **data: Any) -> None:
         if "id" in __pydantic_self__.__fields__:
-            data.setdefault("id", OMEType._AUTO_SEQUENCE)
+            data.setdefault("id", AUTO_SEQUENCE)
         super().__init__(**data)
 
     def __init_subclass__(cls) -> None:
-        """Add some properties to subclasses with units.
+        """Add `*_quantity` property for fields that have both a value and a unit.
 
-        It adds ``*_quantity`` property for fields that have both a value and a
-        unit, where ``*_quantity`` is a pint ``Quantity``
+        where `*_quantity` is a pint `Quantity`.
         """
-        _clsdir = set(cls.__fields__)
-        for field in _clsdir:
-            if f"{field}_unit" in _clsdir:
-                setattr(cls, f"{field}_quantity", quantity_property(field))
-
-    # pydantic BaseModel configuration.
-    # see: https://pydantic-docs.helpmanual.io/usage/model_config/
-    class Config:
-        # whether to allow arbitrary user types for fields (they are validated
-        # simply by checking if the value is an instance of the type). If
-        # False, RuntimeError will be raised on model declaration
-        arbitrary_types_allowed = False
-        # whether to perform validation on assignment to attributes
-        validate_assignment = True
-        # whether to treat any underscore non-class var attrs as private
-        # https://pydantic-docs.helpmanual.io/usage/models/#private-model-attributes
-        underscore_attrs_are_private = True
-        # whether to populate models with the value property of enums, rather
-        # than the raw enum. This may be useful if you want to serialise
-        # model.dict() later.  False by default
-        # see conversation in https://github.com/tlambert03/ome-types/pull/74
-        use_enum_values = False
-        # whether to validate field defaults (default: False)
-        validate_all = True
-
-    def __repr__(self: Any) -> str:
-        from datetime import datetime
-        from enum import Enum
-        from textwrap import indent
+        for field in cls.__fields__:
+            if _UNIT_FIELD.format(field) in cls.__fields__:
+                setattr(cls, _QUANTITY_FIELD.format(field), _quantity_property(field))
 
+    def __repr__(self) -> str:
         name = self.__class__.__qualname__
         lines = []
         for f in sorted(
             self.__fields__.values(), key=lambda f: f.name not in ("name", "id")
         ):
             if f.name.endswith("_"):
-                continue
+                continue  # pragma: no cover
             # https://github.com/python/mypy/issues/6910
-            if f.default_factory:
-                default = f.default_factory()
-            else:
-                default = f.default
-
+            default = f.default_factory() if f.default_factory else f.default
             current = getattr(self, f.name)
             if current != default:
                 if isinstance(current, Sequence) and not isinstance(current, str):
                     rep = f"[<{len(current)} {f.name.title()}>]"
                 elif isinstance(current, Enum):
                     rep = repr(current.value)
                 elif isinstance(current, datetime):
@@ -114,56 +101,76 @@
                 lines.append(f"{f.name}={rep},")
         if len(lines) == 1:
             body = lines[-1].rstrip(",")
         elif lines:
             body = "\n" + indent("\n".join(lines), "   ") + "\n"
         else:
             body = ""
-        out = f"{name}({body})"
-        return out
+        return f"{name}({body})"
 
     @validator("id", pre=True, always=True, check_fields=False)
-    def validate_id(cls, value: Any) -> str:
+    @classmethod
+    def _validate_id(cls, value: Any) -> Any:
         """Pydantic validator for ID fields in OME models.
 
         If no value is provided, this validator provides and integer ID, and stores the
         maximum previously-seen value on the class.
         """
-        from typing import ClassVar
+        # FIXME: clean this up
+        id_field = cls.__fields__["id"]
+        id_regex = cast(str, id_field.field_info.regex)
+        id_name = id_regex.split(":")[-3]
+
+        current_count = _COUNTERS.setdefault(id_name, -1)
+        if isinstance(value, str) and value != AUTO_SEQUENCE:
+            # parse the id and update the counter
+            *name, v_id = value.rsplit(":", 1)
+            if not re.match(id_regex, value):
+                newname = cls._validate_id(
+                    int(v_id) if v_id.isnumeric() else AUTO_SEQUENCE
+                )
+                warnings.warn(
+                    f"Casting invalid {id_name}ID {value!r} to {newname!r}",
+                    stacklevel=2,
+                )
+                return newname
 
-        # get the required LSID field from the annotation
-        id_field = cls.__fields__.get("id")
-        if not id_field:
+            with contextlib.suppress(ValueError):
+                _COUNTERS[id_name] = max(current_count, int(v_id))
             return value
 
-        # Store the highest seen value on the class._max_id attribute.
-        if not hasattr(cls, "_max_id"):
-            cls._max_id = 0  # type: ignore [misc]
-            cls.__annotations__["_max_id"] = ClassVar[int]
-        if value is OMEType._AUTO_SEQUENCE:
-            value = cls._max_id + 1
         if isinstance(value, int):
-            v_id = value
-            id_string = id_field.type_.__name__[:-2]
-            value = f"{id_string}:{value}"
+            _COUNTERS[id_name] = max(current_count, value)
+        elif value == AUTO_SEQUENCE:
+            # just increment the counter
+            _COUNTERS[id_name] += 1
+            value = _COUNTERS[id_name]
         else:
-            value = str(value)
-            v_id = value.rsplit(":", 1)[-1]
-        try:
-            v_id = int(v_id)
-            cls._max_id = max(cls._max_id, v_id)  # type: ignore [misc]
-        except ValueError:
-            pass
-
-        return id_field.type_(value)
-
-    def __getstate__(self: Any) -> Dict[str, Any]:
-        """Support pickle of our weakref references."""
-        state = super().__getstate__()
-        state["__private_attribute_values__"].pop("_ref", None)
-        return state
+            raise ValueError(f"Invalid ID value: {value!r}, {type(value)}")
+
+        return f"{id_name}:{value}"
+
+    def __getattr__(self, key: str) -> Any:
+        cls_name = self.__class__.__name__
+        if key in DEPRECATED_NAMES and hasattr(self, DEPRECATED_NAMES[key]):
+            new_key = DEPRECATED_NAMES[key]
+            warnings.warn(
+                f"Attribute '{cls_name}.{key}' is deprecated, use {new_key!r} instead",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+            return getattr(self, new_key)
+        raise AttributeError(f"{cls_name} object has no attribute {key!r}")
 
-    @classmethod
-    def snake_name(cls) -> str:
-        from .model import _camel_to_snake
 
-        return _camel_to_snake[cls.__name__]
+def _quantity_property(field_name: str) -> property:
+    """Create property that returns a ``pint.Quantity`` combining value and unit."""
+
+    def quantity(self: Any) -> Optional["pint.Quantity"]:
+        value = getattr(self, field_name)
+        if value is None:
+            return None
+
+        unit = cast("Enum", getattr(self, _UNIT_FIELD.format(field_name)))
+        return ureg.Quantity(value, unit.value.replace(" ", "_"))
+
+    return property(quantity)
```

### Comparing `ome_types-0.3.4/src/ome_types/ome-2016-06.xsd` & `ome_types-0.4.0a1/src/ome_types/ome-2016-06.xsd`

 * *Files identical despite different names*

### Comparing `ome_types-0.3.4/src/ome_types/util.py` & `ome_types-0.4.0a1/src/ome_types/_mixins/_ome.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 from __future__ import annotations
 
-import re
-from functools import lru_cache
-from pathlib import Path
-from typing import TYPE_CHECKING, Any
-
-from . import model
-from ._base_type import OMEType
-from .model.reference import Reference
+import weakref
+from typing import TYPE_CHECKING, Any, cast
+
+from ome_types._mixins._base_type import OMEType
 
 if TYPE_CHECKING:
-    from .model.simple_types import LSID
+    from pathlib import Path
 
+    from ome_types._autogenerated.ome_2016_06 import OME, Reference
 
-def cast_number(qnum: str) -> str | int | float:
-    """Attempt to cast a number from a string.
 
-    This function attempts to cast a string to a number. It will first try to parse an
-    int, then a float, and finally returns a string if both fail.
-    """
-    try:
-        return int(qnum)
-    except ValueError:
-        try:
-            return float(qnum)
-        except ValueError:
-            return qnum
+class OMEMixin:
+    def __init__(self, **data: Any) -> None:
+        super().__init__(**data)
+        self._link_refs()
 
+    def _link_refs(self) -> None:
+        ids = collect_ids(self)
+        for ref in collect_references(self):
+            # all reference subclasses do actually have an 'id' field
+            # but it's not declared in the base class
+            ref._ref = weakref.ref(ids[ref.id])  # type: ignore [attr-defined]
 
-def collect_references(value: Any) -> list[Reference]:
-    """Return a list of all References contained in value.
+    def __setstate__(self, state: dict[str, Any]) -> None:
+        """Support unpickle of our weakref references."""
+        super().__setstate__(state)  # type: ignore
+        self._link_refs()
 
-    Recursively walks all dataclass fields and iterates over lists. The base
-    case is when value is either a Reference object, or an uninteresting type
-    that we don't need to inspect further.
+    @classmethod
+    def from_xml(cls, xml: Path | str) -> OME:
+        from ome_types._conversion import from_xml
 
-    """
-    references: list[Reference] = []
-    if isinstance(value, Reference):
-        references.append(value)
-    elif isinstance(value, list):
-        for v in value:
-            references.extend(collect_references(v))
-    elif isinstance(value, OMEType):
-        for f in value.__fields__:
-            references.extend(collect_references(getattr(value, f)))
-    # Do nothing for uninteresting types
-    return references
+        return from_xml(xml)
+
+    @classmethod
+    def from_tiff(cls, path: Path | str) -> OME:
+        from ome_types._conversion import from_tiff
+
+        return from_tiff(path)
 
+    def to_xml(self) -> str:
+        from ome_types._conversion import to_xml
 
-def collect_ids(value: Any) -> dict[LSID, OMEType]:
+        return to_xml(cast("OME", self))
+
+
+def collect_ids(value: Any) -> dict[str, OMEType]:
     """Return a map of all model objects contained in value, keyed by id.
 
     Recursively walks all dataclass fields and iterates over lists. The base
     case is when value is neither a dataclass nor a list.
     """
-    ids: dict[LSID, OMEType] = {}
+    from ome_types.model import Reference
+
+    ids: dict[str, OMEType] = {}
     if isinstance(value, list):
         for v in value:
             ids.update(collect_ids(v))
     elif isinstance(value, OMEType):
         for f in value.__fields__:
             if f == "id" and not isinstance(value, Reference):
                 # We don't need to recurse on the id string, so just record it
@@ -67,40 +66,28 @@
                 ids[value.id] = value  # type: ignore
             else:
                 ids.update(collect_ids(getattr(value, f)))
     # Do nothing for uninteresting types.
     return ids
 
 
-CAMEL_REGEX = re.compile(r"(?<!^)(?=[A-Z])")
+def collect_references(value: Any) -> list[Reference]:
+    """Return a list of all References contained in value.
 
+    Recursively walks all dataclass fields and iterates over lists. The base
+    case is when value is either a Reference object, or an uninteresting type
+    that we don't need to inspect further.
 
-@lru_cache()
-def camel_to_snake(name: str) -> str:
-    """Return a snake_case version of a camelCase string."""
-    return model._camel_to_snake.get(name, CAMEL_REGEX.sub("_", name).lower())
-
-
-@lru_cache()
-def norm_key(key: str) -> str:
-    """Return a normalized key."""
-    return key.split("}")[-1]
-
-
-def _get_plural(key: str, tag: str) -> str:
-    return model._singular_to_plural.get((norm_key(tag), key), key)
-
-
-def _ensure_xml_bytes(path_or_str: Path | str | bytes) -> bytes:
-    """Ensure that `path_or_str` is bytes.  Read from disk if it's an existing file."""
-    if isinstance(path_or_str, Path):
-        return path_or_str.read_bytes()
-    if isinstance(path_or_str, str):
-        # FIXME: deal with magic number 10.  I think it's to avoid Path.exists
-        # failure on a full string
-        if "xml" not in path_or_str[:10] and Path(path_or_str).exists():
-            return Path(path_or_str).read_bytes()
-        else:
-            return path_or_str.encode()
-    if isinstance(path_or_str, bytes):
-        return path_or_str
-    raise TypeError("path_or_str must be one of [Path, str, bytes].  I")
+    """
+    from ome_types.model import Reference
+
+    references: list[Reference] = []
+    if isinstance(value, Reference):
+        references.append(value)
+    elif isinstance(value, list):
+        for v in value:
+            references.extend(collect_references(v))
+    elif isinstance(value, OMEType):
+        for f in value.__fields__:
+            references.extend(collect_references(getattr(value, f)))
+    # Do nothing for uninteresting types
+    return references
```

### Comparing `ome_types-0.3.4/.gitignore` & `ome_types-0.4.0a1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -103,12 +103,13 @@
 # mypy
 .mypy_cache/
 .vscode/
 
 
 .DS_Store
 _test_data
-src/ome_types/model/
+src/ome_types/_autogenerated/
 src/ome_types/_version.py
 docs/source/_autosummary
 .benchmarks/
 _build/
+qupath/
```

### Comparing `ome_types-0.3.4/LICENSE` & `ome_types-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ome_types-0.3.4/README.md` & `ome_types-0.4.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -300,10 +300,7 @@
 ```
 
 ### Running tests
 
 To run tests quickly, just install and run `pytest`.  Note, however, that this
 requires that the `ome_types.model` module has already been built with `python
 src/ome_autogen.py`.
-
-Alternatively, you can install and run `tox` which will run tests and
-code-quality checks in an isolated environment.
```

### Comparing `ome_types-0.3.4/pyproject.toml` & `ome_types-0.4.0a1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,179 +1,193 @@
 # https://peps.python.org/pep-0517/
 [build-system]
 requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
-# https://hatch.pypa.io/latest/config/metadata/
-[tool.hatch.version]
-source = "vcs"
-
-[tool.hatch.build]
-artifacts = ["src/ome_types/model"]
-
-[tool.hatch.build.targets.sdist]
-include = ["src", "tests", "CHANGELOG.md"]
-
-[tool.hatch.build.hooks.custom]
-# requirements to run the autogen script in hatch_build.py
-dependencies = [
-  "black",
-  "isort>=5.0",
-  "xmlschema==1.4.1",
-  "autoflake",
-  "numpydoc",
-]
-
 # https://peps.python.org/pep-0621/
 [project]
 name = "ome-types"
 description = "Python dataclasses for the OME data model"
 keywords = ["ome", "ome-model", "microscopy", "schema", "types"]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = { text = "MIT" }
 authors = [{ name = "Talley Lambert", email = "talley.lambert@gmail.com" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
-dependencies = [
-  "Pint >=0.15",
-  "lxml >=4.8.0",
-  "pydantic[email] >=1.0, <2.0",
-  "xmlschema >=2.0.0",
-]
+dependencies = ["Pint >=0.15", "lxml >=4.8.0", "pydantic[email] <2.0", "xsdata"]
 
 [project.urls]
 Source = "https://github.com/tlambert03/ome-types"
 Tracker = "https://github.com/tlambert03/ome-types/issues"
 Documentation = "https://ome-types.readthedocs.io/en/latest/"
 
 [project.entry-points."napari.plugin"]
 ome-types = "ome_types._napari_plugin"
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
-autogen = ["autoflake", "black", "isort>=5.0", "numpydoc"]
+dev = ["black", "ruff", "xsdata[cli]>=23.6", "mypy"]
 docs = [
-  "autoflake",
-  "black",
-  "ipython",
-  "isort>=5.0",
   "numpydoc",
   "pygments",
   "sphinx==5.3.0",
   "sphinx-rtd-theme==1.1.1",
+  "ipython",
 ]
-test = ["pytest", "pytest-cov", "pytest-benchmark", "tox"]
+test = ["pytest", "pytest-cov", "xmlschema", "distributed"]
 
+# https://hatch.pypa.io/latest/plugins/build-hook/custom/
+[tool.hatch.build.targets.wheel.hooks.custom]
+# requirements to run the autogen script in hatch_build.py
+require-runtime-dependencies = true
+dependencies = ["black", "ruff", "xsdata[cli]>=23.6"]
+
+
+# https://hatch.pypa.io/latest/config/metadata/
+[tool.hatch]
+version = { source = "vcs" }
+
+[tool.hatch.build.targets.wheel]
+only-include = ["src/ome_types", "src/xsdata_pydantic_basemodel"]
+sources = ["src"]
+artifacts = ["src/ome_types/_autogenerated"]
+
+[tool.hatch.build.targets.sdist]
+include = ["src", "CHANGELOG.md", "hatch_build.py"]
+exclude = ["src/ome_types/_autogenerated"]
 
-[tool.setuptools_scm]
-write_to = "src/ome_types/_version.py"
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 line-length = 88
 src = ["src", "tests"]
-target-version = "py37"
-extend-select = [
+target-version = "py38"
+select = [
   "E",    # style errors
   "F",    # flakes
   "D",    # pydocstyle
-  "I001", # isort
+  "I",    # isort
   "UP",   # pyupgrade
-  # "N",  # pep8-naming
   "S",    # bandit
-  "C",    # flake8-comprehensions
+  "C4",   # flake8-comprehensions
   "B",    # flake8-bugbear
   "A001", # flake8-builtins
+  "TID",  # tidy
+  "TCH",  # typechecking
   "RUF",  # ruff-specific rules
 ]
-extend-ignore = [
-  "D100", # Missing docstring in public module
-  "D104", # Missing docstring in public package
-  "D107", # Missing docstring in __init__
-  "D203", # 1 blank line required before class docstring
-  "D212", # Multi-line docstring summary should start at the first line
-  "D213", # Multi-line docstring summary should start at the second line
-  "D400", # First line should end with a period
-  "D413", # Missing blank line after last section
-  "D416", # Section name should end with a colon
-  "C901", # Function is too complex
+ignore = [
+  "D100",   # Missing docstring in public module
+  "D101",   # Missing docstring in public class
+  "D104",   # Missing docstring in public package
+  "D106",   # Missing docstring in public nested class
+  "D107",   # Missing docstring in __init__
+  "D203",   # 1 blank line required before class docstring
+  "D205",   # 1 blank line required between summary line and description
+  "D212",   # Multi-line docstring summary should start at the first line
+  "D213",   # Multi-line docstring summary should start at the second line
+  "D400",   # First line should end with a period
+  "D404",   # First word of the docstring should not be This
+  "D413",   # Missing blank line after last section
+  "D416",   # Section name should end with a colon
+  "C901",   # Function is too complex
+  "RUF009", # Do not perform function calls in default arguments
 ]
+exclude = ['src/_ome_autogen.py']
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all" # Disallow all relative imports.
 
 [tool.ruff.per-file-ignores]
 "tests/*.py" = ["D", "S"]
 "src/ome_autogen.py" = ["D10", "E501"]
 ".github/*.py" = ["D"]
 "setup.py" = ["D"]
 "docs/**/*.py" = ["D"]
+"src/xsdata_pydantic_basemodel/**/*.py" = ["D"]
 
 [tool.check-manifest]
 ignore = [
-  "src/ome_types/model/*",
   "coverage.yml",
   ".pre-commit-config.yaml",
   ".github_changelog_generator",
   ".readthedocs.yml",
   "docs/**/*",
-  "setup.py",
-  "tox.ini",
+  "tests/**/*",
 ]
 
 
 [tool.isort]
 profile = "black"
 line_length = 88
 float_to_top = true
 skip_glob = ["*examples/*", "*vendored*"]
 
 [tool.black]
-target-version = ['py37', 'py38']
-exclude = '''
-/(
-    \.git
-  | \.hg
-  | \.mypy_cache
-  | \.tox
-  | \.venv
-  | _build
-  | buck-out
-  | build
-  | dist
-  | docs
-)/
-'''
+target-version = ['py38']
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "--benchmark-disable"
 testpaths = ["tests"]
 filterwarnings = [
   "error",
   "ignore:Casting invalid AnnotationID:UserWarning",
+  # FIXME: i think this might be an xsdata issue?
+  "ignore::ResourceWarning",
+  "ignore:::pkg_resources",  # paquo tests
+  "ignore:::paquo",          # paquo tests
 ]
 
 # https://mypy.readthedocs.io/en/stable/config_file.html
 [tool.mypy]
 files = "src/**/*/*.py"
 follow_imports = 'silent'
 strict_optional = true
 warn_redundant_casts = true
 disallow_any_generics = false
 no_implicit_reexport = true
 ignore_missing_imports = true
 disallow_untyped_defs = true
+
+[[tool.mypy.overrides]]
+module = ['ome_types._autogenerated.ome_2016_06.structured_annotations']
+# Definition of "__iter__" in base class "BaseModel"
+# is incompatible with definition in base class "Sequence"
+disable_error_code = "misc"
+
+# https://coverage.readthedocs.io/en/6.4/config.html
+[tool.coverage.report]
+exclude_lines = [
+  "pragma: no cover",
+  "if TYPE_CHECKING:",
+  "@overload",
+  "except ImportError",
+  "\\.\\.\\.",
+  "raise NotImplementedError()",
+]
+
+[tool.coverage.run]
+source = ["src/ome_types", "src/ome_autogen"]
+
+
+# Entry points -- REMOVE ONCE XSDATA-PYDANTIC-BASEMODEL IS SEPARATE
+[project.entry-points."xsdata.plugins.class_types"]
+xsdata_pydantic_basemodel = "xsdata_pydantic_basemodel.hooks.class_type"
+
+[project.entry-points."xsdata.plugins.cli"]
+xsdata_pydantic_basemodel = "xsdata_pydantic_basemodel.hooks.cli"
```

### Comparing `ome_types-0.3.4/PKG-INFO` & `ome_types-0.4.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-types
-Version: 0.3.4
+Version: 0.4.0a1
 Summary: Python dataclasses for the OME data model
 Project-URL: Source, https://github.com/tlambert03/ome-types
 Project-URL: Tracker, https://github.com/tlambert03/ome-types/issues
 Project-URL: Documentation, https://ome-types.readthedocs.io/en/latest/
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -13,43 +13,39 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Requires-Dist: lxml>=4.8.0
 Requires-Dist: pint>=0.15
-Requires-Dist: pydantic[email]<2.0,>=1.0
-Requires-Dist: xmlschema>=2.0.0
-Provides-Extra: autogen
-Requires-Dist: autoflake; extra == 'autogen'
-Requires-Dist: black; extra == 'autogen'
-Requires-Dist: isort>=5.0; extra == 'autogen'
-Requires-Dist: numpydoc; extra == 'autogen'
+Requires-Dist: pydantic[email]<2.0
+Requires-Dist: xsdata
+Provides-Extra: dev
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: xsdata[cli]>=23.6; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: autoflake; extra == 'docs'
-Requires-Dist: black; extra == 'docs'
 Requires-Dist: ipython; extra == 'docs'
-Requires-Dist: isort>=5.0; extra == 'docs'
 Requires-Dist: numpydoc; extra == 'docs'
 Requires-Dist: pygments; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme==1.1.1; extra == 'docs'
 Requires-Dist: sphinx==5.3.0; extra == 'docs'
 Provides-Extra: test
+Requires-Dist: distributed; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
-Requires-Dist: pytest-benchmark; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
-Requires-Dist: tox; extra == 'test'
+Requires-Dist: xmlschema; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ome-types
 
 [![License](https://img.shields.io/github/license/tlambert03/ome-types)](LICENSE)
 [![Version](https://img.shields.io/pypi/v/ome-types.svg)](https://pypi.python.org/pypi/ome-types)
 [![CondaVersion](https://img.shields.io/conda/v/conda-forge/ome-types)](https://anaconda.org/conda-forge/ome-types)
@@ -350,10 +346,7 @@
 ```
 
 ### Running tests
 
 To run tests quickly, just install and run `pytest`.  Note, however, that this
 requires that the `ome_types.model` module has already been built with `python
 src/ome_autogen.py`.
-
-Alternatively, you can install and run `tox` which will run tests and
-code-quality checks in an isolated environment.
```

