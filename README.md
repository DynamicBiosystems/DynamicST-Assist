DynamicST-Assist introduction
---

DynamicST-Assist software is used to obtain the location and information of uncaptured spots on tissue image.

The spots extracted from the image will necessarily contain some misses. The relative position relationship between the fiducial points position and the spots position is fixed.  Therefore, the position and size of spots can be obtained through the position of the fiducial point.

The fiducial points are the corner of the fiducial frame. DynamicST-Assist software includes the function of manually selecting fiducial points on image.

After obtaining the position and size of the spots, it is possible to determine which spots are covered by the tissue through tissue area detection. DynamicST-Assist software includes function of tissue area detection.

The result file include the information of each spot,including it’s position, barcode, and whether it is covered by the tissue.

DynamicST-Assist require files
---

The files required to run this software are:

1. Tissue image with fiducial frame;

2. Barcode list file.

Barcode list file was provided in barcode_coordinate.txt .

Tissue image requirements:

1. With fiducial frame；

2. Image resolution less than 8000 * 8000.

DynamicST-Assist software operation
---

Detailed operation documents can be found in DynamicSTAssistv1.0.0_operation_manual.pdf .

The software includes five interfaces: LOAE IMAGE, SELECT POINTS, REGIST IMAGE, TISSUE DETECT, and EXPOSE JSON.

The STEP area in the upper left of the software interfaces can guide the operation.

**Load Image**:

In LOAE IMAGE interface, press button LOADIMAGE to load a tissue image.

Press button NEXT or button 2.SELECT POINTS to next interface.

**Regist Image**:

In SELECT POINTS interface, click the mouse to select fiducial points on image.

Press button NEXT or button 3.REGIST IMAGE to next interface.

In REGIST IMAGE interface, fine tune the position of the fiducial points and then press button REGISTIMAGE.

Press button NEXT or button 4.TISSUE DETECT to next interface.

**Tissue Detect**:

In TISSUE DETECT interface, press button TISSUEDETECTION.

fine tune the spots covered by tissue.

Press button NEXT or button 5.EXPOSE JSON to next interface.

**Output Result**:

In EXPOSE JSON interface, press button EXPOSEJSON.




