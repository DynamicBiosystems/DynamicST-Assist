Introduction
---


  <div align=center><img src='./images/exe.png' width =60%, height=60%></div>
  DynamicST Assist is an interactive software that guides users in manually identifying fiducials in DynaSpatial images, selecting spots under tissue, and aligning DynaBlot images with microscope images. 

  This software includes two functions: DynaBlot image and microscope image Alignment, fiducial alignment and tissue detection.

  DynaBlot image and microscope image Alignment is used to align microscope image with DynaBlot image.

  In this function,the following files are required：

    1.DynaBlot image

    2.Microscope image

  Fiducial alignment and tissue detection is used to adjust DynaBlot image and detect tissue area to obtain the location information of each spot and whether it is covered by tissue area.

  In this function, image with fiducial frame is required.

Installation
---

<div align=center><img src='./images/setup.png' width =40%, height=40%></div>

Double click the exe shown in figure to start the installation.


Usage
---

  The operation of DynamicST Assist consists of three parts, start software, DynaBlot image and microscope image alignment and fiducial alignment and issue detection.

  Current step and completed steps will be displayed in STEPS. And currently available operations will be displayed in tools.

  During the operation, you can  zoom the image by scroll the mouse wheel to, or drag the image by pressing the right mouse button.

**1.Start software**:

  In this part, you have two choices.The operation process is as follows:

    (1)If you only have DynaBlot image, you need to click button “DYNABLOT IMAGE - MICROSCOPE IMAGE ALIGNMENT” and software will skip DynaBlot image and microscope image alignment. In this part, you can adjust DynaBlot image and detect tissue area.

    (2)If you have DynaBlot image and microscope image of the same tissue and need to align the two image, you need to click button“FIDUCIAL ALIGNMENT AND TISSUE DETECTION” and software will skip DynaBlot image and microscope image alignment. In this part, you can align DynaBlot image and microscope image. After alignment, you need to continue to fiducial alignment and issue detection.

  <div align=center><img src='./images/start.png' width =60%, height=60%></div>


**2.DynaBlot image-microscope image alignment**:

  In this part, you can align DynaBlot image and microscope image. 
  (1)Operation process:

    1)Load images

      A.Click button “LOADIMAGE” on the left to load DynaBlot image, the DynaBlot image will be flipped horizontally.
  
      B.Click button “LOADIMAGE” on the right to load microscope image.
  
      C.Click button “REPLACEIMAGE” on the top of “TOOLS” to replace DynaBlot image, the DynaBlot image will be flipped horizontally.
  
      D.Click button “REPLACEIMAGE” on the bottom of “TOOLS” to replace microscope image.
  
      E.Click button ”NEXT” to Alignment image step.

  <div align=center><img src='./images/LoadAlignmentImages.png' width =60%, height=60%></div>
  
  
    2)Alignment image

      A.Pin landmarks on the images by clicking the mouse.
  
      B.Click button “ALIGNMENTIMAGE” to alignment microscope according to landmarks.
  
      C.Click button ”NEXT” to Auto refine step.
  <div align=center><img src='./images/AlignmentImages.png' width =60%, height=60%></div>
  
  
    3)Auto refine

      A.Adjust the Slider “Traqnsparency” to visual inspect the result of alignment.
      
      B.Click button “AUTO-REFINE” to automatically fine tune the result of alignment.
      
      C.If the fine-tuning result is unsatisfactory, you can click it several times until the result is satisfactory.
      
      D.Click button ”NEXT” to Expose alignment result step.

  <div align=center><img src='./images/Auto-Refine.png' width =60%, height=60%></div>
  
  
    4)Expose alignment result

      A.Click button ”CONTINUE TO MANUAL FIDUCIAL ALIGNMENT” to skip manual alignment of DynaBlot image with fiducial frame.
  
      B.In this step, microscope image after alignment will be saved to the path of the microscope image and named as “microscope image name_tissue_image.tif”.

  <div align=center><img src='./images/ExposeAlignment.png' width =60%, height=60%></div>

  (2)Output
    The output of this step is the image of the microscope image after alignbment. 
    
    The image will be named as “microscope image name_tissue_image.tif” and saved to the path of the microscope image.

<div align=center><img src='./images/AlignmentResult.png' width =60%, height=60%></div>
  

**3.Manual alignment of DynaBlot image with fiducial frame**:

  In this part, you can adjust DynaBlot image and detect tissue area.
  (1)Operation process:

    1)Load image

      A.Click button “LOADIMAGE” to load image with fiducial frame.
  
      B.Click button “REPLACEIMAGE” on the “TOOLS” to replace image.
  
      C.Choose chip type in combobox.
  
      D.Click button ”NEXT” to Select points step.

  <div align=center><img src='./images/LoadFiducialImage.png' width =60%, height=60%></div>
  

    2)Select points

      A.Select the points by clicking the mouse, in the order shown in the figure.
  
      B.Clean up the records of the selected points by clicking button “CLEANPOINTS”.
  
      C.Click button ”NEXT” to Adjust image step.

  <div align=center><img src='./images/SelectPoints.png' width =60%, height=60%></div>
  

    3)Adjust image

      A.If the coordinates of the points are not accurate, you can select the point to be tuned, and then fine tune the coordinate of this point in the x and y directions in the spinbox.
  
      B.Click button “ADJUSTIMAGE” to adjust DynaBlot image.
  
      C.The spots corresponding to the DynaBlot image will be displayed on the image.
  
      D.In tihs step, if you have aligned DynaBlot image and microscope image, the microscope image will be adjusted in the same way as DynaBlot image and replace “microscope image name_tissue_image.tif”.
  
      E.Click button ”NEXT” to Detect tissue area step.
  
  <div align=center><img src='./images/AdjustImage.png' width =60%, height=60%></div>

      
    4)Detect tissue area

      A.If you have aligned DynaBlot image and microscope image, select image for tissue area detection, microscope image or DynaBlot image can be selected.
  
      B.Modify Sensitive slider to set parameter of tissue area detection algorithm.
  
      C.Choose image channel of tissue area detection algorithm.
  
      D.Click button “TISSUEDETECTION” to automatically detect tissue area.
  
      E.Modify Transparency slider can modify the transparency of spots.
  
      F.If the result of automatic detection is not accurate, you can fine tune the tissue area through the brush function.
  
        a.Select “SelectSpot” to add spots covered by tissue to the image.
    
        b.Select “DeleteSpot” to delete spots covered by tissue to the image.
    
        c.Modify Width slider to modify width of brush.
    
      G.Click button ”NEXT” to Expose json step.

  <div align=center><img src='./images/ChooseTissueDetectionImage.png' width =40%, height=40%></div>

  <div align=center><img src='./images/TissueDetection.png' width =60%, height=60%></div>
    

    5)Expose json

      A.Click button “EXPOSEJSON” to expose adjusted image and json file.
  
      B.The json file willed be named “Image name_alignment.json”。
  
      C.The adjusted image will be saved in the same path of json file.If you have aligned DynaBlot image and microscope image, the adjusted DynaBlot image will be named “DynaBlot image name_dynaimage.tif”, else the adjusted image will be named “Image name_tissue_image.tif”.

  <div align=center><img src='./images/ExposeAdjustResult.png' width =60%, height=60%></div>

  (2)Output:
    The json file willed be named “Image name_alignment.json” and saved in path selected.
    
    The adjusted image will be saved in the same path of json file.
    
    If you have aligned DynaBlot image and microscope image, the adjusted DynaBlot image will be named “DynaBlot image name_dynaimage.tif”.

<div align=center><img src='./images/AdjustResult1.png' width =60%, height=60%></div>
    
    Else the adjusted image will be named “Image name_tissue_image.tif”.

<div align=center><img src='./images/AdjustResult2.png' width =60%, height=60%></div>






