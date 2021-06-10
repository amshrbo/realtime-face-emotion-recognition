# realtime-face-emotion-recognition
Real time **emotion recognition** for person's face using opencv for face detection from the video source and the model is trained on FER2013 dataset using tensorflow and transefer learning, the data set consistis of seven classes (happy, sad, angry, disgusted, surprized, fearful, and neutral).
## Table of contents
- [Installation](#Installation)
- [Technologies Used in this project](#Technologies)
- [The dataset and their challenges](#Dataset)
- [My strategy for solving this problem](#strategy)
- [What did I learn from this project](#what-did-I-learn)
- [LICENCSE](#license)


## Installation
- Run It using docker You just simply 

1. `Docker pull 'The DockerHub link For the project'`
1. `docker run -it ImageName`

### Technologies 
- [Tensorflow 2](https://github.com/tensorflow/tensorflow)
- [opencv](https://github.com/opencv)
- Python

### Dataset
Here I'm gonna use the [FER 2013](https://www.kaggle.com/msambare/fer2013) Dataset 

#### Pitfalls of this dataset
1. Imbalanced:
    - Classes don't have the same number of Imgs as the most dominanet class is the happy class
2. Intra class variation
    - There are different type of Images like photos, paintings, and cartoon
3. Contrast variation
    - There are different levels of contrast in the images, going from too dark to too bright images
4. Eyeglasses
5. Occulsion
    - Like if someone convring his face with hands
6. Outliers 
### Stratgey
- Using opencv for detecting faces
- Transefer learning

### What did I learn
- Working with transefer learning 
- Data Augmentation

### Useful resources
- Here are some Useful resiources you can use
### LICENSE
[***GNU GPL V3***](./LICENSE)