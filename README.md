# Gender and Age Detection
To build a gender and age detector that can approximately guess the gender and age of the person (face) in a picture or through webcam.

# About the Project :
In this Python Project, I had used Deep Learning to accurately identify the gender and age of a person from a single image of a face. I used the models trained by Tal Hassner and Gil Levi. The predicted gender may be one of ‘Male’ and ‘Female’, and the predicted age may be one of the following ranges- (0 – 2), (4 – 6), (8 – 12), (15 – 20), (21 - 25), (26 – 32), (38 – 43), (48 – 53), (60 – 100) (8 nodes in the final softmax layer). It is very difficult to accurately guess an exact age from a single image because of factors like makeup, lighting, obstructions, and facial expressions. And so, I made this a classification problem instead of making it one of regression.

# Additional Python Libraries Required :
OpenCV
   pip install opencv-python
argparse
   pip install argparse
   
# The contents of this Project :
opencv_face_detector.pbtxt
opencv_face_detector_uint8.pb
age_deploy.prototxt
age_net.caffemodel
gender_deploy.prototxt
gender_net.caffemodel

a few pictures to try the project on
gender_age_detection.py

For face detection, we have a .pb file- this is a protobuf file (protocol buffer); it holds the graph definition and the trained weights of the model. We can use this to run the trained model. And while a .pb file holds the protobuf in binary format, one with the .pbtxt extension holds it in text format. These are TensorFlow files. For age and gender, the .prototxt files describe the network configuration and the .caffemodel file defines the internal states of the parameters of the layers.

# Usage :
Download my Repository
Open your Command Prompt or Terminal and change directory to the folder where all the files are present.

# Detecting Gender and Age of face in Image Use Command :
python gender_age_detection.py --image <image_name>
  
Note: The Image should be present in same folder where all the files are present

# Detecting Gender and Age of face through webcam Use Command :
python gender_age_detection.py

Press Ctrl + C to stop the program execution.

# Working:
Watch the video

![Screenshot (54)](https://github.com/darshkantaria/Ineuron.ai_Internship/assets/91107260/47af6ec0-e3de-4cc0-b886-3c75a770f926)
