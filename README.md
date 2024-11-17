# Day-Night-Image-Translations-using-CycleGAN
Day-Night Image Translations using CycleGAN

This notebook uses Cycle GANs to trying to convert high resolution Day cityscapes images to Night images and vice versa. The dataset consists of high resolution Day and Night images. Cycle GANs allows us to use the dataset without any explicit image-target image pairs, by using cycle consistancy loss to ensure that the images retain the semantic and structural components. Hence Cycle GAN builds on top of Pix2Pix GANs, with an additional Cycle Consistency loss.

Paper: https://www.cs.cmu.edu/~junyanz/projects/CycleGAN/CycleGAN.pdf


Cycle GANs provide the approach to translate an image from source domain X to target domain Y in absence of paired examples. 
The goal is to learn a mapping G: X-> Y , and inverse mapping F: Y -> X , and introduce a cycle consistancy loss to enforce F(G(X)) = X and G(F(Y_hat)) = Y_hat.

The problem that Cycle GANs address can be classified as Image to Image translation. While there are other methods that address the problem with image-target pairs, obtaining these pairs is difficult and expensive. This method is applied for the tasks of style transfer, object transfiguration, and attribute transfer and claims to outperform baseline approaches.
