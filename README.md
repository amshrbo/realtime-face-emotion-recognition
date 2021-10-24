# realtime-face-emotion-recognition
__Done into two main steps__:         
> 1. __Face-detection:__ from the video source using OpenCV and haarcascade algorithm.
> 2. __Emotion recognition:__              
    - __First solution:__ Using a model trained on [FER-2013 dataset](https://www.kaggle.com/msambare/fer2013) with Tensorflow.         
    - __Second solution:__ I've used [DeepFace package](https://github.com/serengil/deepface) as a prefabricated solution.      

## Table of contents
- [The dataset and its challenges](#dataset)
- [High level roadmap for the project](#project-roadmap)
- [The mentioned solutions and demos for how to tackle the problem](problem-solutions-and-demos)
- [Technologies Used in this project](#technologies)
- [What did I learn from this project](#what-did-i-learn)
- [LICENCSE](#license)

### Dataset
[__FER 2013__](https://www.kaggle.com/msambare/fer2013) Dataset:
> The data consists of 48x48 pixel grayscale images of faces. The dataset consists of 7 unblanced classes    

__Note that the data has lots of pitfalls:__ 
> __So don't expect a high accuracy on training I got about 70% on the validation set__

- __Imbalanced classes__: you can notice from the below charts that the `happy` class represents __25%__ of the data               
    <img src="./assets/imbalncing_charts.png" alt="imbalanced" width="750" height="427"/>
- Some other problems exist in the dataset like __occulsion, contrast variation and Intra class variation__:
    <img src="./assets/sample_imgs_fer2013.png" alt="imbalanced" width="750" height="427"/>

### Project Roadmap
![roadmap](./assets/realtime_emotion_detection_digram.png)

### Problem solutions and demos
__Solutions:__                     
- [Realtime emotion recognition using the trained model](./fer_solution/realtime_emotion_recognition.ipynb)
- [Realtime emotion recognition using DeepFace](./deepFace_solution/realtimeFaceEmotionRecognition_using_deepface.ipynb)

__Demos:__              
- [Emotion recognition Model training in the fer-2013 dataset](./fer_solution/emotion_recognition_model_training)
- [Realtime face detection demo](./src/realtime_face_detection_demo.ipynb)
- [Emotion recognition for multiple faces in a snigle image demo](./fer_solution/demo_for_multiple_faces_emotion_recognition.ipynb)

### Technologies 
- [Tensorflow 2.0](https://github.com/tensorflow/tensorflow)
- __Keras__
- [OpenCV](https://github.com/opencv)
- __Python__
- [DeepFace](https://github.com/serengil/deepface)

### Useful resources
- Fer-2013 dataset [link in kaggle](https://www.kaggle.com/msambare/fer2013)
- Realtime emotino recognition hypertuning mobilenet model [youtube video](https://www.youtube.com/watch?v=fkgpvkqcoJc)
- [PAZ a GitHub repo which contains different applications on computer vision](https://github.com/oarriaga/paz)

### Contacts
> - [LinkedIn](https://www.linkedin.com/in/amshrbo)
> - Email: _amshrbo@gmail.com_
> - [Twitter](https://twitter.com/amshrbo)

### LICENSE
[***GNU GPL V3***](./LICENSE)
