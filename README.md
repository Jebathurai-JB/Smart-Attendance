
# Smart Attendance using Face Recognition

#### This project is a smart attendance system that uses face recognition to detect and recognize students' faces and mark their attendance in an Excel sheet. The system is designed to simplify the attendance tracking process in classrooms or other educational settings.


## Problem Statement
Traditional attendance tracking methods involve manual entry and are time-consuming and prone to errors. With the increasing use of technology in education, a smart attendance system that uses face recognition can improve efficiency and accuracy.
## Face Recognition step by step

- Encode a picture using the HOG algorithm to create a simplified version of the image. Using this simplified image, find the part of the image that most looks like a generic HOG encoding of a face.
- Figure out the pose of the face by finding the main landmarks in the face. Once we find those landmarks, use them to warp the image so that the eyes and mouth are centered.
- Pass the centered face image through a neural network that knows how to measure features of the face. Save those 128 measurements.
- Looking at all the faces we’ve measured in the past, see which person has the closest measurements to our face’s measurements. That’s our match!
## How to use

We recommend to use python 3.7 for this project

**Create a virtual env:** 

`conda create -n <envname> python=3.7 -y` 

`activate <envname>`

**Clone the repository to your local machine:**

`git clone https://github.com/Jebathurai-JB/Smart-Attendance.git`

**Install the Dependencies:**

`pip install -r requirements.txt`

**Run the python file:**

`python iattendance.py`
