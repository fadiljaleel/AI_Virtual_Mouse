# AI Virtual Mouse

Creating an AI virtual mouse using Python with libraries such as cv2, mediapipe, and pyautogui involves building a system that enables users to control the computer mouse cursor using hand gestures detected by a camera. Here's a brief description of how these libraries come together to achieve this:

OpenCV (cv2): OpenCV (Open Source Computer Vision Library) is used for computer vision tasks, particularly for accessing and processing image and video data from a camera. In this project, it's used to capture live video frames from a webcam and perform image analysis to detect hand movements and landmarks.

MediaPipe (mediapipe): MediaPipe is a library developed by Google that provides various pre-trained machine learning models for tasks like hand tracking. In the context of an AI virtual mouse, the mediapipe library is used to identify and track the position of a user's hand in real-time, along with key landmarks on the hand, such as the fingertips and palm.

PyAutoGUI (pyautogui): PyAutoGUI is a Python library that allows you to programmatically control the mouse and keyboard. It provides functions to move the mouse cursor, simulate mouse clicks, and perform keyboard actions. In this project, pyautogui is used to control the mouse cursor based on the hand movements detected by mediapipe.

Here's how the process typically works:

The program uses cv2 to capture video frames from the webcam.

It then employs the mediapipe library to detect and track the user's hand in each frame, identifying landmarks on the hand to determine its position.

Based on the hand's position and movements, the program calculates the corresponding mouse cursor movements and passes those to pyautogui.

As the user moves their hand, the mouse cursor on the screen follows the hand's movements, effectively creating a virtual mouse controlled by hand gestures.

This project can be a fun and interactive way to control a computer, and it's often used in applications like virtual presentations, gaming, or as an assistive technology for users with physical disabilities.
