# signlanguagedetector
A sign language detector which detects basic signs created using OpenCV and Tensorflow Object Detection API. 

The trained model present in the repo can detect basic signs of Hello, Yes, No, Thank you and I Love You. You can customise your model to detect various types of objects as per your requirement. 

## Step 1: Data Collection

1. Run `captures.ipynb` to capture images from your camera using OpenCV. This will collect data for training your object detection model.

## Step 2: Labeling Images

1. Clone the labelImg repository using the following command inside the `Tensorflow` folder:
   ```bash
   git clone https://github.com/HumanSignal/labelImg.git
   ```

2. Navigate to the cloned `labelImg` directory.

3. Use labelImg to manually label each image captured in the previous step.

## Step 3: Data Preparation

1. Create two folders named `test` and `train` to divide your dataset for training and testing purposes.

2. Sort both the images and label files into their respective folders (`test` and `train`).

## Step 4: Setting Up TensorFlow Object Detection

1. Open `Tutorial.ipynb` and run each section to set up paths, create label maps, generate TF records, and clone TensorFlow Object Detection API files.

2. Copy the `pipeline.config` file to the training folder and update the configuration file as required for transfer learning.

## Step 5: Model Training

1. Train the model using SSD Mobilenet or your preferred architecture.

## Step 6: Real-Time Detections

1. Load the trained model and perform real-time detections using the provided scripts.

2. Store the detections for later use if necessary.



- Make sure you have all the necessary dependencies installed.
