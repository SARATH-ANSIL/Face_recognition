# Face Recognition Project

This project implements face detection and recognition using a pre-trained FaceNet model and OpenCV. The application captures images from the webcam, detects faces in the captured images, and recognizes them based on a pre-built database of known faces.

## Features
- **Face Detection:** Uses Haar Cascade to detect faces in images.
- **Face Recognition:** Recognizes faces using a pre-trained FaceNet model.
- **Webcam Capture:** Captures images directly from the webcam for face detection and recognition.
- **Database Storage:** Saves face signatures in a pickle file for future recognition.

## Prerequisites
- Python 3.x
- The following Python libraries must be installed:
  - `opencv-python`
  - `numpy`
  - `keras`
  - `tensorflow`
  - `Pillow`
  - `matplotlib`
  
You can install the required libraries using pip:
```bash
pip install opencv-python numpy keras tensorflow Pillow matplotlib
```
## Project Structure
```bash
.
├── fotoPeserta/        # Folder containing images of known participants
│   ├── participant1.jpg  # Example image for participant 1
│   ├── participant2.jpg  # Example image for participant 2
│   └── ...               # Additional images of known participants
├── facenet_keras.h5    # Pre-trained FaceNet model file
├── data.pkl             # Pickle file containing face signatures
├── Face_detection.ipynb  # Main Jupyter Notebook for face detection and recognition
└── README.md            # Project README file
```
## How It Works
Face Detection: The notebook uses Haar Cascade Classifier to detect faces in the input images.
Face Recognition: Detected faces are resized and pre-processed, then passed to the FaceNet model to generate face signatures. These signatures are stored in a database.
Webcam Capture: The notebook captures images from the user's webcam and processes them for face detection and recognition.
Output: Recognized faces are labeled with their corresponding identities.

## Running the Project
Clone this repository:
`git clone https://github.com/SARATH-ANSIL/Face_recognition.git`

Navigate to the project directory:
`cd Face-recognition`

Ensure you have the required images of known participants in the fotoPeserta/ folder.
Open the Jupyter Notebook:

`jupyter notebook Face_recognition.ipynb`

Run the cells in the notebook. Allow the application to access your webcam when prompted. Capture a photo, and the application will recognize any known faces.

## Example Output
When running the notebook, if any faces are detected and recognized, the script will draw bounding boxes around the faces and label them with the participant's name.

## Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page for new ideas.

## License
This project is licensed under the MIT License.

## Acknowledgments
OpenCV for computer vision functionalities.
Keras and TensorFlow for deep learning.
Haar Cascades for face detection.
