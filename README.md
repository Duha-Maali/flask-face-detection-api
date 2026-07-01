# Flask Face Detection API

A Flask-based API for face detection using MTCNN and OpenCV.

The API accepts an uploaded image, detects faces, draws bounding boxes around them, saves the processed image, and returns it in the response.

## Features

* Accepts image uploads through an HTTP POST request

* Uses MTCNN (Multi-Task Cascaded Convolutional Neural Network) for face detection

* Draws bounding boxes around detected faces

* Returns the processed image with detected faces
  
* Saves processed images in the `processed` folder
  
* Returns a message when no faces are detected

## Requirements

* Python 3
* Dependencies listed in `requirements.txt`

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/Duha-Maali/flask-face-detection-api.git
   ```

2. Open the project folder:

   ```bash
   cd flask-face-detection-api
   ```

3. Install the required packages:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the application:

   ```bash
   python face_detection.py
   ```

5. Send a `POST` request to:

   ```text
   http://127.0.0.1:5000/detect_faces
   ```

Use `form-data` with the following field:

```text
Key: image
Type: File
```

The API returns the processed image with bounding boxes around detected faces.
