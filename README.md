# DLProject

Authors: Lahav Barak & Gali Eytan

* [Introduction](#introduction)
* [How to Use](#how-to-use)
* [Results](#results)

## Introduction
This repo is part of a student project in deep learning course.
This project attempts to improve upon the method of image generation with encoder-decoder system by adding a layer of Generative Adversarial Network (GAN).
Encoder-Decoder system takes a dataset of images (we used MNIST), encodes it into a 2d space called latent-space, and can later decode it back into image space.
after learning the relations between image space and latent space, the decoder is able to produce new images by getting points in latent space.

GAN employs a generator and discriminator. the generator creates fake images and feeds them to the discriminator, which is also provided with real images. the discriminator then attempts to identify whether an image is fake or real.
The training process of the GAN makes the generator learn to fool the discriminator better, while the discriminator learns to tell fake images better from real imagery.

This project uses the Encoder-Decoder system as the generator for the GAN and attempts to use this method to improve the decoder's ability to reproduce better images.

The second part of this project is to add a classifier after the encoder which learns to predict the label of the data given the latent space coordinates. The classifier learns it's task together with the Vae-Gan and optimizes the encoder to give more separable representation throughout the learning process.

The training routine used is special and designed specifically for this architecture, The first part is to train the Discriminator, and The second part is to train both VAE with classifier and The Discriminator (while training the Discriminator more due to its lower learning rate. In the last part of the training increase the Kl-divergence loss term weight so the latent space will shrink back and hopefully maintain it's separability.

## How to Use
1. clone this github repo:
   ```
   git clone https://github.com/LahavBarak/DLProject
   ```
   or download DeepProject.ipynb directly
   make sure to pip install all libraries and (optionally) the trained models in the same directory as the ipynb file.
   To train the discriminator alone, fake data is needed, it can be found in the pre-generated library inside the data section.
3. run notebook cell-by-cell or download trained models and plot their performence
   There are cells used to load and plot the model's performances in the end of the Python file.
   Note that inside the "plot_latent_with_eval" function there are various options for models used to check data separability by the accuracy of different classifiers like Knn, logistic regression, SVM, etc, and also two seperability indexes to choose from.
.00

.

.

.

.


.

.

.



...

## Results
.


.

.

.

.

.

.

.

.

.

.

.

.

.

.

.

.

.



.
