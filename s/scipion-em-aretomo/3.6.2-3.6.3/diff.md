# Comparing `tmp/scipion-em-aretomo-3.6.2.tar.gz` & `tmp/scipion-em-aretomo-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-aretomo-3.6.2.tar", last modified: Sun Mar 12 19:53:18 2023, max compression
+gzip compressed data, was "scipion-em-aretomo-3.6.3.tar", last modified: Sat Apr  8 16:18:19 2023, max compression
```

## Comparing `scipion-em-aretomo-3.6.2.tar` & `scipion-em-aretomo-3.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 19:53:18.702351 scipion-em-aretomo-3.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-03-12 19:53:18.702351 scipion-em-aretomo-3.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 19:53:18.698351 scipion-em-aretomo-3.6.2/aretomo/
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/aretomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/aretomo/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/aretomo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/aretomo/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 19:53:18.702351 scipion-em-aretomo-3.6.2/aretomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/aretomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28569 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/aretomo/protocols/protocol_aretomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/aretomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 19:53:18.702351 scipion-em-aretomo-3.6.2/aretomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/aretomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/aretomo/tests/test_protocols_aretomo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 19:53:18.702351 scipion-em-aretomo-3.6.2/scipion_em_aretomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-03-12 19:53:18.000000 scipion-em-aretomo-3.6.2/scipion_em_aretomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-12 19:53:18.000000 scipion-em-aretomo-3.6.2/scipion_em_aretomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 19:53:18.000000 scipion-em-aretomo-3.6.2/scipion_em_aretomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-12 19:53:18.000000 scipion-em-aretomo-3.6.2/scipion_em_aretomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-12 19:53:18.000000 scipion-em-aretomo-3.6.2/scipion_em_aretomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-12 19:53:18.000000 scipion-em-aretomo-3.6.2/scipion_em_aretomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 19:53:18.702351 scipion-em-aretomo-3.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-03-12 19:51:35.000000 scipion-em-aretomo-3.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/aretomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/aretomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28337 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/protocols/protocol_aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/aretomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/aretomo/tests/test_protocols_aretomo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-08 16:18:19.000000 scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:18:19.669469 scipion-em-aretomo-3.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-04-08 16:16:33.000000 scipion-em-aretomo-3.6.3/setup.py
```

### Comparing `scipion-em-aretomo-3.6.2/CHANGES.txt` & `scipion-em-aretomo-3.6.3/CHANGES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+3.6.3: reduce number of Set[item] calls
 3.6.2:
  - fix applyTransform in the convert step
  - add interpolated flag
 3.6.1:
  - add aretomo 1.3.4, remove support for versions < 1.1.0
  - fix alignment matrix for excluded TS views
 3.6:
```

### Comparing `scipion-em-aretomo-3.6.2/LICENSE` & `scipion-em-aretomo-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.2/PKG-INFO` & `scipion-em-aretomo-3.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-aretomo
-Version: 3.6.2
+Version: 3.6.3
 Summary: Plugin to use AreTomo program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-aretomo
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-aretomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-aretomo/
```

### Comparing `scipion-em-aretomo-3.6.2/README.rst` & `scipion-em-aretomo-3.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.2/aretomo/__init__.py` & `scipion-em-aretomo-3.6.3/aretomo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,35 +28,35 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
 
-__version__ = '3.6.2'
+__version__ = '3.6.3'
 _logo = "aretomo_logo.png"
 _references = ['Zheng2022']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = ARETOMO_HOME
     _pathVars = [ARETOMO_HOME, ARETOMO_CUDA_LIB]
     _supportedVersions = [V1_1_0, V1_1_1, V1_2_0, V1_2_5,
                           V1_3_0, V1_3_3, V1_3_4]
     _url = "https://github.com/scipion-em/scipion-em-aretomo"
 
     @classmethod
     def _defineVariables(cls):
-        cls._defineEmVar(ARETOMO_HOME, 'aretomo-%s' % V1_3_4)
+        cls._defineEmVar(ARETOMO_HOME, f'aretomo-{V1_3_4}')
         cls._defineVar(ARETOMO_CUDA_LIB, pwem.Config.CUDA_LIB)
 
         # Define the variable default value based on the guessed cuda version
         cudaVersion = cls.guessCudaVersion(ARETOMO_CUDA_LIB)
-        cls._defineVar(ARETOMO_BIN, 'AreTomo_1.3.4_Cuda%s%s_Feb22_2023' % (
-            cudaVersion.major, cudaVersion.minor))
+        cls._defineVar(ARETOMO_BIN,
+                       f'AreTomo_1.3.4_Cuda{cudaVersion.major}{cudaVersion.minor}_Feb22_2023')
 
     @classmethod
     def getEnviron(cls):
         """ Return the environment to run AreTomo. """
         environ = pwutils.Environ(os.environ)
         # Get AreTomo CUDA library path if defined
         cudaLib = cls.getVar(ARETOMO_CUDA_LIB, pwem.Config.CUDA_LIB)
@@ -84,9 +84,9 @@
         """ Return the program binary that will be used. """
         return cls.getHome('bin', cls.getVar(ARETOMO_BIN))
 
     @classmethod
     def defineBinaries(cls, env):
         for v in cls._supportedVersions:
             env.addPackage('aretomo', version=v,
-                           tar='aretomo_v%s.tgz' % v,
+                           tar=f"aretomo_v{v}.tgz",
                            default=v == V1_3_4)
```

### Comparing `scipion-em-aretomo-3.6.2/aretomo/bibtex.py` & `scipion-em-aretomo-3.6.3/aretomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.2/aretomo/constants.py` & `scipion-em-aretomo-3.6.3/aretomo/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,18 +25,14 @@
 # **************************************************************************
 
 ARETOMO_BIN = 'ARETOMO_BIN'
 ARETOMO_HOME = 'ARETOMO_HOME'
 ARETOMO_CUDA_LIB = 'ARETOMO_CUDA_LIB'
 
 # Supported versions
-V1_0_6 = '1.0.6'
-V1_0_8 = '1.0.8'
-V1_0_10 = '1.0.10'
-V1_0_12 = '1.0.12'
 V1_1_0 = '1.1.0'
 V1_1_1 = '1.1.1'
 V1_2_0 = '1.2.0'
 V1_2_5 = '1.2.5'
 V1_3_0 = '1.3.0'
 V1_3_3 = '1.3.3'
 V1_3_4 = '1.3.4'
```

### Comparing `scipion-em-aretomo-3.6.2/aretomo/convert.py` & `scipion-em-aretomo-3.6.3/aretomo/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.2/aretomo/protocols/__init__.py` & `scipion-em-aretomo-3.6.3/aretomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.2/aretomo/protocols/protocol_aretomo.py` & `scipion-em-aretomo-3.6.3/aretomo/protocols/protocol_aretomo.py`

 * *Files 5% similar despite different names*

```diff
@@ -247,63 +247,66 @@
 
         form.addHidden(params.GPU_LIST, params.StringParam,
                        default='0', label="Choose GPU IDs")
 
     # --------------------------- INSERT steps functions ----------------------
     def _insertAllSteps(self):
         for ts in self.inputSetOfTiltSeries.get():
-            self._insertFunctionStep('convertInputStep', ts.getObjId())
-            self._insertFunctionStep('runAreTomoStep', ts.getObjId())
-            self._insertFunctionStep('createOutputStep', ts.getObjId())
-        self._insertFunctionStep('closeOutputSetsStep')
+            tsObjId = ts.getObjId()
+            self._insertFunctionStep(self.convertInputStep, tsObjId)
+            self._insertFunctionStep(self.runAreTomoStep, tsObjId)
+            self._insertFunctionStep(self.createOutputStep, tsObjId)
+        self._insertFunctionStep(self.closeOutputSetsStep)
 
     # --------------------------- STEPS functions -----------------------------
     def convertInputStep(self, tsObjId):
         ts = self._getSetOfTiltSeries()[tsObjId]
         tsId = ts.getTsId()
+        tsFn = ts.getFirstItem().getFileName()
         extraPrefix = self._getExtraPath(tsId)
         tmpPrefix = self._getTmpPath(tsId)
         pwutils.makePath(tmpPrefix)
         pwutils.makePath(extraPrefix)
 
         # Apply the transformation for the input tilt-series
-        outputTsFileName = self.getFilePath(tsObjId, tmpPrefix, ".mrc")
+        outputTsFileName = self.getFilePath(tsFn, tmpPrefix, ".mrc")
         rotationAngle = ts.getAcquisition().getTiltAxisAngle()
         doSwap = 45 < abs(rotationAngle) < 135
         ts.applyTransform(outputTsFileName, swapXY=doSwap)
 
         # Generate angle file
-        angleFilePath = self.getFilePath(tsObjId, tmpPrefix, ".tlt")
+        angleFilePath = self.getFilePath(tsFn, tmpPrefix, ".tlt")
         self._generateTltFile(ts, angleFilePath)
 
         if self.useInputProt:
             # Find and copy aln file
             protExtra = self.inputProt.get()._getExtraPath(tsId)
-            protAlnBase = self.getFilePath(tsObjId, protExtra, ".aln").replace("_even", "*").replace("_odd", "*")
+            protAlnBase = self.getFilePath(tsFn, protExtra, ".aln").replace("_even", "*").replace("_odd", "*")
             protAln = glob(protAlnBase)
             if len(protAln):
                 pwutils.copyFile(protAln[0],
-                                 self.getFilePath(tsObjId, extraPrefix, ".aln"))
-                self.info("Using input alignment: %s" % protAln[0])
+                                 self.getFilePath(tsFn, extraPrefix, ".aln"))
+                self.info(f"Using input alignment: {protAln[0]}")
             else:
                 raise FileNotFoundError("Missing input aln file ", protAlnBase)
 
     def runAreTomoStep(self, tsObjId):
         """ Call AreTomo with the appropriate parameters. """
         tsSet = self._getSetOfTiltSeries()
         ts = tsSet[tsObjId]
         tsId = ts.getTsId()
+        tsFn = ts.getFirstItem().getFileName()
 
         extraPrefix = self._getExtraPath(tsId)
         tmpPrefix = self._getTmpPath(tsId)
 
         args = {
-            '-InMrc': self.getFilePath(tsObjId, tmpPrefix, ".mrc"),
-            '-OutMrc': self.getFilePath(tsObjId, extraPrefix, ".mrc"),
-            '-AngFile': self.getFilePath(tsObjId, tmpPrefix, ".tlt"),
+            '-InMrc': self.getFilePath(tsFn, tmpPrefix, ".mrc"),
+            '-OutMrc': self.getFilePath(tsFn, extraPrefix, ".mrc"),
+            '-AngFile': self.getFilePath(tsFn, tmpPrefix, ".tlt"),
             '-VolZ': self.tomoThickness if self.makeTomo else 0,
             '-OutBin': self.binFactor,
             '-FlipInt': 1 if self.flipInt else 0,
             '-FlipVol': 1 if self.makeTomo and self.flipVol else 0,
             '-PixSize': tsSet.getSamplingRate(),
             '-Kv': tsSet.getAcquisition().getVoltage(),
             '-Cs': tsSet.getAcquisition().getSphericalAberration(),
@@ -312,62 +315,62 @@
             '-Gpu': '%(GPU)s'
         }
 
         if not self.useInputProt:
             args['-Align'] = 0 if self.skipAlign else 1
 
             tiltAxisAngle = ts.getAcquisition().getTiltAxisAngle() or 0.0
-            if ts.getFirstItem().hasTransform():
+            if ts.hasAlignment():
                 # in this case we already used ts.applyTransform()
                 tiltAxisAngle = 0.0
 
-            args['-TiltAxis'] = "%s %s" % (tiltAxisAngle,
-                                           self.refineTiltAxis.get() - 1)
-            args['-TiltCor'] = "%s" % (self.refineTiltAngles.get() - 1)
+            args['-TiltAxis'] = f"{tiltAxisAngle} {self.refineTiltAxis.get() - 1}"
+            args['-TiltCor'] = self.refineTiltAngles.get() - 1
 
             if not self.skipAlign:
                 args['-AlignZ'] = self.alignZ
 
             if self.sampleType.get() == LOCAL_MOTION_COORDS:
                 args['-RoiFile'] = self.coordsFn
             elif self.sampleType.get() == LOCAL_MOTION_PATCHES:
-                args['-Patch'] = '%d %d' % (self.patchX, self.patchY)
+                args['-Patch'] = f"{self.patchX} {self.patchY}"
 
             if self.roiArea.get():
                 args['-Roi'] = self.roiArea.get()
 
         else:
-            args['-AlnFile'] = self.getFilePath(tsObjId, extraPrefix, ".aln")
+            args['-AlnFile'] = self.getFilePath(tsFn, extraPrefix, ".aln")
 
         if self.reconMethod == RECON_SART:
-            args['-Sart'] = '%d %d' % (self.SARTiter, self.SARTproj)
+            args['-Sart'] = f"{self.SARTiter} {self.SARTproj}"
         else:
             args['-Wbp'] = 1
 
-        param = ' '.join(['%s %s' % (k, str(v)) for k, v in args.items()])
+        param = ' '.join([f'{k} {str(v)}' for k, v in args.items()])
         param += ' ' + self.extraParams.get()
         program = Plugin.getProgram()
 
         self.runJob(program, param, env=Plugin.getEnviron())
 
     def createOutputStep(self, tsObjId):
         ts = self._getSetOfTiltSeries()[tsObjId]
         tsId = ts.getTsId()
+        tsFn = ts.getFirstItem().getFileName()
         extraPrefix = self._getExtraPath(tsId)
 
         if not (self.makeTomo and self.skipAlign):
             sec_nums, imod_matrix, tilt_angs, tilt_axes = readAlnFile(
-                self.getFilePath(tsObjId, extraPrefix, ".aln"),
+                self.getFilePath(tsFn, extraPrefix, ".aln"),
                 newVersion=Plugin.versionGE("1.3.0"))
             alignmentMatrix = getTransformationMatrix(imod_matrix)
 
         if self.makeTomo:
             outputSetOfTomograms = self.getOutputSetOfTomograms()
             newTomogram = Tomogram()
-            newTomogram.setLocation(self.getFilePath(tsObjId, extraPrefix, ".mrc"))
+            newTomogram.setLocation(self.getFilePath(tsFn, extraPrefix, ".mrc"))
 
             # Set tomogram origin
             origin = Transform()
             sr = self._getOutputSampling()
             origin.setShifts(ts.getFirstItem().getXDim() / -2. * sr,
                              ts.getFirstItem().getYDim() / -2. * sr,
                              self.tomoThickness.get() / self.binFactor.get() / -2 * sr)
@@ -396,15 +399,15 @@
 
                         acq = tiltImage.getAcquisition()
                         acq.setTiltAxisAngle(0.)
                         newTi.setAcquisition(acq)
 
                         newTi.setTiltAngle(tilt_angs[sec_nums.index(secNum)])
                         newTi.setLocation(sec_nums.index(secNum) + 1,
-                                          (self.getFilePath(tsObjId, extraPrefix, ".mrc")))
+                                          (self.getFilePath(tsFn, extraPrefix, ".mrc")))
                         newTi.setSamplingRate(self._getOutputSampling())
                         newTs.append(newTi)
                         accumDose = acq.getAccumDose()
 
                 acq = newTs.getAcquisition()
                 acq.setAccumDose(accumDose)  # set accum dose from the last tilt-image
                 acq.setTiltAxisAngle(0.)  # 0 because TS is aligned
@@ -416,15 +419,15 @@
                 newTs.write(properties=False)
 
                 outTsAligned.update(newTs)
                 outTsAligned.write()
                 self._store(outTsAligned)
             else:
                 # remove aligned stack from output
-                pwutils.cleanPath(self.getFilePath(tsObjId, extraPrefix, ".mrc"))
+                pwutils.cleanPath(self.getFilePath(tsFn, extraPrefix, ".mrc"))
 
         # Save original TS stack with new alignment,
         # unless making a tomo from pre-aligned TS
         if not (self.makeTomo and self.skipAlign):
             outputSetOfTiltSeries = self.getOutputSetOfTiltSeries(OUT_TS)
             newTs = ts.clone()
             newTs.copyInfo(ts)
@@ -464,36 +467,33 @@
             newTs.setDim(self._getSetOfTiltSeries().getDim())
             newTs.write(properties=False)
 
             outputSetOfTiltSeries.update(newTs)
             outputSetOfTiltSeries.write()
             self._store(outputSetOfTiltSeries)
 
-        self._store()
-
     def closeOutputSetsStep(self):
-        if not (self.makeTomo and self.skipAlign):
-            self.getOutputSetOfTiltSeries(OUT_TS).setStreamState(Set.STREAM_CLOSED)
-        if self.makeTomo:
-            self.getOutputSetOfTomograms().setStreamState(Set.STREAM_CLOSED)
-        elif self._saveInterpolated():
-            self.getOutputSetOfTiltSeries(OUT_TS_ALN).setStreamState(Set.STREAM_CLOSED)
+        for _, outputset in self.iterOutputAttributes():
+            outputset.setStreamState(Set.STREAM_CLOSED)
+
         self._store()
 
     # --------------------------- INFO functions ------------------------------
     def _summary(self):
         summary = []
         if hasattr(self, OUT_TOMO):
-            summary.append("Input Tilt-Series: %d.\nTomograms reconstructed: %d.\n"
-                           % (self._getSetOfTiltSeries().getSize(),
-                              self.outputSetOfTomograms.getSize()))
+            summary.append(f"Input tilt-series: "
+                           f"{self._getSetOfTiltSeries().getSize()}.\n"
+                           f"Tomograms reconstructed: "
+                           f"{self.outputSetOfTomograms.getSize()}.\n")
         elif hasattr(self, OUT_TS):
-            summary.append("Input Tilt-Series: %d.\nTilt series aligned: %d.\n"
-                           % (self._getSetOfTiltSeries().getSize(),
-                              self.outputSetOfTiltSeries.getSize()))
+            summary.append(f"Input tilt-series: "
+                           f"{self._getSetOfTiltSeries().getSize()}.\n"
+                           f"Tilt series aligned: "
+                           f"{self.outputSetOfTiltSeries.getSize()}")
         else:
             summary.append("Output is not ready yet.")
 
         if self._saveInterpolated() and not self.makeTomo:
             summary.append("*Interpolated TS stack may have a few "
                            "dark tilt images removed.*")
 
@@ -517,26 +517,28 @@
                 errors.append("Z volume height for alignment should be always "
                               "smaller than tomogram thickness.")
 
         if self.skipAlign and not self.makeTomo:
             errors.append("You cannot switch off both alignment and "
                           "reconstruction.")
 
-        tr = self._getSetOfTiltSeries().getFirstItem().getFirstItem().hasTransform()
-        if tr and not self.skipAlign:
+        if self._getSetOfTiltSeries().hasAlignment() and not self.skipAlign:
             errors.append("Input tilt-series already have alignment "
                           "information. You probably want to skip alignment step.")
 
         return errors
     
     # --------------------------- UTILS functions -----------------------------
-    def getFilePath(self, tsObjId, prefix, ext=None):
-        ts = self._getSetOfTiltSeries()[tsObjId]
-        return os.path.join(prefix,
-                            ts.getFirstItem().parseFileName(extension=ext))
+    def getFilePath(self, tsFn, prefix, ext=None):
+        fileName, fileExtension = os.path.splitext(os.path.basename(tsFn))
+
+        if ext is not None:
+            fileExtension = ext
+
+        return os.path.join(prefix, fileName + fileExtension)
 
     def getOutputSetOfTomograms(self):
         if hasattr(self, OUT_TOMO):
             self.outputSetOfTomograms.enableAppend()
         else:
             outputSetOfTomograms = self._createSetOfTomograms()
             outputSetOfTomograms.copyInfo(self._getSetOfTiltSeries())
@@ -566,34 +568,30 @@
                                        outputSetOfTiltSeries)
         return getattr(self, outputName)
 
     def _getSetOfTiltSeries(self):
         return self.inputSetOfTiltSeries.get()
 
     def _getOutputSampling(self):
-        return self._getSetOfTiltSeries().getSamplingRate() * self.binFactor.get()
+        return self._getInputSampling() * self.binFactor.get()
 
     def _getInputSampling(self):
         return self._getSetOfTiltSeries().getSamplingRate()
 
     def _getOutputDim(self, fn):
         ih = ImageHandler()
         x, y, z, _ = ih.getDimensions(fn)
         return (x, y, z)
 
     def _generateTltFile(self, ts, outputFn):
         """ Generate .tlt file with tilt angles and accumulated dose. """
-        angleList = []
-
-        for ti in ts.iterItems():
-            accDose = ti.getAcquisition().getAccumDose()
-            tAngle = ti.getTiltAngle()
-            angleList.append((tAngle, accDose))
+        tsParams = ts.aggregate(["COUNT"], "_tiltAngle",
+                                ["_tiltAngle", "_acquisition._accumDose"])
 
         with open(outputFn, 'w') as f:
             if self.doDW:
-                f.writelines(f"{i[0]:0.3f} {i[1]:0.3f}\n" for i in angleList)
+                f.writelines(f"{i['_tiltAngle']:0.3f} {i['_acquisition._accumDose']:0.3f}\n" for i in tsParams)
             else:
-                f.writelines(f"{i[0]:0.3f}\n" for i in angleList)
+                f.writelines(f"{i['_tiltAngle']:0.3f}\n" for i in tsParams)
 
     def _saveInterpolated(self):
         return self.saveStack
```

### Comparing `scipion-em-aretomo-3.6.2/aretomo/protocols.conf` & `scipion-em-aretomo-3.6.3/aretomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.2/aretomo/tests/__init__.py` & `scipion-em-aretomo-3.6.3/aretomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.2/aretomo/tests/test_protocols_aretomo.py` & `scipion-em-aretomo-3.6.3/aretomo/tests/test_protocols_aretomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.2/scipion_em_aretomo.egg-info/PKG-INFO` & `scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-aretomo
-Version: 3.6.2
+Version: 3.6.3
 Summary: Plugin to use AreTomo program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-aretomo
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-aretomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-aretomo/
```

### Comparing `scipion-em-aretomo-3.6.2/scipion_em_aretomo.egg-info/SOURCES.txt` & `scipion-em-aretomo-3.6.3/scipion_em_aretomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.6.2/setup.py` & `scipion-em-aretomo-3.6.3/setup.py`

 * *Files identical despite different names*

