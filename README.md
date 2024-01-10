###DynamicST-Assist introduction
---

This software is ued to regist tissue image with reference frames and detect tissue area, and output the information of each spot,including its location, barcode, and whether it is covered by the tissue.

###DynamicST-Assist require files
---

The files required to run this software are:

1. Tissue image with reference frames;

2. Barcode list file.

Tissue image requirements:

1. With reference frame；

2. Image resolution less than 8000 * 8000.

###DynamicST-Assist software operation
---

Detailed operation documents can be found in [here]

The software includes five interfaces: LOAE IMAGE, SELECT POINTS, REGIST IMAGE, TISSUE DETECT, and EXPOSE JSON.

The STEP area in the upper left of the software interfaces can guide the operation.

-**Load Image**:

In LOAE IMAGE interface, press button LOADIMAGE to load a tissue image.

Press button NEXT or button 2.SELECT POINTS to next interface.

-**Regist Image**:

In SELECT POINTS interface, click the mouse to select reference points on image.

Press button NEXT or button 3.REGIST IMAGE to next interface.

In REGIST IMAGE interface, fine tune the position of the reference points and then press button REGISTIMAGE.

Press button NEXT or button 4.TISSUE DETECT to next interface.

-**Tissue Detect**:

In TISSUE DETECT interface, press button TISSUEDETECTION.

fine tune the spots covered by tissue.

Press button NEXT or button 5.EXPOSE JSON to next interface.

-**Output Result**:

In EXPOSE JSON interface, press button EXPOSEJSON.




