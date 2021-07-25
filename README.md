<h1 align="center">Self-driving training with YOLOv4</h1>

## Demo
![1627216237257](https://user-images.githubusercontent.com/34447298/126899013-21aadbf8-b79e-46ad-b63e-0d3d0f59cab5.gif)


## mAP(mean accuracy precision)

**mean average precision (mAP@0.50) = 51.93 %**<br><br>
detections_count = 110160, unique_truth_count = 32699<br>
class_id = 0, name = car, ap = 72.28% (TP = 16024, FP = 6722)<br>
class_id = 1, name = truck, ap = 62.58% (TP = 624, FP = 277)<br>
class_id = 2, name = pedestrian, ap = 39.53% (TP = 2060, FP = 1502)<br>
class_id = 3, name = bicyclist, ap = 36.90% (TP = 89, FP = 75)<br>
class_id = 4, name = light, ap = 48.34% (TP = 2138, FP = 758)<br>
for conf_thresh = 0.25, precision = 0.69, recall = 0.64, F1-score = 0.66<br>
for conf_thresh = 0.25, TP = 20935, FP = 9334, FN = 11764, average IoU = 53.16 %<br>
IoU threshold = 50 %, used Area-Under-Curve for each unique Recall<br>

## Types that can be detected
1. car
2. truck
3. pedestrian
4. bicyclist
5. light

## Training Log

![image](https://user-images.githubusercontent.com/34447298/126898309-b749ffc5-0495-4594-894b-fdc57090ed4e.png)
> I loss some training log beacuse it will be disconnected after a about 2~3 hours with Goolge Colaboratory.


## Weights I trained

- <a href='https://drive.google.com/file/d/1mmxOU3D-wyLeLI1jg-vhKj-Kt7UQ_GHs/view?usp=sharing' target="_blank">yolov4-obj_3.1656.weights</a>


## How to use

- Use with <a href='https://github.com/AlexeyAB/darknet' target="_blank">YOLOv4 AlexeyAB</a>


## Environment

VM: Google Colaboratory<br>
GPU: NVIDIA T4 Tensor GPU<br>
NVIDIA-SMI 470.42.01    Driver Version: 460.32.03    CUDA Version: 11.2<br>
nvcc: NVIDIA (R) Cuda compiler driver<br>
Cuda compilation tools, release 11.0, V11.0.221<br>
Build cuda_11.0_bu.TC445_37.28845127_0


## Full video demo

- Quality: 720p
- AVG_FPS: 33.5<br>
[![Alt text](https://i.ytimg.com/vi/KRhkeHaPoyg/hqdefault.jpg?sqp=-oaymwEcCPYBEIoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLBuo-TOUEEKVe7HPJy5eIkQZiCVdQ)](https://youtu.be/KRhkeHaPoyg)


### Other quality

- 360p
- AVG_FPS: 52.0

## Conference
Training data from: https://www.kaggle.com/alincijov/self-driving-cars
Tesing data from: https://youtu.be/z1obnaqPgMA
