# UML-Project
## Denoise images using Autoencoders

### Problem Statement:-
In the realm of digital document processing, noise often infiltrates images due to various factors such as scanning artifacts, low-quality cameras, or environmental conditions. This noise not only impedes readability but also hinders subsequent processing tasks such as optical character recognition (OCR) or document classification.

### Objective:-
The objective of this project is to develop an effective solution for denoising document images using autoencoder neural networks. Autoencoders are a type of artificial neural network trained to copy their input data to the output while compressing the data representation into a lower-dimensional space. By leveraging the capabilities of autoencoders, we aim to restore clarity and remove noise from the document images, thereby enhancing their quality for downstream tasks.

### About Dataset:-
train.zip contains the images that we will train our deep learning autoencoder on. These images contain text to which noise has been added. Our aim is to build an autoencoder neural network that will denoise those images.
test.zip contains the images that we will use to test our neural network once it has been trained. We will try to get clean images as the output by cleaning the noise from the test images.
train_cleaned.zip contains the same images as the train images but without the noise. We will use these images as targets to train our network.
We will train our autoencoder neural network on the noisy train images. While doing so, we will try to eliminate the noise by posing the clean train image as the targets. After that, when we will feed our network with the noisy test images, we should be able to get clean images as output. 
