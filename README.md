# Semantic Segmention with U-Net to spot Nuclei in Micrscopic images
## Overview:
The project focuses on perfroming semantic segmentation using the U-Net architecture to identify nuclei in microscopic images. The resulting output image contains only two colors: one representing nuclei and the other representing everything else, making it a binary classification task.

## Dataset:
The dataset contains images of cell nuclei obtained from microscopy. It consists of:
- Training Set: Microscopy images with labeled masks for nuclei.
- Test Set: Microscopy images without labels for segmentation evaluation. 


The dataset can be downloaded from [2018 Kaggle competetion page](https://www.kaggle.com/competitions/data-science-bowl-2018/overview)

## U-Net Architecture:
The U-Net is a convolutional neural network architecture designed for biomedical image segmentation. It employs an encoder-decoder structure:
- Encoder: Extracts features using convolutional and max-pooling layers.
- Decoder: Performs upsampling and combines with high-resolution features from the encoder using skip connections.

## Key Features:
- Data Preprocessing: Includes resizing images, normalizing pixel values.
- Model Architecture: U-Net implementation with TensorFlow/Keras.
- Training: Custom loss functions and metrics to handle imbalanced segmentation masks.
- Evaluation: Binary Cross Entropy Loss and Validation Accuracy for performance measurement.
- Callbacks: Early stopping and model checkpointing.

## Performance
- Training and validation accuracy of 95.4% and 96% respectively.

## Future Steps
- Select a dataset to perfrom semantic segmentation of multi-class with Mean IOU and Dice coefficient for performance measurement.

## Acknowlegment
- U-Net architecture by Ronneberger et al., "[U-Net: Convolutional Networks for Biomedical Image Segmentation](https://arxiv.org/abs/1505.04597)".
- Video lectures on U-Net by [DigitalSreeni](https://www.youtube.com/watch?v=azM57JuQpQI)
