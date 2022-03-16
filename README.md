Face Mask Detection

Face Mask Detection System built with OpenCV, Keras/TensorFlow using Deep Learning and Computer Vision concepts in order to detect face masks in static images as well as in real-time video streams.
                               Python contributions welcome Forks Stargazers Issues LinkedIn

                                    Live Demo

👇 Support me here!
Buy Me A Coffee

😇 Motivation
Amid the ongoing COVID-19 pandemic, there are no efficient face mask detection applications which are now in high demand for transportation means, densely populated areas, residential districts, large-scale manufacturers and other enterprises to ensure safety. The absence of large datasets of ‘with_mask’ images has made this task cumbersome and challenging.



⚠️ TechStack/framework used
OpenCV
Caffe-based face detector
Keras
TensorFlow
MobileNetV2
⭐ Features
Our face mask detector doesn't use any morphed masked images dataset and the model is accurate. Owing to the use of MobileNetV2 architecture, it is computationally efficient, thus making it easier to deploy the model to embedded systems (Raspberry Pi, Google Coral, etc.).

This system can therefore be used in real-time applications which require face-mask detection for safety purposes due to the outbreak of Covid-19. This project can be integrated with embedded systems for application in airports, railway stations, offices, schools, and public places to ensure that public safety guidelines are followed.

📁 Dataset
The dataset used can be downloaded here - Click to Download

This dataset consists of 4095 images belonging to two classes:

with_mask: 2165 images
without_mask: 1930 images
The images used were real images of faces wearing masks. The images were collected from the following sources:

Bing Search API (See Python script)
Kaggle datasets
RMFD dataset (See here)
🔑 Prerequisites
All the dependencies and required libraries are included in the file requirements.txt See here

🚀  Installation
Clone the repo
$ git clone https://github.com/chandrikadeb7/Face-Mask-Detection.git
Change your directory to the cloned repo
$ cd Face-Mask-Detection
Create a Python virtual environment named 'test' and activate it
$ virtualenv test
$ source test/bin/activate
Now, run the following command in your Terminal/Command Prompt to install the libraries required
$ pip3 install -r requirements.txt
💡 Working
Open terminal. Go into the cloned project directory and type the following command:
$ python3 train_mask_detector.py --dataset dataset
To detect face masks in an image type the following command:
$ python3 detect_mask_image.py --image images/pic1.jpeg
To detect face masks in real-time video streams type the following command:
$ python3 detect_mask_video.py 

Internet of Things Device Setup
Expected Hardware
Raspberry Pi 4 4GB with a case
5MP OV5647 PiCamera from Arducam
Getting Started
Setup the Raspberry Pi case and Operating System by following the Getting Started section on page 3 at documentation/CanaKit-Raspberry-Pi-Quick-Start-Guide-4.0.pdf or https://www.canakit.com/Media/CanaKit-Raspberry-Pi-Quick-Start-Guide-4.0.pdf
With NOOBS, use the recommended operating system
Setup the PiCamera
Assemble the PiCamera case from Arducam using documentation/Arducam-Case-Setup.pdf or https://www.arducam.com/docs/cameras-for-raspberry-pi/native-raspberry-pi-cameras/5mp-ov5647-cameras/
Attach your PiCamera module to the Raspberry Pi and enable the camera
Raspberry Pi App Installation & Execution
Run these commands after cloning the project

Commands	Time to completion
sudo apt install -y libatlas-base-dev liblapacke-dev gfortran	1min
sudo apt install -y libhdf5-dev libhdf5-103	1min
pip3 install -r requirements.txt	1-3 mins
wget "https://raw.githubusercontent.com/PINTO0309/Tensorflow-bin/master/tensorflow-2.4.0-cp37-none-linux_armv7l_download.sh"	less than 10 secs
./tensorflow-2.4.0-cp37-none-linux_armv7l_download.sh	less than 10 secs
pip3 install tensorflow-2.4.0-cp37-none-linux_armv7l.whl	1-3 mins
