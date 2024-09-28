# Assignment 1 - Anime-Face-Generation-with-GANs

This repository contains the code for training a Generative Adversarial Network (GAN) to generate anime-style faces. The project uses PyTorch and torchvision for building and training the models. Below you'll find instructions on how to set up the project, a brief explanation of how the GAN works, and links to the Colab notebook and demonstration video.

Overview
This project demonstrates the use of a GAN to generate anime faces using a dataset of anime images. The GAN consists of a Generator and a Discriminator, which are trained simultaneously to create increasingly realistic anime faces.

Generator: Takes random noise (latent space vectors) as input and outputs synthetic anime face images.
Discriminator: Distinguishes between real anime face images and fake ones created by the Generator.

Features
* Anime Face Generation: The GAN generates anime face images based on random noise.
* Training with PyTorch: The GAN is trained using PyTorch, leveraging the GPU for faster computations.
* FID Evaluation: The quality of the generated images is measured using the Frechet Inception Distance (FID) score.
  
Getting Started
Follow these instructions to run the project on your local machine or directly in Google Colab.

Prerequisites
You will need the following libraries:

torch
torchvision
Pillow
pytorch-fid

Install the dependencies using: pip install torch torchvision Pillow pytorch-fid

Dataset
The dataset used for this project is a collection of anime faces. You can download a suitable dataset, such as Anime Face Dataset, and extract it into the /content/extracted_images/ directory.
https://www.kaggle.com/datasets/splcher/animefacedataset


Clone this repository:
* git clone ->>
* cd anime-face-gan
* Prepare your dataset by extracting it to the extracted_images/ folder.
* Run the training script: python train_gan.py

Alternatively, you can use the Google Colab notebook:
Anime Face GAN - Colab Notebook

Evaluating Performance
After training, you can compute the FID score to evaluate the quality of the generated images: python calculate_fid.py --real-dir /path/to/real_images --fake-dir /path/to/generated_images

Results
The generated anime faces can be visualized in real-time as the GAN trains. Here are some sample images after training:
Additionally, you can watch the progression of the generated images over epochs in the following video:

Video link: 


# Assignment 2 - Real-time-chat-Application 
