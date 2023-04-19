

![Git pic](https://user-images.githubusercontent.com/116640061/233091079-37df1297-2af9-482f-bc0a-6cc63e2d792b.png)


# Visual Intelligence: Enhancing Image Analysis for Surveillance and Investigations

##### Authors : 

* [Moses Kuria](https://github.com/moseskuriia)
* [Eva Moisasi](https://github.com/Eva-Moisasi)
* [Nobert Akwir](https://github.com/NobertAkwir)
* [Nurulain Abdi](https://github.com/Nurul-ain2022)
* [Alice Wamuyu](https://github.com/AliceWamuyu)


## Overview


Visual Intelligence is an essential tool for surveillance and law enforcement agencies, providing critical information for investigations and public safety. However, compromised images, including low resolution, poor lighting, and motion blur, often limit the usability of visual evidence. To address this gap in the market, we have developed a solution using Variational Autoencoder (VAE) technology to reconstruct and enhance degraded images, providing law enforcement agencies with an advanced tool for image analysis.


## Business Problem



Law enforcement agencies and security organizations rely heavily on visual evidence in the form of images and videos for investigations and crime prevention. However, these images are often compromised due to various factors, including low quality, degradation, and blur. This makes it difficult to extract critical information from visual evidence, potentially hindering investigations and compromising public safety.


## Data

For  image reconstruction, we will use the [CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) dataset. This dataset contains over 200,000 celebrity face images with consistent alignment and cropping, making it suitable for facial image reconstruction tasks. Additionally, we will need a dataset of positive examples (i.e., of faces) and a dataset of negative examples (i.e., of things that are not faces) to train our facial detection models. For this, we will use the CelebA dataset as the positive training data and ImageNet as the negative training data, which is a large-scale dataset with many images across many different categories. We will take negative examples from a variety of non-human categories.

## Methods

1. Data collection: The project uses a combination of publicly available and private image datasets from various sources, including law enforcement agencies and surveillance cameras.

2. Data preprocessing: The collected data will be preprocessed using techniques such as resizing, normalization, and augmentation to enhance the quality of the images and ensure consistency across the dataset.

3. Model development: A Variational Autoencoder (VAE) will be used for facial image reconstruction and detection. The VAE will be trained on the preprocessed data using deep learning frameworks such as TensorFlow or PyTorch.

4. Model evaluation: The performance of the trained model will be evaluated using metrics such as accuracy, precision, and recall, and the model will be iteratively refined based on the results of the evaluation.

5. Deployment: The trained model will be deployed using Flask, a web framework for Python, to create a web interface that allows users to upload images and receive reconstructed images or detection results. The deployment will be hosted on a cloud server such as Amazon Web Services (AWS) or Google Cloud Platform (GCP).

## Results

## Conclusions


## Next Steps



For More Information

See the full analysis in the [Jupyter Notebook]() or review this [presentation]().

For additional info, contact 


Repository Structure

├── data

├── images

├── README.md

├── Presentation.pdf

└── vae.ipynb

