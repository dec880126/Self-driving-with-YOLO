<h1 align="center">Self-driving training with YOLO</h1>

## Demo
YOLOv4             |  YOLOv3
:-------------------------:|:-------------------------:
![1627216237257](https://user-images.githubusercontent.com/34447298/126899013-21aadbf8-b79e-46ad-b63e-0d3d0f59cab5.gif) | ![1627544679170](https://user-images.githubusercontent.com/34447298/127452341-4deb4463-1c65-4923-a30f-6aa8326c46cd.gif)


## AP
class             |  AP in YOLOv4 |  AP in YOLOv3 | TP&FP in YOLOv4 | TP&FP in YOLOv3
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
car | ap = 72.28% | ap = 69.30% | TP = 16024, FP = 6722 | TP = 15037, FP = 6829
truckr | ap = 62.58% | ap = 51.89% | TP = 624, FP = 277 | TP = 469, FP = 244
pedestrianr | ap = 39.53% | ap = 24.20% | TP = 2060, FP = 1502 | TP = 1213, FP = 1242
bicyclistr | ap = 36.90% | ap = 15.66% | TP = 89, FP = 75 | TP = 51, FP = 94
lightr | ap = 48.34% | ap = 42.93% | TP = 2138, FP = 758 | TP = 1793, FP = 706


## mAP(mean Average Precision)
YOLOv4             |  YOLOv3
:-------------------------:|:-------------------------:
**mean average precision (mAP@0.50) = 51.93 %** | **mean average precision (mAP@0.50) = 40.80 %**


## Types that can be detect
1. car: with 101314 labels
2. truck: with 6313 labels
3. pedestrian: with 10637 labels
4. bicyclist: with 1442 labels
5. light: with 12700 labels

## Training Log
YOLOv4             |  YOLOv3
:-------------------------:|:-------------------------:
![image](https://user-images.githubusercontent.com/34447298/126898309-b749ffc5-0495-4594-894b-fdc57090ed4e.png)  |  ![chart](https://user-images.githubusercontent.com/34447298/127447409-ed86928f-d060-440b-925c-fc0bedb69b0c.png)



## Weights I trained
YOLOv4             |  YOLOv3
:-------------------------:|:-------------------------:
<a href='https://drive.google.com/file/d/1mmxOU3D-wyLeLI1jg-vhKj-Kt7UQ_GHs/view?usp=sharing' target="_blank">yolov4-obj_3.1656.weights</a> | <a href='https://drive.google.com/file/d/1Hrf_RzsQWD8oRv5UX37C9JvF8QO8w7qp/view?usp=sharing' target="_blank">yolov3-obj_10000.weights</a>


## How to use

- Use with <a href='https://github.com/AlexeyAB/darknet' target="_blank">YOLOv4 AlexeyAB</a>


## Environment

- VM: Google Colaboratory
- GPU: NVIDIA T4 Tensor GPU
- NVIDIA-SMI 470.42.01    Driver Version: 460.32.03    CUDA Version: 11.2
- nvcc: NVIDIA (R) Cuda compiler driver
- Cuda compilation tools, release 11.0, V11.0.221
- Build cuda_11.0_bu.TC445_37.28845127_0


# Speed
| | YOLOv4             |  YOLOv3
|:-------------------------:|:-------------------------:|:-------------------------:
|Quality: 720p | AVG FPS = 33.5 | AVG FPS = 27.1
|Quality: 360p | AVG FPS = 52.0 | AVG FPS = 35.9
| mAP | 51.93 % | 40.80 %


## Full video demo

- Quality: 720p
- AVG_FPS: 33.5<br>
[![Alt text](https://i.ytimg.com/vi/KRhkeHaPoyg/hqdefault.jpg?sqp=-oaymwEcCPYBEIoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLBuo-TOUEEKVe7HPJy5eIkQZiCVdQ)](https://youtu.be/KRhkeHaPoyg)


### Other quality

- 360p
- AVG_FPS: 52.0

## References
- YOLOv4: Optimal Speed and Accuracy of Object Detection: https://arxiv.org/pdf/2004.10934
- Training data from: https://www.kaggle.com/alincijov/self-driving-cars
- Tesing data from: https://youtu.be/z1obnaqPgMA
