# ASL Static Sign Language Recognition using YOLOv5
This project focuses on recognizing American Sign Language (ASL) **static hand signs** using **YOLOv5**, a state-of-the-art object detection neural network. The implementation leverages **PyTorch 1.9.0** and is executed in **Google Colab** with **GPU acceleration** (Tesla T4).

## Project Overview

-  **Goal**: Classify static ASL signs using real-time object detection techniques.
-  **Model**: YOLOv5 (You Only Look Once version 5)
-  **Framework**: PyTorch 1.9.0
-  **Platform**: Google Colab (CUDA GPU Enabled)
-  **Use Case**: Assistive technology for speech and hearing impaired communication

---

## Neural Network Architecture

- **YOLO Version**: v5
- **Model Depth Multiple**: `0.33`
- **Model Width Multiple**: `0.50`
- **Model Summary**:
  - Layers: `283`
  - Parameters: `7,346,792`
  - Gradients: `7,346,792`
  - GFLOPs: `17.1`
- **Optimizer Groups**: 62 `.bias`, 70 `conv.weight`, 59 `other`
- **Scaled Weight Decay**: `0.00046875`

---

##  Hyperparameters

| Parameter           | Value     | Parameter         | Value     |
|---------------------|-----------|--------------------|-----------|
| `lr0`               | 0.01      | `lrf`              | 0.2       |
| `momentum`          | 0.937     | `weight_decay`     | 0.0005    |
| `warmup_epochs`     | 3.0       | `warmup_momentum`  | 0.8       |
| `warmup_bias_lr`    | 0.1       | `box`              | 0.05      |
| `cls`               | 0.5       | `cls_pw`           | 1.0       |
| `obj`               | 1.0       | `obj_pw`           | 1.0       |
| `iou_t`             | 0.2       | `anchor_t`         | 4.0       |
| `hsv_h`             | 0.015     | `hsv_s`            | 0.7       |
| `hsv_v`             | 0.4       | `translate`        | 0.1       |
| `scale`             | 0.5       | `fliplr`           | 0.5       |
| `mosaic`            | 1.0       |                   |           |

---

## Hardware & GPU Info

- **GPU**: Tesla T4  
- **CUDA Info**:
  - Compute Capability: `7.5`
  - Total Memory: `15,109 MB`
  - Multiprocessor Count: `40`

---

## Libraries Used

###  Base Libraries
- `matplotlib`
- `numpy`
- `opencv-python`
- `Pillow`
- `PyYAML`
- `scipy`
- `torch`
- `torchvision`
- `tqdm`

### Logging & Plotting
- `tensorboard`
- `seaborn`
- `pandas`

---

##  Dataset Details

- **Full Dataset**: [Download from Mega](https://mega.nz/folder/nF5TESLZ#NbGRqCzZTunbY49LCNrp_g)
- **Total Classes**: 35
- **Total Images**: 15,472

### Training Dataset
- Classes Used: `['Airplane', 'Bus', 'Calm Down', 'Car', 'Church']`
- Total Training Images: `500` (100 per class)

### Validation Dataset
- Classes Used: `['Airplane', 'Bus', 'Calm Down', 'Car', 'Church']`
- Total Validation Images: `200` (40 per class)

---

## Training Configuration

- **Epochs**: `50`
- **Batch Size**: `10`
- **Image Size**: `1088` (Max stride: `32`)

---
