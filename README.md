# RealTimeObjectDetection
## Installation
Before walking through the code, please make sure to install TensorFlow's object detection API from the following [link](https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html)

## Labeling Images for Object Detection
* Clone labelImage [repository](https://github.com/tzutalin/labelImg)
* Install pyqt=5 inside the labelimage folder:

```
conda install pyqt=5
```

* Install lxml in the same folder:
```
conda isntall -c anaconda lxml
```
* Put all image data in allimages folder (Mask and No-Mask).
* Rub labelimage and start annotating all images as mask or no mask as shown:
```
python labelImge.py
```
![alt text](https://github.com/waliddib095/RealTimeObjectDetection/blob/main/RealTimeObjectDetection-main/example_images/Image%20Labeling.PNG)
![alt text](https://github.com/waliddib095/RealTimeObjectDetection/blob/main/RealTimeObjectDetection-main/example_images/Mask%20label.PNG)

## Training TensorFlow
Run through main [code](https://github.com/waliddib095/RealTimeObjectDetection/tree/main/RealTimeObjectDetection-main/main_code)
