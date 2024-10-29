# Eye-Blinking-Detection
This project detects eye blinking using a webcam feed. By analyzing the landmarks around the eyes, it determines whether the eyes are open or closed, displaying a "BLINKING" message when a blink is detected.

Features:
- Real-time face and eye landmark detection
- Calculates eye aspect ratio to determine eye status
- Shows messages based on eye status (Open or Blinking)
  
Requirements:
- Python 3.x
- OpenCV
- Numpy
- Dlib
- shape_predictor_68_face_landmarks.dat (Dlib facial landmark model file)

# Code Explanation
- cap = cv2.VideoCapture(0) starts the webcam feed.
- detector and predictor are used to detect facial landmarks.
- Landmark points around the eyes are used to calculate the eye aspect ratio.
- If the ratio exceeds a threshold, it is interpreted as a "BLINKING" state; otherwise, the eyes are marked as "Open."
  
# How It Works
- Detects the face and eye landmarks in each video frame.
- Calculates the horizontal and vertical distances between specific eye landmarks.
- Based on the ratio of these distances, determines the state of the eyes.
  
# Sample Output
- Open: The eyes are open.
- BLINKING: A blink is detected.
