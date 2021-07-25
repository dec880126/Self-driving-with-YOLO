# YOLOv4-Self-driving

## Environment

VM: Google Colaboratory
GPU: NVIDIA T4 Tensor GPU
NVIDIA-SMI 470.42.01    Driver Version: 460.32.03    CUDA Version: 11.2
nvcc: NVIDIA (R) Cuda compiler driver
Cuda compilation tools, release 11.0, V11.0.221
Build cuda_11.0_bu.TC445_37.28845127_0

## Training Log

![image](https://user-images.githubusercontent.com/34447298/126898309-b749ffc5-0495-4594-894b-fdc57090ed4e.png)
> I loss some training log beacuse it will be disconnected after a about 2~3 hours with Goolge Colaboratory.

## mAP(mean accuracy precision)

detections_count = 110160, unique_truth_count = 32699
class_id = 0, name = car, ap = 72.28% (TP = 16024, FP = 6722)
class_id = 1, name = truck, ap = 62.58% (TP = 624, FP = 277)
class_id = 2, name = pedestrian, ap = 39.53% (TP = 2060, FP = 1502)
class_id = 3, name = bicyclist, ap = 36.90% (TP = 89, FP = 75)
class_id = 4, name = light, ap = 48.34% (TP = 2138, FP = 758)
for conf_thresh = 0.25, precision = 0.69, recall = 0.64, F1-score = 0.66
for conf_thresh = 0.25, TP = 20935, FP = 9334, FN = 11764, average IoU = 53.16 %
IoU threshold = 50 %, used Area-Under-Curve for each unique Recall
**mean average precision (mAP@0.50) = 51.93 %**

## Video demo
- Quality: 720p
- AVG_FPS: 33.5<br>
[![Alt text](https://i.ytimg.com/vi/KRhkeHaPoyg/hqdefault.jpg?sqp=-oaymwEcCPYBEIoBSFXyq4qpAw4IARUAAIhCGAFwAcABBg==&rs=AOn4CLBuo-TOUEEKVe7HPJy5eIkQZiCVdQ)](https://youtu.be/KRhkeHaPoyg)


### Other quality

- 360p
- AVG_FPS: 52.0
