# Face Mask Classification Using Hugging Face Pretrained Model
This project demonstrates a face mask classification system using a pretrained model from Hugging Face's Transformers library. It employs Gradio for the user interface, allowing users to upload images and receive predictions on whether the subject is wearing a mask or not.

![image](https://github.com/user-attachments/assets/0a67db1a-4f12-4510-a7ed-43467769feaf)

# Project Overview
The goal of this project is to classify images of faces as either "wearing a mask" or "not wearing a mask" using a pretrained image classification model. The model is fine-tuned for the specific task of detecting face masks. 
This project uses:
Hugging Face Transformers: For loading a pretrained image classification model.
Gradio: To create an interactive, user-friendly interface.
Pillow: For basic image processing.

# Setup and Dependencies:
To run the project, you need the following dependencies:
pip install gradio transformers Pillow

Key Libraries:
Transformers: Provides easy access to a wide variety of state-of-the-art machine learning models.
Gradio: Enables building an easy-to-use web interface where users can upload images and see the classification result in real time.
Pillow: Used for image handling and processing.

# Model Overview
The face mask classification model is based on a pretrained ConvNeXt model from Hugging Face. This model is chosen due to its strong performance in image classification tasks. The model is fine-tuned specifically to differentiate between faces with and without masks.

Steps Involved:
Load Pretrained Model: The ConvNeXt model is loaded via Hugging Face's transformers library.
Image Preprocessing: Uploaded images are converted to a format suitable for model inference (NumPy arrays).
Prediction: The model returns a prediction of either "mask" or "no mask" based on the input image.
Gradio Interface
The interface is built using Gradio, providing a simple and interactive user interface for uploading images and visualizing predictions.

Key Features:
Input: Users can upload images through the web interface.
Output: The model predicts whether the person in the image is wearing a face mask or not.
Real-time Feedback: Immediate results are provided to the user.

# Future Improvements
Model Fine-Tuning: Fine-tune the model further for higher accuracy and robustness across various image qualities.
Dataset Expansion: Incorporate a larger dataset with more diverse facial images to improve model generalization.
Deploy on Hugging Face Spaces: Host the app on Hugging Face Spaces for easier access and permanent deployment.
