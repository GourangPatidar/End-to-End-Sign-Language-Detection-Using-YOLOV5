

# End-to-End Sign Language Detection Using YOLOv5

## Introduction
Welcome to the YOLOv5 HAND SIGN project documentation! This project focuses on detecting and recognizing six different hand gestures using the YOLOv5 deep learning model. The hand gestures include "hello," "yes," "I love you," "please," "thanks," and "no." The main goal is to create a tool that facilitates communication for individuals with hearing impairments by translating hand gestures into understandable signals using computer vision techniques.

## Project Overview
The YOLOv5 HAND SIGN project leverages the YOLO (You Only Look Once) object detection architecture, specifically YOLOv5, to detect and classify hand gestures in images or videos. YOLOv5 is a state-of-the-art object detection model known for its accuracy and speed. This project also incorporates TensorFlow and Keras for building and training the deep learning models. By utilizing advanced neural networks such as Convolutional Neural Networks (CNNs), the project aims to provide real-time and accurate detection of hand gestures.

## Hand Gestures
The project can recognize the following hand gestures:

1. **Hello**: A waving hand gesture used to greet someone.
2. **I Love You**: A gesture representing "I love you" in sign language, typically with the pinky, index finger, and thumb extended.
3. **No**: A hand gesture indicating negation or disagreement, often involving a shaking motion.
4. **Please**: A gesture used to make a polite request.
5. **Thank You**: A gesture used to express gratitude.
6. **Yes**: A hand gesture representing acknowledgment, affirmation, consent, agreement, or approval.

## Project Details
- **Duration**: January 2024 - February 2024
- **Developed By**: Gourang Patidar
- **GitHub Repository**: [End-to-End-Sign-Language-Detection-Using-YOLOv5](https://github.com/GourangPatidar/End-to-End-Sign-Language-Detection-Using-YOLOV5)

## Description
1. **Development**: Created a robust sign language detection system using YOLOv5 architecture, TensorFlow, and Keras. This system aims to facilitate effective communication for the hearing-impaired community.
2. **Techniques**: Utilized Artificial Neural Networks (ANN), Convolutional Neural Networks (CNN), and various mathematical concepts for feature extraction, classification, and model optimization. These techniques are crucial for addressing the challenge of accurately recognizing hand signs used by individuals with speech impairments.

## Skills Utilized
- **Convolutional Neural Networks (CNN)**: Employed for deep learning and image classification tasks, enabling the model to learn and recognize intricate patterns in hand gestures.
- **Computer Vision**: Applied to detect and recognize hand gestures in both images and videos, enhancing the system's capability to operate in real-time scenarios.
- **TensorFlow and Keras**: Used for building, training, and deploying the deep learning models, providing a flexible and powerful framework for development.
- **YOLOv5**: A specialized object detection model known for its efficiency and accuracy, crucial for the fast and reliable detection of hand gestures.

## Installation and Setup
To get started with the project, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/GourangPatidar/End-to-End-Sign-Language-Detection-Using-YOLOV5.git
    ```
2. **Navigate to the project directory**:
    ```bash
    cd End-to-End-Sign-Language-Detection-Using-YOLOV5
    ```
3. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

## Project Structure
- **.github/workflows/**: Contains CI/CD workflows for the project, automating tasks such as testing and deployment.
- **data/**: Contains datasets used for training and testing the models. This directory includes images of hand gestures along with their annotations.
- **docs/**: Contains documentation related to the project, including user guides and technical documentation.
- **flowcharts/**: Contains flowcharts illustrating the project workflow, providing a visual representation of the process.
- **signLanguage/**: Contains scripts and notebooks related to sign language processing, including data preprocessing and augmentation scripts.
- **templates/**: Contains HTML templates for the web application, used for rendering the user interface.
- **yolov5/**: Contains the YOLOv5 model and related scripts, including training, validation, and inference scripts.
- **Dockerfile**: A script for containerizing the application, allowing for consistent and reproducible deployments.
- **app.py**: The main application script, serving as the entry point for the web application.
- **requirements.txt**: A list of dependencies required for the project, specifying the necessary Python packages.
- **setup.py**: A setup script for installing the package, enabling easy distribution and installation.
- **template.py**: A template script for various utilities, providing reusable functions and classes.

## Usage
To run the application and start detecting hand gestures:

1. **Run the application**:
    ```bash
    python app.py
    ```
2. **Follow the instructions in the application** to upload images or videos and detect hand gestures. The application will display the detected gestures along with their confidence scores.

## Training the Model
To train the YOLOv5 model on the hand gesture dataset:

1. **Prepare the dataset**: Ensure the dataset is in the correct format, with images and corresponding annotation files. Split the dataset into training and testing sets.
2. **Configure the YOLOv5 model**: Modify the configuration files in the `yolov5` directory to match the dataset specifications, including the number of classes and paths to the data.
3. **Train the model**:
    ```bash
    python yolov5/train.py --img 640 --batch 16 --epochs 50 --data data/hand_gestures.yaml --cfg yolov5/models/yolov5s.yaml --weights yolov5s.pt
    ```
    This command trains the model with images of size 640x640, a batch size of 16, for 50 epochs.

## Evaluation
To evaluate the trained model:

1. **Run the evaluation script**:
    ```bash
    python yolov5/val.py --data data/hand_gestures.yaml --weights runs/train/exp/weights/best.pt --img 640
    ```
    This script evaluates the model's performance on the test set, providing metrics such as precision, recall, and mAP (mean Average Precision).

## Deployment
To deploy the application using Docker:

1. **Build the Docker image**:
    ```bash
    docker build -t sign-language-detection .
    ```
2. **Run the Docker container**:
    ```bash
    docker run -p 5000:5000 sign-language-detection
    ```
    This command starts the application in a Docker container, making it accessible at `http://localhost:5000`.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements
Special thanks to the developers and contributors of the YOLOv5, TensorFlow, and Keras libraries. Their work provided the foundation for this project.

## Contact
For any queries or issues, please contact Gourang Patidar at gourangpatidar2003@gmail.com

---

