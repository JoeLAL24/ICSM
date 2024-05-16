# DMT

Code release for the paper `"An Information Calibration and Sliding Mining Network for Co-saliency Object Detection"`.

![image](https://github.com/JoeLAL24/ICSM/assets/100739402/630dee0d-c63c-4595-8774-5201a189efb8)

## Abstract

Co-saliency object detection simulates human visual attention behavior,which is committed to detecting the common attractive objects shared by each image in a set of images. There are two problems in many co-saliency object detection methods. One is that low-level high-resolution encoding features and high-level low-resolution decoding features are fused only by adding operation, resulting lots of information loss in the process of image size increasing and channel number compression. The other one is that some feature extraction modules brings improved accuracy while ignoring local information and it is computationally heavy. In this paper, we propose a novel end-to-end Information Calibration and Sliding Mining Co-saliency Detector (ICSM) for co-saliency object detection. In the stage of encoding features and decoding features fusion, we propose a Multistage Calibration Correlation (MCC) module. In MCC module, we calibrate the information from the features of different sizes and channel numbers to reduce the information loss when these features are fused, where a series of region-level modeling is carried out to preliminarily calculate the correlation between image pixels. Then, we propose the Sliding Region Mining (SRM) module, which converts pixel-level features into foreground and background contrast token features by modified Transformer. It uses these token features to search for synergistic saliency object across multiple images and to suppress background interference while reducing computing costs. Extensive experiments show that our model achieves better performance than the excellent Co-saliency object detection methods in recent years under the three most popular benchmark datasets.

## Result

![image](https://github.com/JoeLAL24/ICSM/assets/100739402/739c5add-7b22-47c0-95ab-8d18bf807530)

![image](https://github.com/JoeLAL24/ICSM/assets/100739402/f000747e-2580-4d44-b9b4-5d8b1aa0b481)

## Environment Configuration

- `pip install -r requirements.txt`
