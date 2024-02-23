# Vehicle Detection using a Custom Vision Model

This project demonstrates the implementation of vehicle detection and tracking using a Custom Vision model trained on Azure. The project utilizes computer vision techniques to analyze a video stream, identify different types of vehicles, and track their movements.

## Overview

The project involves several key steps:

1. **Creating a Custom Vision Resource**: Setting up a Custom Vision resource in Azure for training and deploying machine learning models for image classification, object detection, etc.

2. **Creating and Training the Project**: Establishing a project in the Custom Vision portal, uploading training images of bicycles, cars, and trams, applying corresponding labels, and initiating the training process.

3. **Publishing the Iteration**: Publishing the trained iteration of the model to make it available for use in various applications, ensuring its accuracy through monitoring and updates.

4. **Getting the Prediction URL**: Retrieving the endpoint URL and prediction key from the Custom Vision portal to make predictions using the trained model through an API endpoint.

5. **Importing Libraries**: Utilizing Python libraries such as requests, NumPy, and cv2 for making HTTP requests, handling multi-dimensional arrays, and image processing, respectively.

6. **Setting Custom Vision Endpoint URL and Prediction Key**: Initializing variables in Python to authenticate requests and specify the Custom Vision endpoint for detection.

7. **Defining Prediction Function**: Defining a Python function to send image data to the Custom Vision endpoint for prediction, parsing the JSON response to extract prediction results.

8. **Loading Video and Defining Output Path**: Loading a video file, setting up an output video writer, and defining parameters such as codec, frame rate, and dimensions for the output video.

9. **Vehicle Detection**: Implementing vehicle detection by processing each frame of the video, sending it for object detection using the Custom Vision model, drawing bounding boxes around detected vehicles, and displaying labels and confidence scores.

10. **Releasing Resources**: Releasing resources used for object detection, such as video stream and output video file, to prevent memory leaks and optimize resource utilization.

## Video Output

[Click here to view the output video](https://drive.google.com/file/d/1IocJfV5mJ5lROOj3ZVclb7cBAw_wPzhR/view?usp=sharing)

The output video showcases the results of vehicle detection and tracking performed by the Custom Vision model on a one-minute video containing various vehicles such as bicycles, trams, and cars.

## Dependencies

- Python 3.x
- Azure Custom Vision Service
- OpenCV
- NumPy

## Usage

To replicate the vehicle detection and tracking process:

1. Clone this repository.
2. Set up a Custom Vision resource on Azure and train your model.
3. Update the Python script with your endpoint URL and prediction key.
4. Install the required dependencies.
5. Run the Python script, providing the input video file path.
6. View the output video to observe the vehicle detection and tracking results.

