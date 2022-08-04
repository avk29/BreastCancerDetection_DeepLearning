# BreastCancerDetection_DeepLearning
Detecting breast cancer in mammogram images using a **Convolutional Neural Network (CNN)** based **Deep Learning model**.


## Problem Statement
- **Conventional detection** of breast cancer tumours in mammograms is a complex task that involves **clinical examination**, **radiological imaging**, and **pathology testing** and can only be accomplished by **domain experts**.

- These methods can be **automated** using **machine learning** which relies on **numerical attributes**. However, feature detection continues to be to be a **manual task** and can be further overcome using **deep learning approaches**.

- Hence, in my study I have focused on breast cancer detection using deep learning.


## Motivation
- Breast cancer is one of the most common cancer diseases among women. According to the **International Agency for Research on Cancer** (IARC), it accounts for **22.9%** of **invasive cancers** and **13.7%** of **cancer-related deaths** in women across the globe.

- Therefore, **early** and **accurate diagnosis** is critical as it can minimise the death rate and improve the prognosis of breast cancer.

- Since **manual diagnosis** is a **tedious task**, there exists an imperative need to automate breast cancer detection using deep learning.


## CNN Architecture Used
The Convolutional Neural Network (CNN) used comprises of the following architecture:
- **Three convolutional layers** with **16**, **32** and **64** **filters** respectively, using the **Rectified Linear Units (ReLU)** activation function.
- A **max pooling layer** after every convolutional layer with a **pool size** of **2**.
- After the series of convolutional and pooling layers, there exists **four fully connected layers** with **512**, **256**, **128** and **64** **neurons** respectively.
- Finally, in the CNN there exists an **output layer** with three neurons corresponding to three classes- **Normal, Benign and Cancer**.

The aforementioned CNN architecture can be graphically seen below.

![CNN_Architecture](https://user-images.githubusercontent.com/66971874/182913879-6d6288bd-bea5-463c-ae23-1341cb9002b7.png)


## Data Cleaning and Preprocessing
- At the onset, it was observed that most of the images in the image datasets were not in a standardised format. The images contained noise in terms of annotations and artefacts which were introduced due to malfunctioning of the device and/or poor illumination.

- Proceeding further, the annotated images were filtered out and the artefacts were eliminated by creating a uniform black background in a subset of the images.

- These processes were manually performed (leading to fewer samples) and in the future I would like to automate them.



## Experimentation
- Initially built a **Logistic Regression** based **Machine Learning model** using the numerical dataset with **~96% accuracy** (More details about the datasets used can be found in the end).

- To further automate **feature detection** and **extraction** process in mammogram images, built a **CNN based Deep Learning model** and **increased** its **accuracy** from **66.6%** to **88.8%**


## Conclusion
- My current work focused on automating the detection and classification of breast cancer in mammogram images using deep learning approaches.

- Due to the unavailablity of large and noise-free datasets, the experimentation that was based on a limited number of samples, manual noise-removal methods and different combinations of optimisers achieved a **maximum accuracy** of **88.8%**


## Future Directions
- In the future, I would like to automate the noise-removal process using sophisticated image processing techniques based on Median filters and Gaussian filters to name a few.

- The automation would lead to the generation of a large number of samples which would better train the CNN and ultimately lead to a better accuracy.


## Datasets Used
- [Breast Cancer Wisconsin (Diagnostic):](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29) 357 Benign, 212 Malignant samples.
- [The Mini–MIAS Database of Mammograms:](http://peipa.essex.ac.uk/info/mias.html) 56 Benign, 52 Malignant samples.
- [Mini-DDSM:](https://www.kaggle.com/datasets/cheddad/miniddsm) 2728 Normal, 3360 Benign, 3596 Cancer samples.


## About the Author
Hi, I am [Arjun Kohli](linkedin.com/in/arjunveerkohli). I'm currently pursuing a Computer Science major at Krea University. 

This project was built under the guidance of professor Pavan Kumar Perepu at Krea University. I also had constant help from my peer Ashutosh Verma (Computer Science major,  Krea University) throughout the course of the project.
