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
* Run through main [code](https://github.com/waliddib095/RealTimeObjectDetection/tree/main/RealTimeObjectDetection-main/main_code) on Jupyter notebook up to step 6.
* Note: Training steps can be set based on desired accuracy/time trade off. 5000 steps were used to reach a loss below 0.2 as shown:
![alt text](https://github.com/waliddib095/RealTimeObjectDetection/blob/main/RealTimeObjectDetection-main/example_images/Training%20Steps.PNG)

## Detect in Real Time
* Use CV2 to setup video capture: 
```
cap = CV2.VideoCaptue(0)
```
* Note: My webcame is device 0. The user's webcam could be accessed through a diffrent number like 1 or 2, if 0 doesn't work out.
* Run subsequent code for real time detection to start as shown:

![alt text](https://github.com/waliddib095/RealTimeObjectDetection/blob/main/RealTimeObjectDetection-main/example_images/Mask.PNG)

![alt text](https://github.com/waliddib095/RealTimeObjectDetection/blob/main/RealTimeObjectDetection-main/example_images/Nomask.PNG)

* Note: To terminate, run the following code:
```
cap.release()
```
