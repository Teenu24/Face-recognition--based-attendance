Face Recognition

This repository features a facial recognition system implemented using OpenCV and Python, coupled with a Tkinter GUI interface. To test the code, simply execute the `train.py` file.

Technologies Used:
- OpenCV (Open Source Computer Vision)
- Python
- Tkinter GUI interface

The primary focus here is on developing a Facial Recognition-based Attendance Management System using OpenCV in Python. This system enables users to mark their attendance by facing the camera.

 Functionality:

1.  Initialization : Upon running `train.py`, a window prompts the user to enter an ID and Name.

2.  Image Capture : After entering the ID and Name, clicking the "Take Images" button opens the computer's camera to capture image samples of the person. These images are saved in the "TrainingImage" folder. Additionally, the provided ID and Name are stored in a CSV file named "StudentDetails.csv" within the "StudentDetails" folder.

3.  Training : Once a sufficient number of images (60 in this case) are captured, clicking the "Train Image" button initiates the training process. The system trains itself using the captured images and generates a "Trainer.yml" file, which is saved in the "TrainingImageLabel" folder.

4.  Recognition : After the initial setup, clicking the "Track Image" button reopens the camera for facial recognition. If a face is recognized, the person's ID and Name are displayed on the image.

5.  Attendance Logging : Upon exiting the recognition window by pressing "Q" or "q", the system logs the attendance of the recognized person. This information, including the Name, ID, Date, and Time, is stored in a CSV file within the "Attendance" folder and is also displayed in the window.

This system provides a convenient solution for facial recognition-based attendance management, combining the capabilities of OpenCV, Python, and Tkinter GUI for a user-friendly experience.
