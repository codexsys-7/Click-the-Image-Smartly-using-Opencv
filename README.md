# Click-the-Image-Smartly-using-OpenCV
Smart Selfie using OpenCV is an Interface which allows us to click selfies without touching our mobiles or any photo capturing devices. So, in this project we have used OpenCV to do the trick for us, where using the OpenCV’s video capture function and some haarcascade files integrated with flask web framework we have made a smart selfie web application where you can click images without touching any keys on your laptop. The photos are later saved on your device specified directory for later use.

![Laughing is the best medicine](https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fblog.indyhealthnet.org%2Fwp-content%2Fuploads%2F2013%2F04%2F9587539_ml1.jpg&f=1&nofb=1)

# Algorithm Overview
So, here we are using an OpenCV’s face, eye and smile cascade files to identify facial expressions of a person in the frame and then whenever it detects any smile or blink of an eye, it will capture the image. These cascading classifiers are like models which are trained on several positive similar images. So, in order to detect facial expression or eye of a person we use another cascade. detect Multiscale () function to detect the faces and draw a rectangle box over the face.

**Reference links:**
https://en.wikipedia.org/wiki/Cascading_classifiers, https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html

# How to Execute?
So, before execution we have some pre-requisites that we need to download or install i.e., anaconda environment, python and a code editor.
**Anaconda**: Anaconda is like a package of libraries and offers a great deal of information which allows a data engineer to create multiple environments and install required libraries easy and neat.

**Download link:**
https://www.anaconda.com/

**Python**: Python is a most popular interpreter programming language, which is used in almost every field. Its syntax is very similar to English language and even children and learning it nowadays, due to its readability and easy syntax and large community of users to help you whenever you face any issues.

**Download link:**
https://www.python.org/downloads/

**Code editor**: Code editor is like a notepad for a programming language which allows user to write, run and execute program which we have written. Along with these some code editors also allows us to debug, which usually allows users to execute the code line by line and allows them to see where and how to solve the errors. But I personally feel visual code is very good to work with any programming language and makes a great deal of attachment with user.

**Download links:**
https://code.visualstudio.com/Download, https://www.jetbrains.com/pycharm/download/#section=windows

# Steps to execute.
1. Install the prerequisites mentioned above.
2. open anaconda prompt and create a new environment.
  1. conda create -n "env_name"
  2. conda activate "env_name"
3. Install necessary libraries from requirements.txt file provided.
4. Run pip install -r requirements.txt or conda install requirements.txt 
(Requirements.txt is a text file consisting of all the necessary libraries required for executing this python file. If it gives any error while installing libraries, you might need to install them individually.)
5. Run app.py on your terminal.

# Data Description
The Data which we use here to detect faces, smile and blink of an eye can be downloaded from any external website or we can even load them from built in method such as, cv2.CascadeClassifier('Haarcascade_frontalface_default.xml'). XML is an Extensible markup language which is only used for structure and to store data. This file should be loaded and it will try to identify the facial features present on the human face and then the detect Multiscale () is responsible for identifying actual images on the frame and helps to draw the bounding box around them.

# Issues Faced.
1. we might face an issue while installing specific libraries.
2. make sure you have the latest version of python, since sometimes it might cause version mismatch.
3. Adding path to environment variables in order to run python files and anaconda environment in code editor, specifically in visual studio code.
4. make sure to change the path where your classifiers are saved.

# Evaluation metric.
None

### **Note:**
All the required data has been provided over here. Obviously, feel free to contact if you face any issues. abhiabhinay629@gmail.com
