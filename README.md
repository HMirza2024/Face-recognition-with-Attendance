Face Recognition Attendance System
-
A simple Python script that uses face recognition to track attendance via a webcam. It identifies people, logs their names and timestamps in a CSV file, and shows who's present on the video feed.

Features
-
1. Detects faces in real-time using a webcam.
2. Recognizes known faces and logs attendance in a CSV file (e.g., 2025-09-06.csv).
3. Displays names on the video feed for recognized people.
4. Stops when you press the 'q' key.

Requirements
-
1. Python 3.6 or higher
2. Libraries:
- opencv-python
- face_recognition
- numpy

Install them with:
-
pip install opencv-python face_recognition numpy

Setup
-
A. Add Face Images:
-
1. Put images of people to recognize (e.g., person1.jpg, person2.jpg) in the same folder as the script.
2. Make sure all the files are in same folder and have the same name and spelling you wrote in the code.
3. Edit the script to include the correct names and image filenames in the known_face_names and file list.

B. Webcam:
-
- Ensure a webcam is connected. The script uses the default camera (cv2.VideoCapture(0)). Change the index if needed.
- Ensure that the camera quality and lighting in the room is good to recognize the face properly.

C. Output:
-
Attendance is saved in a CSV file named after the current date, like 2025-09-06.csv.

How to Run
-
- Run the script:python attendance_system.py
- The webcam will start, showing recognized faces with names on the screen.
- Attendance is logged in the CSV file (one entry per person).
- Press q to quit.

Example CSV Output
Person1,15:00:45
Person2,15:01:10

Notes
-
- Use clear, well-lit face images for better recognition.
- The script resizes webcam frames to speed up processing.
- Make sure images have only one face to avoid errors.

Contributing
-
Feel free to fork this repo and make improvements. Share your changes via pull requests!

Credits
-
Uses face_recognition (built on dlib) for face detection.
Uses opencv-python for webcam and image handling.
Thanks to all the python developers 
