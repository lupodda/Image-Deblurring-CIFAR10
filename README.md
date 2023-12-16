# Image Deblurring - Luigi Podda

## Introduction
The aim of this project is to build a deep learning model in order to remove gaussian blur and gaussian noise from images.

**Wide Inference Networks (WIN)** are convolutional neural networks, with a wide structure, that in particular are capable of learning pixel-distribution features from noisy data. Moreover, WIN predict reconstructed images from features learned by pixel-distributions. This type of networks work better when the noise is higher, due to the fact that distributions are more similar under higher degree of noise.

In this analysis we compare three different architectures that have a very similar structure: **WIN5, WIN5-R, WIN5-RB**.
* WIN5 is a Wide Inference Network with 5 layers;
* WIN5-R is a Wide Inference Network with 5 layers that deploys a skip connection (i.e. it uses Residual Learning); 
* WIN5-RB is almost equivalent with respect to WIN5-R, adding a Batch Normalization layer for each of the previous layers; 

![](https://www.researchgate.net/profile/Peng-Liu-68/publication/318528076/figure/fig2/AS:527642848120832@1502811266274/Architectures-a-WIN5-b-WIN5-R-c-WIN5-RB.png)

The main reference for this project is available at the following link:
https://arxiv.org/pdf/1707.09135.pdf

To replicate all the experiments done, the three models' weights (in hdf5 format) are available at the following link:
https://drive.google.com/drive/folders/1lk1GScDehsZAs0c1vcTbwRPhH1qQT0TV?usp=sharing
