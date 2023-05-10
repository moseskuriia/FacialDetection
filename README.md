

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

1. Data collection: The project uses image dataset from [CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)

2. Data preprocessing: The dataset is split into training, validation, and test sets (70% train, 30% test, and the test set is further split into 50% test and 50% validation). A batch generator function is created to yield batches of a specified size from the given sequence.

3. Model development: A Variational Autoencoder (VAE) and Super-Resolution Generative Adversarial Network(SRGAN) will be used for facial image reconstruction and detection. The VAE AND SRGAN will be trained on the preprocessed data using deep learning frameworks such as TensorFlow or PyTorch.

4. Model evaluation: The performance of the trained model will be evaluated using metrics such as accuracy, precision, and recall, and the model will be iteratively refined based on the results of the evaluation.

5. Deployment: The trained model will be deployed using Flask, a web framework for Python, to create a web interface that allows users to upload images and receive reconstructed images or detection results. The deployment will be hosted on a cloud server such as Amazon Web Services (AWS) or Google Cloud Platform (GCP).

## Results

1. VAE results 

![download (5)](https://user-images.githubusercontent.com/116640061/235289531-8b72dcbd-7e30-4360-863a-7474363203c8.png)

Upon visually inspecting the reconstructed images, we obtain a qualitative assessment of the VAE's performance. Comparing the original images to their corresponding reconstructions allows us to gauge the VAE's ability to capture crucial features and details within the input images. Our VAE model generated reconstructions that were strikingly similar to the original images in aspects such as facial features, color, and overall structure. This comparison highlights the model's proficiency in learning significant representations of the data, serving as a foundation for future model optimizations and enhancements.

![download (6)](https://user-images.githubusercontent.com/116640061/235289556-755e9e2e-08b4-4b97-85d9-e0022cb990ae.png)

2. SRGAN Results 

![download (8)](https://user-images.githubusercontent.com/116640061/235289613-53cad76c-e046-4a6e-90b3-40cc7c88a411.png)

The SRGAN model produced impressive results on the CelebA dataset, achieving an adversarial loss of 0.08 and a content loss of 0.93. These metrics indicate that the generated images are of good quality and resemble the original images. Visually, the generated images are clear enough and have recovered more detail than the low-resolution images.

## Conclusions

In conclusion, the implemented SRGAN model has performed very well on the CelebA dataset, achieving low adversarial loss and content loss scores. These results indicate that the SRGAN model is an effective approach for single-image super-resolution, and has the potential to be used in a variety of applications where high-resolution images are required.

## Next Steps
Based on the results, We would recommend the following:

1. Upgrade existing CCTV cameras with high-resolution cameras: While the SRGAN model can enhance low-resolution images to a certain extent, it is still limited by the quality of the original images. Therefore, upgrading existing CCTV cameras with high-resolution cameras would provide better input images for the SRGAN model to work with, resulting in even better super-resolved images.

2. Deploy SRGAN models on-site or in the cloud: Depending on the size of the CCTV network, it may be more efficient to deploy the SRGAN model on-site or in the cloud. This would allow for faster processing of the images and quicker access to the super-resolved images. Additionally, deploying the model in the cloud would allow for scalability and ease of maintenance.

3. Combine SRGAN with object detection algorithms: Object detection algorithms can be used to identify specific objects or people in the super-resolved images. This would improve the accuracy and effectiveness of the CCTV system in identifying potential security threats.

4. Train staff on interpreting super-resolved images: Super-resolved images may contain more detail and information than the original images, which could potentially aid in investigations. Therefore, it is important to train staff on how to interpret and analyze these images effectively.

5. Consider privacy and ethical concerns: While the SRGAN model can enhance images for security purposes, it is important to consider privacy and ethical concerns. Law enforcement agencies should ensure that they have policies and procedures in place to protect the privacy of individuals and to use the technology ethically and responsibly.


For More Information

See the full analysis in the [Jupyter Notebook](https://github.com/moseskuriia/Visual-Intelligence/blob/main/Visual%20Intelligence%20.ipynb) or review this [presentation](https://github.com/moseskuriia/Visual-Intelligence/blob/main/Visual%20Intelligence%20Presentation%20.pdf).

For additional info, you can contact 
* [Moses Kuria](https://github.com/moseskuriia)
* [Eva Moisasi](https://github.com/Eva-Moisasi)
* [Nobert Akwir](https://github.com/NobertAkwir)
* [Nurulain Abdi](https://github.com/Nurul-ain2022)
* [Alice Wamuyu](https://github.com/AliceWamuyu)



Repository Structure

├── data

├── images

├── README.md

├── Presentation.pdf

└── visual intelligence.ipynb

