
# Real-time Sign Language Detection


Real-time sign language detection model with __face detection__, identifying gestures like ThumbsUp', 'Love', 'Hello', 'ThankYou', 'Yes', 'No', and 'Victory'.

<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/1d7da493-5a34-4d08-ba46-b5f1786dcef3" alt="Title" width= "600" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/95a036b5-4515-47e5-84a8-d92eee5036d6" alt="Detections" width= "400" />



## Introduction

A real-time communication model based on SSD MobileNet V2. It efficiently detects faces and interprets common sign languages like 'ThumbsUp,' 'Love,' 'Hello,' 'ThankYou,' 'Yes,' 'No,' and 'Victory.' Trained with personalized data, SignSense is a practical and reliable tool for enhanced gesture recognition.


## About SSD MobileNet V2


SSD MobileNet V2 is a combination of __MobileNet V2__ and __Single Shot Multibox Detector__ (SSD), creating an efficient object detection framework. MobileNet V2 provides a lightweight yet effective CNN, and SSD allows the model to detect objects in real-time in a single pass.

SSD,  divides an image into a grid, predicts bounding boxes and class scores for each grid cell, and handles objects of different sizes by predicting at multiple scales.


## Key features

- _Real-time Gesture Recognition_: The model quickly recognizes sign languages, facilitating prompt communication.

- _Face Detection_: Integrated face detection improves contextual interpretation of gestures.

- _SSD MobileNet V2 Architecture_: The project employs a reliable object detection framework, balancing accuracy and speed.

- _Custom Dataset Training_: Fine-tuned with a personalized dataset for improved performance.

  
## Usage Instructions:

To get started with Sign Language Detection, follow these simple steps:

- Clone the repository to your local mac
hine.

- Install the required dependencies using `pip install`.

- Execute the file " __4. Model Deployment.ipynb__"



## SSD Architecture
It includes VGG-16 Architecture as initial layers. Adding Extra feature layers with skip connection to Detection heads( with each layer having different convolution )

Now, Multibox detector detectes the presence & location of different class objects ( >8k per class )

In final layer, NMS ( Non-Max Supression) is performed (i.e) Overlapping detection boxes are removed, and only highest IOU value box is kept for each detection.

<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/36dc9b64-f4de-4f50-90b6-429fc63eedab" alt="SSD Architecture" />

### Alternate Architecture
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/3d26ae19-fc94-46e7-93ea-fcb1c5a9a3ae" alt="Alternate Architecture" >
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/85263b58-6056-4bcd-b562-a1f5cdefb458" alt="Feature Extraction" width="500"/>
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/7929b1be-60f4-4214-b497-079e64a79b2c" alt="Multibox Detector" width="500"/>

### Feature Pyramid Network
Deep layers hold meaningful information about image and intital layers contains details of images. To bridge this gap, we use __Feature Pyramid Network__ (FPN)
We find semantics ( meaningful insights) and upsample back to higher resolution feature map.

<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/0c3e9776-3675-457d-91d5-2a59bf14296a" alt="FPN" width= "500" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/9c10ed8d-94f2-4d20-b94f-a20f21f851c3" alt="FPN" width= "400"  />


## Losses

<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/d8b3f9ff-83c2-48a1-b142-eacf4369383c" alt="classification_loss" width= "600" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/a92baf6e-6d12-4b69-865f-d6d764df25e7" alt="localization_loss" width= "600" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/0a412d4a-980f-49af-88ba-76e55fbd2207" alt="total_loss" width= "600" />


## Detections

<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/f23ef967-52b1-4601-a39a-5788dd826ae6" alt="face" width= "330" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/74771e71-68be-4b41-8299-d1932a852138" alt="hello" width= "330" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/bcc1dc93-ff1e-4165-9518-fc79024f4119" alt="love" width= "330" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/600d7e6a-8e59-4bb2-bfb8-5656404f417e" alt="no" width= "330" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/0767bf83-95c7-4e1e-88ea-e2c16e03bd11" alt="thankyou" width= "330" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/1c69fb45-501e-4692-9780-62cc60f4cd22" alt="thumbsup" width= "330" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/e76da2a6-7c11-4b97-8c01-294dd199c341" alt="victory" width= "330" />
<img src="https://github.com/ankursinghbisht/Real-Time-Sign_Language_Detector/assets/112644477/1a77da63-a48d-480b-b399-0c58b81cdd92" alt="yes" width= "330" />

## 🔗 Links
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/ankursinghbisht?tab=repositories)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ankursinghbisht/)


## Why I Built it?
I developed this project as a hands-on application of the computer vision basics I learned in lectures. Wanting to gain practical experience in object detection, I chose to implement a model using SSD MobileNet V2. The focus on detecting faces and interpreting sign languages, emerged as a natural extension of this learning journey.
My motivation was to apply theoretical knowledge to a real-world scenario, resulting in a functional and meaningful project.

