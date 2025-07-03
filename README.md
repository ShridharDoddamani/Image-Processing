# Image-Processing
Project on image processing
This project aims at recognizing the ASL Static Sign Language using the concept of Neural
Networking. The neural network used to build this model is YOLO v5. This was implemented
using pytorch1.9.0 in Google Colab. The GPU used is CudaDevice. The properties of the same
are : Name- 'Tesla T4', Major- 7, Minor-5, Total memory- 15109MB, Multi processor count- 40.

Technical specifications:
● Yolo version-5
● GPU: CudaDevice
● Model Depth Multiple - 0.33
● Layer Depth Multiple - 0.50
Model Summary:
● 283 layers
● 7346792 parameters
● 7346792 gradients
● 17.1 GFLOPs
Scaled weight_decay = 0.00046875
Optimizer groups: 62 .bias, 70 conv.weight, 59 other
Hyperparameters: lr0=0.01, lrf=0.2, momentum=0.937, weight_decay=0.0005,
warmup_epochs=3.0, warmup_momentum=0.8, warmup_bias_lr=0.1, box=0.05, cls=0.5,
cls_pw=1.0, obj=1.0, obj_pw=1.0, iou_t=0.2, anchor_t=4.0, hsv_h=0.015, hsv_s=0.7,
hsv_v=0.4, translate=0.1, scale=0.5, fliplr=0.5, mosaic=1.0
Libraries used
Base Libraries:
➔ matplotlib
➔ numpy
➔ opencv-python>
➔ Pillow
➔ PyYAML
➔ scipy
➔ torch
➔ torchvision
➔ tqdm
Logging Libraries:
➔ tensorboard
Plotting Libraries:
➔ seaborn
➔ pandas
Dataset

Link: https://mega.nz/folder/nF5TESLZ#NbGRqCzZTunbY49LCNrp_g
Details of the entire dataset:
No. of classes - 35
Total Images - 15472

Details of the images used for training:
No. of classes - 5 [‘Airplane’, ’Bus’, ’Calm Down’, ’Car’, ’Church”]
Total Images - 500 (100 per class)

Details of the images used for Validation:
No. of classes - 5 [‘Airplane’, ’Bus’, ’Calm Down’, ’Car’, ’Church”]
Total Images - 200 (40 per class)

Epochs - 50
Batch Size - 10
Image Size - 1088 (Max stride = 32)


