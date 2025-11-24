# Road Segmentation Using MobileNetV2

This project implements a road segmentation model using MobileNetV2 for efficient pixel-level classification of road areas in images.

## Data Preparation

The dataset includes road scene images with corresponding masks that highlight road areas. should set the file paths in the notebooks so each image is correctly paired with its mask for training and evaluation.

The dataset, including training images, testing images, and ground truth masks, can be accessed from the following link:

[https://drive.google.com/drive/folders/13ypfoSRW-D65os-DB1cL4sTPximTPo4u?usp=drive_link](https://drive.google.com/drive/folders/13ypfoSRW-D65os-DB1cL4sTPximTPo4u?usp=drive_link)

## Preprocessing

Preprocessing involves loading the images and masks, resizing if necessary, normalizing pixel values, and applying data augmentation techniques to improve model generalization. The masks are binarized to explicitly represent road and non-road areas for training.

## Training

The training process uses an encoder-decoder network architecture with MobileNetV2 as the backbone to extract features efficiently. The model is trained on the prepared dataset using pixel-wise loss functions suitable for segmentation tasks. Training continues until convergence with checkpoints to save model weights.

## Evaluation

The trained model is evaluated on a test set using metrics such as mean Intersection over Union (mean IoU) and Dice coefficient. The model achieved an average mean IoU of 0.750944 and an average Dice score of 0.680053, indicating strong segmentation performance.



