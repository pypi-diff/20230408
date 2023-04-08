# Comparing `tmp/oct_converter-0.5.7.tar.gz` & `tmp/oct_converter-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oct_converter-0.5.7.tar", last modified: Tue Mar 28 19:28:56 2023, max compression
+gzip compressed data, was "oct_converter-0.5.8.tar", last modified: Tue Apr  4 18:11:46 2023, max compression
```

## Comparing `oct_converter-0.5.7.tar` & `oct_converter-0.5.8.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-28 19:28:56.746683 oct_converter-0.5.7/
--rw-r--r--   0 mark       (501) staff       (20)     1069 2022-04-20 18:45:33.000000 oct_converter-0.5.7/LICENSE
--rw-r--r--   0 mark       (501) staff       (20)       22 2022-05-25 18:52:16.000000 oct_converter-0.5.7/MANIFEST.in
--rw-r--r--   0 mark       (501) staff       (20)     5958 2023-03-28 19:28:56.746251 oct_converter-0.5.7/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     4178 2023-03-28 19:28:23.000000 oct_converter-0.5.7/README.md
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-28 19:28:56.726916 oct_converter-0.5.7/examples/
--rw-r--r--   0 mark       (501) staff       (20)      473 2022-11-23 17:04:52.000000 oct_converter-0.5.7/examples/demo_boct_extraction.py
--rw-r--r--   0 mark       (501) staff       (20)      251 2022-11-18 21:45:03.000000 oct_converter-0.5.7/examples/demo_dicom_extraction.py
--rw-r--r--   0 mark       (501) staff       (20)      613 2023-01-13 21:03:00.000000 oct_converter-0.5.7/examples/demo_e2e_extraction.py
--rw-r--r--   0 mark       (501) staff       (20)     1136 2023-03-28 18:59:04.000000 oct_converter-0.5.7/examples/demo_fda_extraction.py
--rw-r--r--   0 mark       (501) staff       (20)      952 2023-03-28 19:28:23.000000 oct_converter-0.5.7/examples/demo_fds_extraction.py
--rw-r--r--   0 mark       (501) staff       (20)      304 2022-11-18 21:50:55.000000 oct_converter-0.5.7/examples/demo_img_extraction.py
--rw-r--r--   0 mark       (501) staff       (20)      233 2023-01-16 22:40:53.000000 oct_converter-0.5.7/examples/demo_optovue_extraction.py
--rw-r--r--   0 mark       (501) staff       (20)      402 2023-01-13 21:03:10.000000 oct_converter-0.5.7/examples/demo_zeissdicom_extraction.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-28 19:28:56.727597 oct_converter-0.5.7/oct_converter/
--rw-r--r--   0 mark       (501) staff       (20)        0 2019-08-08 14:39:58.000000 oct_converter-0.5.7/oct_converter/__init__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-28 19:28:56.729840 oct_converter-0.5.7/oct_converter/exceptions/
--rw-r--r--   0 mark       (501) staff       (20)      156 2023-01-17 16:31:46.000000 oct_converter-0.5.7/oct_converter/exceptions/__init__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-28 19:28:56.732703 oct_converter-0.5.7/oct_converter/image_types/
--rw-r--r--   0 mark       (501) staff       (20)       83 2022-05-25 16:10:32.000000 oct_converter-0.5.7/oct_converter/image_types/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     1318 2023-03-28 19:16:43.000000 oct_converter-0.5.7/oct_converter/image_types/fundus.py
--rw-r--r--   0 mark       (501) staff       (20)     5707 2023-03-28 18:59:04.000000 oct_converter-0.5.7/oct_converter/image_types/oct.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-28 19:28:56.740724 oct_converter-0.5.7/oct_converter/readers/
--rw-r--r--   0 mark       (501) staff       (20)      190 2022-11-18 21:45:03.000000 oct_converter-0.5.7/oct_converter/readers/__init__.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-28 19:28:56.745235 oct_converter-0.5.7/oct_converter/readers/binary_structs/
--rw-r--r--   0 mark       (501) staff       (20)        0 2023-02-07 22:47:53.000000 oct_converter-0.5.7/oct_converter/readers/binary_structs/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)     3158 2023-01-17 16:31:46.000000 oct_converter-0.5.7/oct_converter/readers/binary_structs/boct_binary.py
--rw-r--r--   0 mark       (501) staff       (20)     2808 2023-02-23 22:38:19.000000 oct_converter-0.5.7/oct_converter/readers/binary_structs/e2e_binary.py
--rw-r--r--   0 mark       (501) staff       (20)     5718 2023-03-28 19:08:54.000000 oct_converter-0.5.7/oct_converter/readers/binary_structs/fda_binary.py
--rw-r--r--   0 mark       (501) staff       (20)     5566 2023-03-28 19:28:23.000000 oct_converter-0.5.7/oct_converter/readers/binary_structs/fds_binary.py
--rw-r--r--   0 mark       (501) staff       (20)     5046 2023-02-07 22:52:36.000000 oct_converter-0.5.7/oct_converter/readers/boct.py
--rw-r--r--   0 mark       (501) staff       (20)      816 2022-11-23 17:39:20.000000 oct_converter-0.5.7/oct_converter/readers/dicom.py
--rw-r--r--   0 mark       (501) staff       (20)    17218 2023-03-13 16:09:18.000000 oct_converter-0.5.7/oct_converter/readers/e2e.py
--rw-r--r--   0 mark       (501) staff       (20)    10335 2023-03-28 18:59:04.000000 oct_converter-0.5.7/oct_converter/readers/fda.py
--rw-r--r--   0 mark       (501) staff       (20)     7046 2023-03-28 19:28:23.000000 oct_converter-0.5.7/oct_converter/readers/fds.py
--rw-r--r--   0 mark       (501) staff       (20)     1793 2023-01-10 16:07:18.000000 oct_converter-0.5.7/oct_converter/readers/img.py
--rw-r--r--   0 mark       (501) staff       (20)     2535 2023-01-16 22:40:53.000000 oct_converter-0.5.7/oct_converter/readers/poct.py
--rw-r--r--   0 mark       (501) staff       (20)     6364 2023-01-29 19:59:01.000000 oct_converter-0.5.7/oct_converter/readers/zeissdicom.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-03-28 19:28:56.729516 oct_converter-0.5.7/oct_converter.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)     5958 2023-03-28 19:28:56.000000 oct_converter-0.5.7/oct_converter.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)     1208 2023-03-28 19:28:56.000000 oct_converter-0.5.7/oct_converter.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-03-28 19:28:56.000000 oct_converter-0.5.7/oct_converter.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-03-28 19:28:56.000000 oct_converter-0.5.7/oct_converter.egg-info/requires.txt
--rw-r--r--   0 mark       (501) staff       (20)       23 2023-03-28 19:28:56.000000 oct_converter-0.5.7/oct_converter.egg-info/top_level.txt
--rw-r--r--   0 mark       (501) staff       (20)     1289 2023-03-28 19:28:46.000000 oct_converter-0.5.7/pyproject.toml
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-03-28 19:28:56.746826 oct_converter-0.5.7/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)       50 2022-08-16 17:22:07.000000 oct_converter-0.5.7/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-04 18:11:46.408673 oct_converter-0.5.8/
+-rw-r--r--   0 mark       (501) staff       (20)     1069 2023-03-29 21:01:10.000000 oct_converter-0.5.8/LICENSE
+-rw-r--r--   0 mark       (501) staff       (20)       22 2023-03-29 21:01:10.000000 oct_converter-0.5.8/MANIFEST.in
+-rw-r--r--   0 mark       (501) staff       (20)     6074 2023-04-04 18:11:46.408254 oct_converter-0.5.8/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     4294 2023-03-29 21:01:10.000000 oct_converter-0.5.8/README.md
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-04 18:11:46.349502 oct_converter-0.5.8/examples/
+-rw-r--r--   0 mark       (501) staff       (20)      473 2023-03-29 21:01:10.000000 oct_converter-0.5.8/examples/demo_boct_extraction.py
+-rw-r--r--   0 mark       (501) staff       (20)      251 2023-03-29 21:01:10.000000 oct_converter-0.5.8/examples/demo_dicom_extraction.py
+-rw-r--r--   0 mark       (501) staff       (20)      613 2023-03-29 21:01:10.000000 oct_converter-0.5.8/examples/demo_e2e_extraction.py
+-rw-r--r--   0 mark       (501) staff       (20)     1136 2023-03-29 21:01:10.000000 oct_converter-0.5.8/examples/demo_fda_extraction.py
+-rw-r--r--   0 mark       (501) staff       (20)      952 2023-03-29 21:01:10.000000 oct_converter-0.5.8/examples/demo_fds_extraction.py
+-rw-r--r--   0 mark       (501) staff       (20)      304 2023-03-29 21:01:10.000000 oct_converter-0.5.8/examples/demo_img_extraction.py
+-rw-r--r--   0 mark       (501) staff       (20)      233 2023-03-29 21:01:10.000000 oct_converter-0.5.8/examples/demo_optovue_extraction.py
+-rw-r--r--   0 mark       (501) staff       (20)      402 2023-03-29 21:01:10.000000 oct_converter-0.5.8/examples/demo_zeissdicom_extraction.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-04 18:11:46.349895 oct_converter-0.5.8/oct_converter/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/__init__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-04 18:11:46.351585 oct_converter-0.5.8/oct_converter/exceptions/
+-rw-r--r--   0 mark       (501) staff       (20)      156 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/exceptions/__init__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-04 18:11:46.352910 oct_converter-0.5.8/oct_converter/image_types/
+-rw-r--r--   0 mark       (501) staff       (20)       83 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/image_types/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     1446 2023-03-29 21:04:12.000000 oct_converter-0.5.8/oct_converter/image_types/fundus.py
+-rw-r--r--   0 mark       (501) staff       (20)     5707 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/image_types/oct.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-04 18:11:46.404704 oct_converter-0.5.8/oct_converter/readers/
+-rw-r--r--   0 mark       (501) staff       (20)      190 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/__init__.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-04 18:11:46.407471 oct_converter-0.5.8/oct_converter/readers/binary_structs/
+-rw-r--r--   0 mark       (501) staff       (20)        0 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/binary_structs/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)     3158 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/binary_structs/boct_binary.py
+-rw-r--r--   0 mark       (501) staff       (20)     2808 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/binary_structs/e2e_binary.py
+-rw-r--r--   0 mark       (501) staff       (20)     5718 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/binary_structs/fda_binary.py
+-rw-r--r--   0 mark       (501) staff       (20)     5566 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/binary_structs/fds_binary.py
+-rw-r--r--   0 mark       (501) staff       (20)     5046 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/boct.py
+-rw-r--r--   0 mark       (501) staff       (20)      816 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/dicom.py
+-rw-r--r--   0 mark       (501) staff       (20)    18104 2023-04-04 18:04:58.000000 oct_converter-0.5.8/oct_converter/readers/e2e.py
+-rw-r--r--   0 mark       (501) staff       (20)    10416 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/fda.py
+-rw-r--r--   0 mark       (501) staff       (20)     7127 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/fds.py
+-rw-r--r--   0 mark       (501) staff       (20)     1793 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/img.py
+-rw-r--r--   0 mark       (501) staff       (20)     2535 2023-03-29 21:01:10.000000 oct_converter-0.5.8/oct_converter/readers/poct.py
+-rw-r--r--   0 mark       (501) staff       (20)     6364 2023-04-03 19:45:07.000000 oct_converter-0.5.8/oct_converter/readers/zeissdicom.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-04 18:11:46.351325 oct_converter-0.5.8/oct_converter.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)     6074 2023-04-04 18:11:46.000000 oct_converter-0.5.8/oct_converter.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)     1199 2023-04-04 18:11:46.000000 oct_converter-0.5.8/oct_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-04 18:11:46.000000 oct_converter-0.5.8/oct_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-04 18:11:46.000000 oct_converter-0.5.8/oct_converter.egg-info/requires.txt
+-rw-r--r--   0 mark       (501) staff       (20)       23 2023-04-04 18:11:46.000000 oct_converter-0.5.8/oct_converter.egg-info/top_level.txt
+-rw-r--r--   0 mark       (501) staff       (20)     1289 2023-04-04 18:05:22.000000 oct_converter-0.5.8/pyproject.toml
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-04 18:11:46.408802 oct_converter-0.5.8/setup.cfg
```

### Comparing `oct_converter-0.5.7/LICENSE` & `oct_converter-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/PKG-INFO` & `oct_converter-0.5.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oct_converter
-Version: 0.5.7
+Version: 0.5.8
 Summary: Extract OCT and fundus data from proprietary file formats.
 Author-email: Mark Graham <markgraham539@gmail.com>
 License: MIT License
         
         Copyright (c) 2021  Mark Graham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -83,58 +83,61 @@
 oct_volume.save('fds_testing.avi')  # save volume as a movie
 oct_volume.save('fds_testing.png')  # save volume as a set of sequential images, fds_testing_[1...N].png
 oct_volume.save_projection('projection.png') # save 2D projection
 
 fundus_image = fds.read_fundus_image()  # returns a  Fundus image with additional metadata if available
 fundus_image.save('fds_testing_fundus.jpg')
 
-# extract all other metadata
-metadata = fds.read_all_metadata(verbose=True)
+metadata = fds.read_all_metadata(verbose=True) # extracts all other metadata
 with open("fds_metadata.json", "w") as outfile:
     outfile.write(json.dumps(metadata, indent=4))
 ```
 
 ## Contributions
 Are welcome! Here is a [development roadmap](https://github.com/marksgraham/OCT-Converter/issues/86), including some easy first issues. Please open a [new issue](https://github.com/marksgraham/OCT-Converter/issues/new) to discuss any potential contributions.
 
 ## Updates
+28 March 2023
+- Metadata extraction for .fds expanded to match that of .fda file.
+
 31 January 2023
-- Greatly extended support for extracting metadata from .fda files
+- Greatly extended support for extracting metadata from .fda files.
 
 18 November 2022
 - Initial support for reading the Zeiss Dicom format.
 
 7 August 2022
 - Contours (layer segmentations) are now extracted from .e2e files.
 - Acquisition date is now extracted from .e2e files.
 
 16 June 2022
-- Initial support for reading Optovue OCTs
+- Initial support for reading Optovue OCTs.
 - Laterality is now extracted separately for each OCT/fundus image for .e2e files.
-- More patient info extracted from .e2e files (name, sex, birthdate, patient ID)
+- More patient info extracted from .e2e files (name, sex, birthdate, patient ID).
 
 24 Aug 2021
-- Reading the Bioptigen .OCT format is now supported
+- Reading the Bioptigen .OCT format is now supported/
 
 11 June 2021
 - Can now specify whether Zeiss .img data needs to be de-interlaced during reading.
 
 14 May 2021
 - Can save 2D projections of OCT volumes.
 
 30 October 2020
 - Extract fundus and laterality data from .e2e
-- Now attempts to extract additional volumetric data from .e2e files that was previously missed
+- Now attempts to extract additional volumetric data from .e2e files that was previously missed.
 
 22 August 2020
 - Experimental support for reading OCT data from .fda files.
 
 14 July 2020
 - Can now read fundus data from .fda files.
 
 ## Related projects
 - [uocte](https://bitbucket.org/uocte/uocte/wiki/Home) inspired and enabled this project
 - [LibE2E](https://github.com/neurodial/LibE2E) and [LibOctData](https://github.com/neurodial/LibOctData) provided some additional descriptions of the .e2e file spec
-- [eyepy](https://github.com/MedVisBonn/eyepy) can read HEYEY XML and VOL formats, and [eyelab](https://github.com/MedVisBonn/eyelab) is a tool for annotating this data
+- [eyepy](https://github.com/MedVisBonn/eyepy) for python-based import, visualisation, and analysis of OCT data
+- [eyelab](https://github.com/MedVisBonn/eyelab) is a tool for annotating this data
 
 ## Clinical use
 We can't guarantee images extracted with OCT-Converter will match those extracted or viewed with the manufacturer's software. Any use in clinical settings is at the user's own risk.
```

### Comparing `oct_converter-0.5.7/README.md` & `oct_converter-0.5.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,58 +47,61 @@
 oct_volume.save('fds_testing.avi')  # save volume as a movie
 oct_volume.save('fds_testing.png')  # save volume as a set of sequential images, fds_testing_[1...N].png
 oct_volume.save_projection('projection.png') # save 2D projection
 
 fundus_image = fds.read_fundus_image()  # returns a  Fundus image with additional metadata if available
 fundus_image.save('fds_testing_fundus.jpg')
 
-# extract all other metadata
-metadata = fds.read_all_metadata(verbose=True)
+metadata = fds.read_all_metadata(verbose=True) # extracts all other metadata
 with open("fds_metadata.json", "w") as outfile:
     outfile.write(json.dumps(metadata, indent=4))
 ```
 
 ## Contributions
 Are welcome! Here is a [development roadmap](https://github.com/marksgraham/OCT-Converter/issues/86), including some easy first issues. Please open a [new issue](https://github.com/marksgraham/OCT-Converter/issues/new) to discuss any potential contributions.
 
 ## Updates
+28 March 2023
+- Metadata extraction for .fds expanded to match that of .fda file.
+
 31 January 2023
-- Greatly extended support for extracting metadata from .fda files
+- Greatly extended support for extracting metadata from .fda files.
 
 18 November 2022
 - Initial support for reading the Zeiss Dicom format.
 
 7 August 2022
 - Contours (layer segmentations) are now extracted from .e2e files.
 - Acquisition date is now extracted from .e2e files.
 
 16 June 2022
-- Initial support for reading Optovue OCTs
+- Initial support for reading Optovue OCTs.
 - Laterality is now extracted separately for each OCT/fundus image for .e2e files.
-- More patient info extracted from .e2e files (name, sex, birthdate, patient ID)
+- More patient info extracted from .e2e files (name, sex, birthdate, patient ID).
 
 24 Aug 2021
-- Reading the Bioptigen .OCT format is now supported
+- Reading the Bioptigen .OCT format is now supported/
 
 11 June 2021
 - Can now specify whether Zeiss .img data needs to be de-interlaced during reading.
 
 14 May 2021
 - Can save 2D projections of OCT volumes.
 
 30 October 2020
 - Extract fundus and laterality data from .e2e
-- Now attempts to extract additional volumetric data from .e2e files that was previously missed
+- Now attempts to extract additional volumetric data from .e2e files that was previously missed.
 
 22 August 2020
 - Experimental support for reading OCT data from .fda files.
 
 14 July 2020
 - Can now read fundus data from .fda files.
 
 ## Related projects
 - [uocte](https://bitbucket.org/uocte/uocte/wiki/Home) inspired and enabled this project
 - [LibE2E](https://github.com/neurodial/LibE2E) and [LibOctData](https://github.com/neurodial/LibOctData) provided some additional descriptions of the .e2e file spec
-- [eyepy](https://github.com/MedVisBonn/eyepy) can read HEYEY XML and VOL formats, and [eyelab](https://github.com/MedVisBonn/eyelab) is a tool for annotating this data
+- [eyepy](https://github.com/MedVisBonn/eyepy) for python-based import, visualisation, and analysis of OCT data
+- [eyelab](https://github.com/MedVisBonn/eyelab) is a tool for annotating this data
 
 ## Clinical use
 We can't guarantee images extracted with OCT-Converter will match those extracted or viewed with the manufacturer's software. Any use in clinical settings is at the user's own risk.
```

### Comparing `oct_converter-0.5.7/examples/demo_e2e_extraction.py` & `oct_converter-0.5.8/examples/demo_e2e_extraction.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/examples/demo_fda_extraction.py` & `oct_converter-0.5.8/examples/demo_fda_extraction.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/examples/demo_fds_extraction.py` & `oct_converter-0.5.8/examples/demo_fds_extraction.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter/image_types/fundus.py` & `oct_converter-0.5.8/oct_converter/image_types/fundus.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         """Saves fundus image.
 
         Args:
             filepath (str): Location to save volume to. Extension must be in IMAGE_TYPES.
         """
         extension = os.path.splitext(filepath)[1]
         if extension.lower() in IMAGE_TYPES:
-            cv2.imwrite(filepath, self.image)
+            # change channel order from RGB to BGR and save with cv2
+            image = cv2.cvtColor(self.image, cv2.COLOR_RGB2BGR)
+            cv2.imwrite(filepath, image)
         elif extension.lower() == ".npy":
             np.save(filepath, self.image)
         else:
             raise NotImplementedError(
                 "Saving with file extension {} not supported".format(extension)
             )
```

### Comparing `oct_converter-0.5.7/oct_converter/image_types/oct.py` & `oct_converter-0.5.8/oct_converter/image_types/oct.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter/readers/binary_structs/boct_binary.py` & `oct_converter-0.5.8/oct_converter/readers/binary_structs/boct_binary.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter/readers/binary_structs/e2e_binary.py` & `oct_converter-0.5.8/oct_converter/readers/binary_structs/e2e_binary.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter/readers/binary_structs/fda_binary.py` & `oct_converter-0.5.8/oct_converter/readers/binary_structs/fda_binary.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter/readers/binary_structs/fds_binary.py` & `oct_converter-0.5.8/oct_converter/readers/binary_structs/fds_binary.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter/readers/boct.py` & `oct_converter-0.5.8/oct_converter/readers/boct.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter/readers/dicom.py` & `oct_converter-0.5.8/oct_converter/readers/dicom.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter/readers/e2e.py` & `oct_converter-0.5.8/oct_converter/readers/e2e.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 
         self.power = pow(2, 10)
         self.sex = None
         self.first_name = None
         self.surname = None
         self.acquisition_date = None
 
-    def read_oct_volume(self):
+    def read_oct_volume(self, legacy_intensity_transform=False):
         """Reads OCT data.
+        Args:
+            legacy_intensity_transform (bool): If True, use intensity transform used in v<=0.5.7. Defaults to False.
 
         Returns:
             obj:OCTVolumeWithMetaData
         """
 
         def _make_lut():
             LUT = []
@@ -198,15 +200,18 @@
                                     f"{len(LUT[raw_volume])} elements into a "
                                     f"{image_data.width}x"
                                     f"{image_data.height} array"
                                 ),
                                 UserWarning,
                             )
                         else:
-                            image = 256 * pow(image, 1.0 / 2.4)
+                            if legacy_intensity_transform:
+                                image = pow(image, 1.0 / 2.4)
+                            else:
+                                image = self.vol_intensity_transform(image)
 
                             if volume_string in volume_array_dict.keys():
                                 volume_array_dict[volume_string][
                                     int(chunk.slice_id / 2) - 1
                                 ] = image
                             else:
                                 # try to capture these additional images
@@ -408,7 +413,22 @@
         exponent = exponent[::-1]
 
         # convert to decimal representations
         mantissa_sum = 1 + int(mantissa, 2) / self.power
         exponent_sum = int(exponent, 2) - 63
         decimal_value = mantissa_sum * np.float_power(2, exponent_sum)
         return decimal_value
+
+    def vol_intensity_transform(self, data):
+        """Implementation of intensity transform used in .e2e files. Code thanks to @oli4, see discussion in
+        https://github.com/marksgraham/OCT-Converter/issues/21#issuecomment-1057455183
+        """
+        selection_0 = data == np.finfo(np.float32).max
+        selection_data = data <= 1
+
+        new = np.log(data[selection_data] + 2.44e-04)
+        new = (new + 8.3) / 8.285
+
+        data[selection_data] = new
+        data[selection_0] = 0
+        data = np.clip(data, 0, 1)
+        return data
```

### Comparing `oct_converter-0.5.7/oct_converter/readers/fda.py` & `oct_converter-0.5.8/oct_converter/readers/fda.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,16 @@
             f.seek(chunk_location)  # Set the chunk’s current position.
             raw = f.read(24)  # skip 24 is important
             fundus_header = fda_binary.fundus_header.parse(raw)
             number_pixels = fundus_header.width * fundus_header.height * 3
             raw_image = f.read(fundus_header.size)
             image = Image.open(io.BytesIO(raw_image))
             image = np.asarray(image)
+            # store with RGB channel order
+            image = np.flip(image, 2)
         fundus_image = FundusImageWithMetaData(image)
         return fundus_image
 
     def read_fundus_image_gray_scale(self):
         """Reads gray scale fundus image.
 
         Returns:
```

### Comparing `oct_converter-0.5.7/oct_converter/readers/fds.py` & `oct_converter-0.5.8/oct_converter/readers/fds.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,16 @@
             # raw_image = [struct.unpack('B', f.read(1)) for pixel in range(fundus_header.size)]
             image = np.array(raw_image)
             image = image.reshape(
                 3, fundus_header.width, fundus_header.height, order="F"
             )
             image = np.transpose(image, [2, 1, 0])
             image = image.astype(np.float32)
+            # store with RGB channel order
+            image = np.flip(image, 2)
         fundus_image = FundusImageWithMetaData(image)
         return fundus_image
 
     def read_all_metadata(self, verbose=False):
         """
         Reads all available metadata and returns a dictionary.
```

### Comparing `oct_converter-0.5.7/oct_converter/readers/img.py` & `oct_converter-0.5.8/oct_converter/readers/img.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter/readers/poct.py` & `oct_converter-0.5.8/oct_converter/readers/poct.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter/readers/zeissdicom.py` & `oct_converter-0.5.8/oct_converter/readers/zeissdicom.py`

 * *Files identical despite different names*

### Comparing `oct_converter-0.5.7/oct_converter.egg-info/PKG-INFO` & `oct_converter-0.5.8/oct_converter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oct-converter
-Version: 0.5.7
+Version: 0.5.8
 Summary: Extract OCT and fundus data from proprietary file formats.
 Author-email: Mark Graham <markgraham539@gmail.com>
 License: MIT License
         
         Copyright (c) 2021  Mark Graham
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -83,58 +83,61 @@
 oct_volume.save('fds_testing.avi')  # save volume as a movie
 oct_volume.save('fds_testing.png')  # save volume as a set of sequential images, fds_testing_[1...N].png
 oct_volume.save_projection('projection.png') # save 2D projection
 
 fundus_image = fds.read_fundus_image()  # returns a  Fundus image with additional metadata if available
 fundus_image.save('fds_testing_fundus.jpg')
 
-# extract all other metadata
-metadata = fds.read_all_metadata(verbose=True)
+metadata = fds.read_all_metadata(verbose=True) # extracts all other metadata
 with open("fds_metadata.json", "w") as outfile:
     outfile.write(json.dumps(metadata, indent=4))
 ```
 
 ## Contributions
 Are welcome! Here is a [development roadmap](https://github.com/marksgraham/OCT-Converter/issues/86), including some easy first issues. Please open a [new issue](https://github.com/marksgraham/OCT-Converter/issues/new) to discuss any potential contributions.
 
 ## Updates
+28 March 2023
+- Metadata extraction for .fds expanded to match that of .fda file.
+
 31 January 2023
-- Greatly extended support for extracting metadata from .fda files
+- Greatly extended support for extracting metadata from .fda files.
 
 18 November 2022
 - Initial support for reading the Zeiss Dicom format.
 
 7 August 2022
 - Contours (layer segmentations) are now extracted from .e2e files.
 - Acquisition date is now extracted from .e2e files.
 
 16 June 2022
-- Initial support for reading Optovue OCTs
+- Initial support for reading Optovue OCTs.
 - Laterality is now extracted separately for each OCT/fundus image for .e2e files.
-- More patient info extracted from .e2e files (name, sex, birthdate, patient ID)
+- More patient info extracted from .e2e files (name, sex, birthdate, patient ID).
 
 24 Aug 2021
-- Reading the Bioptigen .OCT format is now supported
+- Reading the Bioptigen .OCT format is now supported/
 
 11 June 2021
 - Can now specify whether Zeiss .img data needs to be de-interlaced during reading.
 
 14 May 2021
 - Can save 2D projections of OCT volumes.
 
 30 October 2020
 - Extract fundus and laterality data from .e2e
-- Now attempts to extract additional volumetric data from .e2e files that was previously missed
+- Now attempts to extract additional volumetric data from .e2e files that was previously missed.
 
 22 August 2020
 - Experimental support for reading OCT data from .fda files.
 
 14 July 2020
 - Can now read fundus data from .fda files.
 
 ## Related projects
 - [uocte](https://bitbucket.org/uocte/uocte/wiki/Home) inspired and enabled this project
 - [LibE2E](https://github.com/neurodial/LibE2E) and [LibOctData](https://github.com/neurodial/LibOctData) provided some additional descriptions of the .e2e file spec
-- [eyepy](https://github.com/MedVisBonn/eyepy) can read HEYEY XML and VOL formats, and [eyelab](https://github.com/MedVisBonn/eyelab) is a tool for annotating this data
+- [eyepy](https://github.com/MedVisBonn/eyepy) for python-based import, visualisation, and analysis of OCT data
+- [eyelab](https://github.com/MedVisBonn/eyelab) is a tool for annotating this data
 
 ## Clinical use
 We can't guarantee images extracted with OCT-Converter will match those extracted or viewed with the manufacturer's software. Any use in clinical settings is at the user's own risk.
```

### Comparing `oct_converter-0.5.7/oct_converter.egg-info/SOURCES.txt` & `oct_converter-0.5.8/oct_converter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.py
 examples/demo_boct_extraction.py
 examples/demo_dicom_extraction.py
 examples/demo_e2e_extraction.py
 examples/demo_fda_extraction.py
 examples/demo_fds_extraction.py
 examples/demo_img_extraction.py
 examples/demo_optovue_extraction.py
```

### Comparing `oct_converter-0.5.7/pyproject.toml` & `oct_converter-0.5.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "oct_converter"
-version = "0.5.7"
+version = "0.5.8"
 description = "Extract OCT and fundus data from proprietary file formats."
 readme = "README.md"
 authors = [{ name = "Mark Graham", email = "markgraham539@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -35,15 +35,15 @@
 
 [tool.setuptools.packages.find]
 where = [""]
 include = ["oct_converter*","examples"]
 exclude= ["my_example_volumes*"]
 
 [tool.bumpver]
-current_version = "0.5.7"
+current_version = "0.5.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

