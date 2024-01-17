# Object-Based-Colour-Detection-Using-Open-CV
 This project is a Python script that captures video from a webcam in real-time and detects objects of different colors using the OpenCV library. The script applies color filtering based on predefined color ranges for various colors and then uses contour detection to identify and draw bounding boxes around objects of specific colors.

 Dependencies
    >numpy: A library for numerical operations.
    >cv2 (OpenCV): An open-source computer vision and machine learning software library.
Usage
 1.Install Dependencies:
    >pip install numpy opencv-python

 2.Run the Script:
    >python color_detection.py
   Make sure your webcam is connected and properly configured.

 3.Terminate the Script:
   Press 'q' key to close the application and release the webcam.

Color Detection Logic
  The script detects the following colors:

  Red
  Green
  Blue
  Yellow
  Purple
  Orange
  Pink
  Black
  Brown
  Hue
  Gold
  White
  Silver
  Dark Green
  Absence of Color (Black)
  Peach
  Violet
  Indigo


Color Filtering
    The script applies color filtering in the HSV (Hue, Saturation, Value) color space to detect specific color ranges for each target color. Masks are created for each color, and bitwise operations are performed to filter the color of interest.

Morphological Transformations
    Morphological operations, specifically dilation, are applied to the color masks to enhance the detection results and reduce noise.

Contour Detection
    Contours are found in each color mask using OpenCV's findContours function. Bounding rectangles are drawn around the detected contours, and the color name is displayed near the corresponding object.

User Interaction
    The application runs in a continuous loop, capturing frames from the webcam and processing them for color detection. The output window displays the real-time video feed with bounding boxes around detected colors. Press 'q' to exit the application.

Troubleshooting
    If there are issues with color detection or unexpected behavior, you may need to adjust the color ranges for each color based on environmental conditions and lighting.

Feel free to modify the script to add more colors or customize the color detection logic according to your specific requirements.
