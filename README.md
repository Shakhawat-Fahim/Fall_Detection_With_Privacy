# Fall Detection with Privacy-Preserving Facial Expression Recognition
This project detects human falls in real-time using body pose estimation, while also ensuring privacy protection by blurring faces. At the same time, it recognizes facial expressions before blurring, giving useful privacy protected insights.

## Features
Fall Detection – Uses pose landmarks (shoulders, hips) to detect unusual postures indicating a fall.

Face Blurring – Protects personal identity by blurring faces in the video stream.

Emotion Recognition – Detects dominant emotions (happy, sad, angry, surprise) using DeepFace.

Real-Time Processing – Works with both webcam and video files.

Output Video – Saves the annotated video.

## Tech_Stack
MediaPipe – Pose and face detection.

OpenCV – Video frame handling and visualization.

DeepFace – Pre-trained facial emotion recognition.

Python 3.9+ 

## Working
Pose Estimation – Detects body landmarks like shoulders and hips.

Angle Analysis – Calculates the torso angle. If it’s too horizontal (<50° or >130°), a fall is detected.

Face Detection & Blurring – Detects faces and applies dynamic Gaussian blur.

Emotion Recognition – Runs DeepFace on the face ROI before blurring to detect expressions.

Alerts & Output – Displays “FALL DETECTED” in real-time and saves an annotated video.

## Test
Input: A video of a person walking and falling/Webcam live feed of falling.

Output: The video with annotation: * “FALL DETECTED!” overlay * Blurred faces * Emotion labels like “happy” or “surprise”

## Future Improvements
Use robust tracking to reduce false positives.

Robust privacy.

Support multi-person detection.

Test on IR/mmWave sensors for low-light conditions.
