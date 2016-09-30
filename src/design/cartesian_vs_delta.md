# Pro and contra list between a cartesian and a delta printer

**UNDER CONSTRUCTION**

|	criteria | Cartesian	| Delta |
| -------- | ---------- | ----- |
| velocity / acceleration | higher number of movable parts<br/>&emsp;&#8594; high inertia<br/>&emsp;&#8594; max v & a is different for every axis | moved mass / number of movable parts small<br/>&emsp;&#8594; small inertia<br/>&emsp;&#8594; relatively high printing speed possible |
| accuracy | Keine klare Aussage möglich. Scheint hauptsächlich von der Bauqualität und der Kalibrierung abzuhängen. | |
| reliability | Calibration has to be checked befor every print. (difficult) | Calibration has to be checked before every print. (easy) |
| | Has to be calibrated often | Has to be calibrated seldom |
| Calibration | Easy. Axis independent. | Difficult. Especailly the first calibration. Axis dependent. <br/>&emsp;&#8594; if one printer axis is false all cartesian axis are false |
| Bugfix | Easy. Bugs can be easily located. | Difficult. Sometimes difficult to locate the source of error. (calibration/build) |
| Printing Volume | cuboid | Cylinder respecively triangle |
| Size | Big in the x- and y-axis. | Big in the z-axis. |
| Slicer | Slicer programmed for cartesian printers | Uses the same software, which is not build for delat printers. |
| Control| Eas control since axis are equal. | Control more complex. Trigonometric functions needed. |
| Base | Moving in most builds <br/>&emsp;&#8594; problems with filigrane products <br/>&emsp;&#8594; no bowden tube needed | Only moved part is the hotend <br/>&emsp;&#8594; extruder mostly static. bowden tube needed <br/>&emsp;&#8594; problems may occure with some filaments |
