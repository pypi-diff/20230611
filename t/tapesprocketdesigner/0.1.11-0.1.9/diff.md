# Comparing `tmp/tapesprocketdesigner-0.1.11.tar.gz` & `tmp/tapesprocketdesigner-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapesprocketdesigner-0.1.11.tar", last modified: Sun Jun 11 12:48:57 2023, max compression
+gzip compressed data, was "tapesprocketdesigner-0.1.9.tar", last modified: Sat Jun 10 18:57:27 2023, max compression
```

## Comparing `tapesprocketdesigner-0.1.11.tar` & `tapesprocketdesigner-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 niels     (1000) niels     (1000)        0 2023-06-11 12:48:57.695581 tapesprocketdesigner-0.1.11/
--rw-rw-r--   0 niels     (1000) niels     (1000)    35149 2023-06-10 15:38:35.000000 tapesprocketdesigner-0.1.11/LICENSE
--rw-rw-r--   0 niels     (1000) niels     (1000)    47955 2023-06-11 12:48:57.695581 tapesprocketdesigner-0.1.11/PKG-INFO
--rw-rw-r--   0 niels     (1000) niels     (1000)     6786 2023-06-11 12:48:46.000000 tapesprocketdesigner-0.1.11/README.md
--rw-rw-r--   0 niels     (1000) niels     (1000)     1152 2023-06-11 12:48:26.000000 tapesprocketdesigner-0.1.11/pyproject.toml
--rw-rw-r--   0 niels     (1000) niels     (1000)       38 2023-06-11 12:48:57.695581 tapesprocketdesigner-0.1.11/setup.cfg
-drwxrwxr-x   0 niels     (1000) niels     (1000)        0 2023-06-11 12:48:57.695581 tapesprocketdesigner-0.1.11/tapesprocketdesigner/
--rw-rw-r--   0 niels     (1000) niels     (1000)        0 2023-06-10 17:58:57.000000 tapesprocketdesigner-0.1.11/tapesprocketdesigner/__init__.py
--rwxrwxr-x   0 niels     (1000) niels     (1000)    15665 2023-06-11 12:46:51.000000 tapesprocketdesigner-0.1.11/tapesprocketdesigner/designer.py
-drwxrwxr-x   0 niels     (1000) niels     (1000)        0 2023-06-11 12:48:57.695581 tapesprocketdesigner-0.1.11/tapesprocketdesigner.egg-info/
--rw-rw-r--   0 niels     (1000) niels     (1000)    47955 2023-06-11 12:48:57.000000 tapesprocketdesigner-0.1.11/tapesprocketdesigner.egg-info/PKG-INFO
--rw-rw-r--   0 niels     (1000) niels     (1000)      364 2023-06-11 12:48:57.000000 tapesprocketdesigner-0.1.11/tapesprocketdesigner.egg-info/SOURCES.txt
--rw-rw-r--   0 niels     (1000) niels     (1000)        1 2023-06-11 12:48:57.000000 tapesprocketdesigner-0.1.11/tapesprocketdesigner.egg-info/dependency_links.txt
--rw-rw-r--   0 niels     (1000) niels     (1000)       76 2023-06-11 12:48:57.000000 tapesprocketdesigner-0.1.11/tapesprocketdesigner.egg-info/entry_points.txt
--rw-rw-r--   0 niels     (1000) niels     (1000)       14 2023-06-11 12:48:57.000000 tapesprocketdesigner-0.1.11/tapesprocketdesigner.egg-info/requires.txt
--rw-rw-r--   0 niels     (1000) niels     (1000)       21 2023-06-11 12:48:57.000000 tapesprocketdesigner-0.1.11/tapesprocketdesigner.egg-info/top_level.txt
+drwxrwxr-x   0 niels     (1000) niels     (1000)        0 2023-06-10 18:57:27.889042 tapesprocketdesigner-0.1.9/
+-rw-rw-r--   0 niels     (1000) niels     (1000)    35149 2023-06-10 15:38:35.000000 tapesprocketdesigner-0.1.9/LICENSE
+-rw-rw-r--   0 niels     (1000) niels     (1000)    47979 2023-06-10 18:57:27.889042 tapesprocketdesigner-0.1.9/PKG-INFO
+-rw-rw-r--   0 niels     (1000) niels     (1000)     6754 2023-06-10 15:44:39.000000 tapesprocketdesigner-0.1.9/README.md
+-rw-rw-r--   0 niels     (1000) niels     (1000)     1134 2023-06-10 18:57:22.000000 tapesprocketdesigner-0.1.9/pyproject.toml
+-rw-rw-r--   0 niels     (1000) niels     (1000)       38 2023-06-10 18:57:27.889042 tapesprocketdesigner-0.1.9/setup.cfg
+drwxrwxr-x   0 niels     (1000) niels     (1000)        0 2023-06-10 18:57:27.889042 tapesprocketdesigner-0.1.9/tapesprocketdesigner/
+-rw-rw-r--   0 niels     (1000) niels     (1000)        0 2023-06-10 17:58:57.000000 tapesprocketdesigner-0.1.9/tapesprocketdesigner/__init__.py
+-rwxrwxr-x   0 niels     (1000) niels     (1000)    18571 2023-06-10 18:36:52.000000 tapesprocketdesigner-0.1.9/tapesprocketdesigner/designer.py
+-rw-rw-r--   0 niels     (1000) niels     (1000)     4468 2011-02-14 01:22:50.000000 tapesprocketdesigner-0.1.9/tapesprocketdesigner/dxf_templates_b2.py
+drwxrwxr-x   0 niels     (1000) niels     (1000)        0 2023-06-10 18:57:27.889042 tapesprocketdesigner-0.1.9/tapesprocketdesigner.egg-info/
+-rw-rw-r--   0 niels     (1000) niels     (1000)    47979 2023-06-10 18:57:27.000000 tapesprocketdesigner-0.1.9/tapesprocketdesigner.egg-info/PKG-INFO
+-rw-rw-r--   0 niels     (1000) niels     (1000)      405 2023-06-10 18:57:27.000000 tapesprocketdesigner-0.1.9/tapesprocketdesigner.egg-info/SOURCES.txt
+-rw-rw-r--   0 niels     (1000) niels     (1000)        1 2023-06-10 18:57:27.000000 tapesprocketdesigner-0.1.9/tapesprocketdesigner.egg-info/dependency_links.txt
+-rw-rw-r--   0 niels     (1000) niels     (1000)       76 2023-06-10 18:57:27.000000 tapesprocketdesigner-0.1.9/tapesprocketdesigner.egg-info/entry_points.txt
+-rw-rw-r--   0 niels     (1000) niels     (1000)        6 2023-06-10 18:57:27.000000 tapesprocketdesigner-0.1.9/tapesprocketdesigner.egg-info/requires.txt
+-rw-rw-r--   0 niels     (1000) niels     (1000)       21 2023-06-10 18:57:27.000000 tapesprocketdesigner-0.1.9/tapesprocketdesigner.egg-info/top_level.txt
```

### Comparing `tapesprocketdesigner-0.1.11/LICENSE` & `tapesprocketdesigner-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tapesprocketdesigner-0.1.11/PKG-INFO` & `tapesprocketdesigner-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapesprocketdesigner
-Version: 0.1.11
+Version: 0.1.9
 Summary: An application to design SMD tape sprockets
 Author-email: Niels Moseley <sofascener@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,25 +680,25 @@
         
 Project-URL: Homepage, https://github.com/trcwm/tapesprocketdesigner
 Project-URL: Bug Tracker, https://github.com/trcwm/tapesprocketdesigner/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tape Sprocket Designer
 
 This is a free (open source) Python script for creating feeder sprockets for e.g. perforated tape or film advance. I wrote it for myself to generate SMD tape-and-reel feed sprockets, but it might also be useful for making replacement sprockets for 8/16/35mm film, microfilm and paper-tape systems whose original reader hardware no longer exists or is difficult to find replacement parts for. The output is a .DXF template suitable for laser cutting, 3D printing or CNC machining.
 
-## Dependencies
-* pyside6
-* ezdxf
+
+
 
 ## Sprocket design goals / differences from other sprocket types
 
 The drive sprocket's dimensions are specified mainly by the number of teeth, width (or diameter) of the sprocket holes, and the pitch (distance between sprocket hole centers). The tape is usually advanced either tangentally to the sprocket, or partially wrapped around the sprocket. Thus the distance between the <i>outside edges</i> of any two teeth at any point, either tangent to the sprocket or along the circumference of the sprocket, should never exceed the distance between the outer edges of any two sprocket holes (the taper of the teeth is computed to counteract the radial splay of the teeth). Additionally, a landing area (flank) is cut at the base of the teeth matching the thickness of the tape, giving it a place to 'catch' when pressed against the sprocket's inner diameter. Unlike e.g. roller chain sprockets or spur gears, no undercut (cuts below the inner diameter) is provided for rollers or a mating gear's teeth, and no special geometry is needed along the sides of the teeth.
```

### Comparing `tapesprocketdesigner-0.1.11/README.md` & `tapesprocketdesigner-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Tape Sprocket Designer
 
 This is a free (open source) Python script for creating feeder sprockets for e.g. perforated tape or film advance. I wrote it for myself to generate SMD tape-and-reel feed sprockets, but it might also be useful for making replacement sprockets for 8/16/35mm film, microfilm and paper-tape systems whose original reader hardware no longer exists or is difficult to find replacement parts for. The output is a .DXF template suitable for laser cutting, 3D printing or CNC machining.
 
-## Dependencies
-* pyside6
-* ezdxf
+
+
 
 ## Sprocket design goals / differences from other sprocket types
 
 The drive sprocket's dimensions are specified mainly by the number of teeth, width (or diameter) of the sprocket holes, and the pitch (distance between sprocket hole centers). The tape is usually advanced either tangentally to the sprocket, or partially wrapped around the sprocket. Thus the distance between the <i>outside edges</i> of any two teeth at any point, either tangent to the sprocket or along the circumference of the sprocket, should never exceed the distance between the outer edges of any two sprocket holes (the taper of the teeth is computed to counteract the radial splay of the teeth). Additionally, a landing area (flank) is cut at the base of the teeth matching the thickness of the tape, giving it a place to 'catch' when pressed against the sprocket's inner diameter. Unlike e.g. roller chain sprockets or spur gears, no undercut (cuts below the inner diameter) is provided for rollers or a mating gear's teeth, and no special geometry is needed along the sides of the teeth.
```

### Comparing `tapesprocketdesigner-0.1.11/pyproject.toml` & `tapesprocketdesigner-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 
 [project]
 name = "tapesprocketdesigner"
 description = "An application to design SMD tape sprockets"
-version = "0.1.11"
+version = "0.1.9"
 authors = [
   { name="Niels Moseley", email="sofascener@gmail.com" },
 ]
 dependencies = [
-    "pyside6",
-    "ezdxf"
+    "PyQt5"
 ]
 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent"
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Build Tools"
 ]
 
-#     "Topic :: Computer Aided Design :: Mechanical"
-
 [tool.setuptools.packages.find]
 include = ["tapesprocketdesigner*"]
 
 #[tool.setuptools.packages.find]
 #where = ["src"]  # list of folders that contain the packages (["."] by default)
 
 [project.scripts]
```

### Comparing `tapesprocketdesigner-0.1.11/tapesprocketdesigner/designer.py` & `tapesprocketdesigner-0.1.9/tapesprocketdesigner/designer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,125 @@
 #!/usr/bin/python3
 import sys
 import math
-import ezdxf
-from ezdxf import units
+from PyQt5.QtWidgets import *
+from PyQt5.QtGui import *
+from PyQt5.QtCore import Qt, QPointF
 
-from PySide6.QtWidgets import *
-from PySide6.QtGui import *
-from PySide6.QtCore import Qt, QPointF
+import tapesprocketdesigner.dxf_templates_b2
+
+class DXFGenerator:
+
+    def __init__(self):
+        self.dxf = ""
+
+    def add(self, str):
+        self.dxf += str
+
+    def insertCode(self, code, value):
+        self.dxf += code + "\n" + value + "\n"
+
+    def line(self, theLine, scale):
+        self.insertCode(   '0', 'LINE' )
+        self.insertCode(   '8', 'Default' ) # layer name
+        self.insertCode(  '62', '4' )
+        self.insertCode(   '5', '255' ) # DXF entity handle
+        self.insertCode( '100', 'AcDbEntity' )
+        self.insertCode( '100', 'AcDbLine' )
+        self.insertCode(  '10', '{:.3f}'.format(theLine[0][0] * scale) ) # line start x
+        self.insertCode(  '20', '{:.3f}'.format(theLine[0][1] * scale) ) # line start y
+        self.insertCode(  '30', '0.0' )
+        self.insertCode(  '11', '{:.3f}'.format(theLine[1][0] * scale) ) # line end x
+        self.insertCode(  '21', '{:.3f}'.format(theLine[1][1] * scale) ) # line end x
+        self.insertCode(  '31', '0.0' )        
+
+    def point(self, point, scale):
+        self.insertCode(   '0', 'POINT' )
+        self.insertCode(   '8', 'Drills' ) # layer name
+        self.insertCode(  '62', '4' )
+        self.insertCode(   '5', '255' ) # DXF entity handle
+        self.insertCode( '100', 'AcDbEntity' )
+        self.insertCode( '100', 'AcDbPoint' )
+        self.insertCode(  '10', '{:.3f}'.format(point[0] * scale) )
+        self.insertCode(  '20', '{:.3f}'.format(point[1] * scale) )
+        self.insertCode(  '30', '0.0' )
+
+    def layerTable(self, layers):
+        self.insertCode('0', 'TABLE')
+        self.insertCode('2', 'LAYER')
+        self.insertCode('5', '2')
+        self.insertCode('330', '0')
+        self.insertCode('100', 'AcDbSymbolTable')
+        # group code 70 tells a reader how many table records to expect (e.g. pre-allocate memory for).
+        # It must be greater or equal to the actual number of records
+        self.insertCode('70',str(len(layers)))
+
+        for layer in layers:
+            self.insertCode('0', 'LAYER')
+            self.insertCode('5', '10')
+            self.insertCode('330', '2')
+            self.insertCode('100', 'AcDbSymbolTableRecord')
+            self.insertCode('100', 'AcDbLayerTableRecord')
+            self.insertCode('2', layer)
+            self.insertCode('70', '0')
+            self.insertCode('62', '7')
+            self.insertCode('6', 'CONTINUOUS')
+
+        self.insertCode('0','ENDTAB')
+        self.insertCode('0','ENDSEC')
+
+    def generate(self, lines) -> str :
+    
+        # handle unit scaling if any
+        unit_scale = 1
+        self.dxf = ""
+
+        # headery crap
+        self.insertCode( '999', 'Tape sprocket created by tapegear.py' ) # bogus code 'almost' universally accepted as a comment; comment this line if your DXF parser complains
+        self.add( dxf_templates_b2.r14_header )
+        self.layerTable(["Default", "Drills"])
+        self.add( dxf_templates_b2.r14_blocks )
+        
+        # now the actual geometry...
+        for L in lines:
+            self.line(L, unit_scale)
+
+        #for i in rect_comp_drills:
+        #    dxf_point(i, unit_scale)
+
+        # and footer
+        self.add( dxf_templates_b2.r14_footer )
+
+        return self.dxf
+
+        #filename = asksaveasfilename(filetypes=[('DXF (Drawing eXchange Format r14)', '.dxf')], initialfile='sprocket.dxf')
+        #if filename != None:
+        #    print("Started writing DXF")
+        #    f = open(filename, 'w')
+        #    f.write(dxf)
+        #    f.close()
+        #    print("Finished writing DXF")
 
 class SprocketCanvas(QWidget):
 
     def __init__(self):
         super().__init__()
         self.lines = []
         self.userOuterRadius = 1000000
 
     def paintEvent(self, paintEvent):
         painter = QPainter(self)
         brush = QBrush()
         brush.setColor(QColor('lightgrey'))
-        brush.setStyle(Qt.BrushStyle.SolidPattern)
+        brush.setStyle(Qt.SolidPattern)
         painter.fillRect(self.rect(), brush)
 
         center = self.rect().center()
 
-        painter.setBrush(Qt.BrushStyle.NoBrush)
+        painter.setBrush(Qt.NoBrush)
         painter.setPen(QColor('black'))
         for L in self.lines:
             start = QPointF(center.x() + self.k*L[0][0], center.y() - self.k*L[0][1])
             stop  = QPointF(center.x() + self.k*L[1][0], center.y() - self.k*L[1][1])
             painter.drawLine(start, stop)
 
     def setLines(self, lines, user_outer_radius):
@@ -55,15 +146,15 @@
 
         # Generate the left side panel
         panelLayout = QVBoxLayout()
         self.mainLayout.addLayout(panelLayout)
 
         # setup Basic Parameters group
         self.basicParametersGrp = QGroupBox("Basic Parameters")
-        self.basicParametersGrp.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Minimum)
+        self.basicParametersGrp.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
         panelLayout.addWidget(self.basicParametersGrp)
 
         gridLayout = QGridLayout()
         self.basicParametersGrp.setLayout(gridLayout)
 
         gridLayout.addWidget(QLabel("# of teeth"), 0,0)
         self.numTeeth = QLineEdit("14")
@@ -89,15 +180,15 @@
         self.toothLengthPct = QLineEdit("60")
         gridLayout.addWidget(self.toothLengthPct, 4,1)
         gridLayout.addWidget(QLabel("percent"), 4,2)
 
         # setup Report group
 
         self.reportGrp = QGroupBox("Report")
-        self.reportGrp.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Minimum)
+        self.reportGrp.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
         panelLayout.addWidget(self.reportGrp)
 
         gridLayout2 = QGridLayout()
         self.reportGrp.setLayout(gridLayout2)
 
         gridLayout2.addWidget(QLabel("Inner diameter"), 0,0)
         self.innerDiameter = QLabel("N/A")
@@ -117,27 +208,27 @@
         gridLayout2.addWidget(QLabel("Max. outer diameter"), 3,0)
         self.maxOuterDiameter = QLabel("N/A")
         gridLayout2.addWidget(self.maxOuterDiameter, 3,1)
         gridLayout2.addWidget(QLabel("mm"), 3,2)        
 
         # Export to DXF button
         self.exportButton = QPushButton("Export to DXF")
-        self.exportButton.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Minimum)
+        self.exportButton.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
         self.exportButton.pressed.connect(self.onWriteDXF)
         panelLayout.addWidget(self.exportButton)
 
-        panelLayout.addSpacerItem(QSpacerItem(0,0, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.MinimumExpanding))
+        panelLayout.addSpacerItem(QSpacerItem(0,0, QSizePolicy.Minimum, QSizePolicy.MinimumExpanding))
 
         # Generate the right sprocket display
 
         rightLayout = QVBoxLayout()
 
         self.sprocketCanvas = SprocketCanvas()
         self.sprocketCanvas.setMinimumSize(200,200)
-        sprocketCanvasSizePolicy = QSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
+        sprocketCanvasSizePolicy = QSizePolicy(QSizePolicy.Expanding, QSizePolicy.Expanding)
         #sprocketCanvasSizePolicy.setHeightForWidth(True)
         self.sprocketCanvas.setSizePolicy(sprocketCanvasSizePolicy)
         rightLayout.addWidget(self.sprocketCanvas, 1)
         #rightLayout.addSpacerItem(QSpacerItem(0,0, QSizePolicy.MinimumExpanding, QSizePolicy.MinimumExpanding))
 
         self.mainLayout.addLayout(rightLayout, 1)
 
@@ -147,17 +238,14 @@
         # Connect up the GUI widgets
         self.numTeeth.editingFinished.connect(self.computeGear)
         self.toothDiameter.editingFinished.connect(self.computeGear)
         self.toothSpacing.editingFinished.connect(self.computeGear)
         self.toothFlankHeight.editingFinished.connect(self.computeGear)
         self.toothLengthPct.editingFinished.connect(self.computeGear)
 
-        # init data
-        self.lines = []
-
         self.show()
 
     def computeGear(self):
         n_teeth   = float(self.numTeeth.text())
         tooth_dia = float(self.toothDiameter.text())
         tooth_pitch = float(self.toothSpacing.text())
         flank_height = float(self.toothFlankHeight.text())
@@ -203,28 +291,28 @@
         #    tooth_outer_angle = float(toothFaceAngleValue.get())
         #    tooth_inner_angle = 90.0 - tooth_outer_angle - (chord_angle / 2.0)
         #except ValueError:
         tooth_outer_angle = (chord_angle + (360.0 / n_teeth)) / 4.0 # half the equidistant-to-two-teeth to edge-of-tooth angle -> 1/4 of edge-to-edge angle
         tooth_inner_angle = 90.0 - tooth_outer_angle - (chord_angle / 2.0)
             #toothFaceAngleValue.set(str(tooth_outer_angle))
 
-        #print("Tooth centers angle: {:f}".format(360.0/n_teeth))
-        #print("Tooth width contribution: {:f}".format(chord_angle))
-        #print("Tooth edges angle: {:f}".format((360.0/n_teeth) + chord_angle))
+        print("Tooth centers angle: {:f}".format(360.0/n_teeth))
+        print("Tooth width contribution: {:f}".format(chord_angle))
+        print("Tooth edges angle: {:f}".format((360.0/n_teeth) + chord_angle))
 
-        #print("Design circumference = {:f} radius = {:f}".format(design_circumference, design_radius))
-        #print("Min. tooth angle: {:f} degrees from vertical".format(tooth_outer_angle))
+        print("Design circumference = {:f} radius = {:f}".format(design_circumference, design_radius))
+        print("Min. tooth angle: {:f} degrees from vertical".format(tooth_outer_angle))
 
         tooth_face_height = (tooth_dia / 2.0) * math.tan(tooth_inner_angle * (math.pi / 180.0))
         max_outer_radius = design_radius + tooth_face_height
 
         user_outer_radius = design_radius + ((max_outer_radius - design_radius) * (tooth_length_pct/100.0)) #design_radius + (design_radius*0.5) #max_outer_radius
 
-        #print("Resulting tooth height (angled portion) = {:f}".format(tooth_face_height))
-        #print("Outer radius = {:f}".format(max_outer_radius))
+        print("Resulting tooth height (angled portion) = {:f}".format(tooth_face_height))
+        print("Outer radius = {:f}".format(max_outer_radius))
 
         # From list of tooth centers...
         # Flank (starts,ends): tooth center +/- tooth chordal angle
         # Faces: Remember, working in polar coords. Doublecheck this, but I think where the angle of the ray intersecting the "end of face" (between 0 and chord_angle/2 relative to tooth center) falls will be proportional to where end of face falls between design radius and max. outer radius.
 
         face_ratio = (user_outer_radius - design_radius) / (max_outer_radius - design_radius) # will produce a result between 0 and 1
 
@@ -280,66 +368,52 @@
                 # put the hole center @ inside diameter line, 1 cutter radius from edge of tooth
                 polar_comp_drills.append([inner_radius, i+(chord_angle/2) + (360*comp_r/(2*math.pi*(inner_radius - comp_r)))])
                 # at start of next tooth
                 polar_comp_drills.append([inner_radius , i+(360.0/n_teeth)-(chord_angle/2) - (360*comp_r/(2*math.pi*(inner_radius - comp_r)))])
         except ValueError:
             comp_r = 0
 
-        self.lines = []
+        rect_lines = []
         rect_comp_drills = []
 
         for i in polar_lines:
-            self.lines.append([self.p2r(i[0][0],i[0][1]),  self.p2r(i[1][0],i[1][1])])
+            rect_lines.append([self.p2r(i[0][0],i[0][1]),  self.p2r(i[1][0],i[1][1])])
 
         for i in polar_comp_drills:
             rect_comp_drills.append(self.p2r(i[0],i[1]))
 
-        self.sprocketCanvas.setLines(self.lines, user_outer_radius)
+        self.sprocketCanvas.setLines(rect_lines, user_outer_radius)
 
         self.innerDiameter.setText("{:.3f}".format(inner_radius * 2))
         self.designDiameter.setText("{:.3f}".format(design_radius * 2))
         self.outerDiameter.setText("{:.3f}".format(user_outer_radius * 2))
         self.maxOuterDiameter.setText("{:.3f}".format(max_outer_radius * 2))
 
     def p2r(self, r, theta):
         #python's builtin math functions work in radians, so convert...
         theta = theta * (math.pi / 180.0)
         return r*math.cos(theta), r*math.sin(theta)
 
-    def p2r_tuple(self, r, theta):
-        #python's builtin math functions work in radians, so convert...
-        theta = theta * (math.pi / 180.0)
-        return (r*math.cos(theta), r*math.sin(theta))
 
     def dist(self, xy1, xy2):
         dist_x = abs(xy1[0] - xy2[0])
         dist_y = abs(xy1[1] - xy2[1])
         distance = math.sqrt((dist_x*dist_x) + (dist_y*dist_y))
         return distance
 
     def onWriteDXF(self):
         if not self.sprocketCanvas.getLines():
             return            
 
+        dxfgen = DXFGenerator()
+        dxf = dxfgen.generate(self.sprocketCanvas.getLines())
+
         fileName, _ = QFileDialog.getSaveFileName(self, "Export as DXF","","DXF Files (*.dxf)")
         if fileName:
-            #doc = ezdxf.new("R2000", setup=True)
-            doc = ezdxf.new("R2000")
-            doc.units = units.MM
-            msp = doc.modelspace()
-            #pline = msp.add_lwpolyline(self.points)
-
-            for L in self.lines:
-                pstart = (L[0][0], L[0][1])
-                pstop  = (L[1][0], L[1][1])
-                msp.add_line(pstart, pstop)
-
-            doc.saveas(fileName)
+            DFXFile = open(fileName, "w")
+            DFXFile.write(dxf)
+            DFXFile.close()
 
 def main():
     app = QApplication(sys.argv)
     window = MainWindow()
     sys.exit(app.exec())
-
-if (__name__ == "__main__"):
-    main()
-
```

### Comparing `tapesprocketdesigner-0.1.11/tapesprocketdesigner.egg-info/PKG-INFO` & `tapesprocketdesigner-0.1.9/tapesprocketdesigner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapesprocketdesigner
-Version: 0.1.11
+Version: 0.1.9
 Summary: An application to design SMD tape sprockets
 Author-email: Niels Moseley <sofascener@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -680,25 +680,25 @@
         
 Project-URL: Homepage, https://github.com/trcwm/tapesprocketdesigner
 Project-URL: Bug Tracker, https://github.com/trcwm/tapesprocketdesigner/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Tape Sprocket Designer
 
 This is a free (open source) Python script for creating feeder sprockets for e.g. perforated tape or film advance. I wrote it for myself to generate SMD tape-and-reel feed sprockets, but it might also be useful for making replacement sprockets for 8/16/35mm film, microfilm and paper-tape systems whose original reader hardware no longer exists or is difficult to find replacement parts for. The output is a .DXF template suitable for laser cutting, 3D printing or CNC machining.
 
-## Dependencies
-* pyside6
-* ezdxf
+
+
 
 ## Sprocket design goals / differences from other sprocket types
 
 The drive sprocket's dimensions are specified mainly by the number of teeth, width (or diameter) of the sprocket holes, and the pitch (distance between sprocket hole centers). The tape is usually advanced either tangentally to the sprocket, or partially wrapped around the sprocket. Thus the distance between the <i>outside edges</i> of any two teeth at any point, either tangent to the sprocket or along the circumference of the sprocket, should never exceed the distance between the outer edges of any two sprocket holes (the taper of the teeth is computed to counteract the radial splay of the teeth). Additionally, a landing area (flank) is cut at the base of the teeth matching the thickness of the tape, giving it a place to 'catch' when pressed against the sprocket's inner diameter. Unlike e.g. roller chain sprockets or spur gears, no undercut (cuts below the inner diameter) is provided for rollers or a mating gear's teeth, and no special geometry is needed along the sides of the teeth.
```

