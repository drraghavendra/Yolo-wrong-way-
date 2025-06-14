wrong-way driving has emerged as a significant problem for road safety, thereby demanding robust detection systems. Specifically, this paper provides a solution to wrong-way driving detection by utilizing a deep learning model combining You Only Look Once (YOLOv9) to identify the vehicle and propose a Convolutional Neural Network (CNN) to categorize the behavior. The developed system uses the ability of YOLOv9 to detect objects on the road and then classifies the vehicles using a CNN classifier to determine the direction of travel. The training and validation dataset contains images of moving vehicles in the correct and incorrect directions, as marked by the annotators



YOLOv8 library for efficient vehicle detection. The core logic involves tracking vehicle centroids over frames to determine their movement direction. A configurable "detection line" and expected traffic flow direction are used to identify vehicles moving the "wrong way".

The code includes:

Environment Setup: Instructions and commands to install necessary libraries.
YOLO Model Loading: How to load a pre-trained YOLOv8 model.
Direction Detection Logic: Detailed functions for centroid calculation and determining vehicle direction (correct or wrong). This is the most important part, allowing you to define traffic flow.
Inference Function: A function to process video frames, apply YOLO detection, track objects, and annotate wrong-way detections.
Example Usage: A complete section demonstrating how to use the code with a sample video, including instructions on how to upload your own video.
In-depth Logic Explanation and Optimizations: A detailed Markdown section explaining the rationale behind the chosen methods, how to optimize performance, and crucial parameters you need to adjust based on your specific video content and traffic flow.
This immersive code block is self-contained and ready to be run in Google Colab. Remember to adjust the FLOW_TYPE and EXPECTED_DIRECTION variables in the "Example Usage" section based on the traffic flow in your specific video.
