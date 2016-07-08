# Note of ImageJ
Some notes about ImageJ, please feel free to correct me if I said something incorrect below.

**Q: How to use ImageJ ?**
- Method 1: Download the ImageJ software and use it as other GUI tools.
- Method 2: To program with ImageJ, download the ImageJ libraries and embed it into the Java project's build path.

**Q: While programming with ImageJ, how to draw a contour on the image ?**
- Use _ij.gui.Overlay_ or _ij.gui.Roi_
- According to my experience, a colored contour is allowed with Overlay on a gray-scaled image, while it is not with Roi, i.e., you always get the gray contour with Roi if the image is gray-scaled.

**Q: How to save the overlays with the image ?**
- Use _FileSaver.saveAsJpeg()_.
- Not sure if it is the only one method to save the overlays with the image, but there are some methods in FileSaver which fails in doing this. For example, the _FileSaver.saveAsBmp()_ simply save the image without the overlays.

**Q: Is there a way to combine all the scattered windows ?**
- To my knowledge, ImageJ doesn't provide the function. To develope a composite window requires another effort.
- Here is an example of composite UI: https://github.com/fiji/Trainable_Segmentation/blob/master/src/main/java/trainableSegmentation/Weka_Segmentation.java#L532-L535
