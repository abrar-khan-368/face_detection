# Face Detection Notebook

This Jupyter Notebook demonstrates how to perform face detection using OpenCV and a deep learning model. The notebook covers the following steps:

## Steps Included

1. **Environment Setup**:
   - Import necessary libraries including OpenCV and NumPy.

2. **Loading the Pre-trained Model**:
   - Load the Caffe model configuration (`deploy.prototxt.txt`) and weights (`res10_300x300_ssd_iter_140000.caffemodel`) for face detection.
   - Initialize the face detector using OpenCV's `cv2.dnn.readNetFromCaffe`.

3. **Loading and Displaying the Test Image**:
   - Load a test image for face detection using OpenCV.
   - Display the image to visualize the input data.

4. **Preprocessing for Face Detection**:
   - Convert the input image into a blob to match the input requirements of the neural network.
   - Normalize the input by performing mean subtraction and resizing the image.

5. **Performing Face Detection**:
   - Pass the preprocessed image through the network to detect faces.
   - Filter out predictions based on a confidence threshold to ignore weak detections.
   - Draw bounding boxes around detected faces and label them with the confidence score.

6. **Displaying Results**:
   - Display the output image with bounding boxes and confidence labels for detected faces.

