# UML-Project
## Denoise images using Autoencoders

### Problem Statement:-
In the realm of digital document processing, noise often infiltrates images due to various factors such as scanning artifacts, low-quality cameras, or environmental conditions. This noise not only impedes readability but also hinders subsequent processing tasks such as optical character recognition (OCR) or document classification.

### Objective:-
The objective of this project is to develop an effective solution for denoising document images using autoencoder neural networks. Autoencoders are a type of artificial neural network trained to copy their input data to the output while compressing the data representation into a lower-dimensional space. By leveraging the capabilities of autoencoders, we aim to restore clarity and remove noise from the document images, thereby enhancing their quality for downstream tasks.

### About Dataset:-
https://drive.google.com/file/d/1u9mskAV4bCrd3Q29H_6LRk5po1LQwTMW/view?usp=sharing 

train.zip contains the images that we will train our deep learning autoencoder on. These images contain text to which noise has been added. Our aim is to build an autoencoder neural network that will denoise those images.
test.zip contains the images that we will use to test our neural network once it has been trained. We will try to get clean images as the output by cleaning the noise from the test images.
train_cleaned.zip contains the same images as the train images but without the noise. We will use these images as targets to train our network.
We will train our autoencoder neural network on the noisy train images. While doing so, we will try to eliminate the noise by posing the clean train image as the targets. After that, when we will feed our network with the noisy test images, we should be able to get clean images as output. 

### About Autoencoders
An autoencoder is a type of artificial neural network used to learn efficient data codings in an unsupervised manner. The aim of an autoencoder is to learn a representation (encoding) for a set of data, typically for dimensionality reduction, by training the network to ignore signal “noise”. Along with the reduction side, a reconstructing side is learnt, where the autoencoder tries to generate from the reduced encoding a representation as close as possible to its original input, hence its name.![image](https://github.com/pandaroshni/UML-Project/assets/112866689/1b9c1758-421d-463c-816f-4c6cdc012ac9)

### About Librarie used

-> NumPy (np): NumPy is a powerful library for numerical computing in Python. It provides support for large, multi-dimensional arrays and matrices, along with a collection of mathematical functions to operate on these arrays efficiently. In image denoising, NumPy is used for array manipulation and mathematical operations on pixel values.
-> Pandas (pd): Pandas is a data manipulation and analysis library. It provides data structures and functions for easily handling structured data, such as tables or DataFrames. In image denoising, Pandas may be used for organizing and preprocessing image data if you're working with metadata or annotations associated with the images.
-> Matplotlib.pyplot (plt): Matplotlib is a plotting library for Python. The pyplot module provides a MATLAB-like interface for creating static, interactive, and animated visualizations. In image denoising, Matplotlib is commonly used to visualize the original images, noisy images, and denoised images for analysis and evaluation.
-> Zipfile: The zipfile module provides tools to create, read, write, append, and list a ZIP file. In image denoising, Zipfile could be used to handle compressed image datasets or to extract images from zip archives.
-> OS: The OS module provides a way of interacting with the operating system. It offers functions for creating, removing, and managing directories, files, and paths. In image denoising, the OS module might be used to navigate directories, load image files, or save denoised images.
-> CV2: OpenCV (Open Source Computer Vision Library) is a library of programming functions mainly aimed at real-time computer vision. The cv2 module in Python provides functions for image processing, manipulation, and analysis. In image denoising, OpenCV can be used for various tasks such as loading images, applying filters, and performing image enhancement techniques.
-> Scikit-learn (sklearn): Scikit-learn is a machine learning library for Python. It provides simple and efficient tools for data mining and data analysis, including classification, regression, clustering, and dimensionality reduction. In image denoising, Scikit-learn may be used for preprocessing steps or for evaluating the denoising model.
-> TensorFlow: TensorFlow is an open-source machine learning framework developed by Google. It provides a comprehensive ecosystem of tools, libraries, and community resources for building and deploying machine learning models, including deep learning models. In image denoising, TensorFlow is used for building, training, and evaluating deep learning models such as convolutional neural networks (CNNs) for denoising images.
