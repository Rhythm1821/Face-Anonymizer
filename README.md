# Face Anonymizer
The "Face Anonymizer" is a Python-based project that blurs human faces in images and webcam video streams. It utilizes OpenCV and MediaPipe for face detection and processing.

## Installation
To use the "Face Anonymizer" project, follow these steps:

**Clone the GitHub repository:**

git clone https://github.com/Rhythm1821/Face-Anonymizer.git

cd Face-Anonymizer

**Install the required dependencies from the requirements.txt file:**

pip install -r requirements.txt

## Usage

The "Face Anonymizer" can be used in three different modes: image, video, and webcam.

### Image Mode:
To anonymize a single image, run the main.py script with the --mode image argument and specify the path to the image file using the --filePath argument:

python main.py --mode image --filePath path/to/your/image.png
The anonymized image will be saved in the output folder.

### Video Mode:
To anonymize a video, run the main.py script with the --mode video argument and specify the path to the video file using the --filePath argument:

python main.py --mode video --filePath path/to/your/video.mp4
The anonymized video will be saved in the output folder as output.mp4.

### Webcam Mode:
To anonymize faces in real-time using your webcam, run the main.py script with the --mode webcam argument:

python main.py --mode webcam
Press 'q' to stop the webcam feed.

## Note
The project uses face detection to identify faces in images or video frames. Detected faces are then anonymized by blurring them. The blurring is done by applying a Gaussian blur to the face region.

## Requirements
The project requires the following Python packages, which can be installed using the provided requirements.txt file:

opencv-python==4.6.0.66
mediapipe==0.9.0
Make sure to install the required packages before running the script.