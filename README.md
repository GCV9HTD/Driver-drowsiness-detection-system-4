# Driver-drowsiness-detection-system
This is a Python code for drowsiness detection system using Haar Cascades. 
Here we have used the OpenCV library to monitor the real-time video of the driver and to detect the face and the eyes of the driver. 
We use the eye-aspect-ratio (EAR) to compute the ratio between the vertical and the horizontal distance of the eyes to determine if the eyes are open or closed.
Haar Cascades are used in this project to detect the face and the eyes from the real-time video captured by the camera using the data from the face_landmarks DAT file.
Once the eyes are detected in real-time, their EAR is computed. If the value for each frame, is computed to be less than the threshold value, then a boolean is set to 'TRUE' to indicate that the eyes are closed.
If the boolean value is TRUE for consecutive 5 frames, the driver is detected to be drowsy by the system.
This project can be supplemented with a raspberry pi, its camera module and an alarm system to monitor the driver and alert him/her in real time.
