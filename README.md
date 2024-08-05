
---

# End-to-End Sign Language Detection Using YOLOv5

## Introduction
Welcome to the YOLOv5 HAND SIGN project documentation! This project focuses on detecting and recognizing six different hand gestures using the YOLOv5 deep learning model. The hand gestures include "hello," "yes," "I love you," "please," "thanks," and "no."

## Project Overview
The YOLOv5 HAND SIGN project utilizes the YOLO (You Only Look Once) object detection architecture, specifically YOLOv5, to detect and classify hand gestures in images or videos. YOLOv5 is a state-of-the-art object detection model known for its accuracy and speed.

## Hand Gestures
1. **Hello**: A waving hand gesture.
2. **I Love You**: A hand gesture representing "I love you" in sign language, with the pinky, index finger, and thumb extended.
3. **No**: A hand gesture for indicating negation or disagreement with a shaking motion.
4. **Please**: This sign indicates a polite request or asking for something politely.
5. **Thank You**: This sign indicates a polite expression of one's gratitude.
6. **Yes**: A hand gesture representing acknowledgment, affirmation, consent, agreement, or approval to answer when one is addressed.

## Project Details
- **Duration**: January 2024 - February 2024
- **Developed By**: Gourang Patidar
- **GitHub Repository**: [End-to-End-Sign-Language-Detection-Using-YOLOv5](https://github.com/GourangPatidar/End-to-End-Sign-Language-Detection-Using-YOLOV5)

## Description
1. Developed a robust sign language detection system using YOLOv5 architecture, TensorFlow, and Keras, enabling effective communication for the hearing-impaired community.
2. Utilized Artificial Neural Networks (ANN), Convolutional Neural Networks (CNN), and mathematical concepts for feature extraction, classification, and model optimization, addressing the challenge of recognizing hand signs used by individuals with speech impairments.

## Skills Utilized
- **Convolutional Neural Networks (CNN)**: For deep learning and image classification.
- **Computer Vision**: For detecting and recognizing hand gestures in images and videos.
- **TensorFlow and Keras**: For building and training the deep learning models.
- **YOLOv5**: For efficient and accurate object detection.

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
- **.github/workflows/**: Contains CI/CD workflows for the project.
- **data/**: Contains datasets used for training and testing the models.
- **docs/**: Contains documentation related to the project.
- **flowcharts/**: Contains flowcharts illustrating the project workflow.
- **signLanguage/**: Contains scripts and notebooks related to sign language processing.
- **templates/**: Contains HTML templates for the web application.
- **yolov5/**: Contains the YOLOv5 model and related scripts.
- **Dockerfile**: For containerizing the application.
- **app.py**: Main application script.
- **requirements.txt**: List of dependencies required for the project.
- **setup.py**: Setup script for installing the package.
- **template.py**: Template script for various utilities.

## Usage
1. **Run the application**:
    ```bash
    python app.py
    ```
2. **Follow the instructions in the application** to detect and recognize hand gestures from images or videos.

## Training the Model
To train the YOLOv5 model on the hand gesture dataset:

1. **Prepare the dataset**: Ensure the dataset is in the correct format and split into training and testing sets.
2. **Configure the YOLOv5 model**: Modify the configuration files in the `yolov5` directory to match the dataset specifications.
3. **Train the model**:
    ```bash
    python yolov5/train.py --img 640 --batch 16 --epochs 50 --data data/hand_gestures.yaml --cfg yolov5/models/yolov5s.yaml --weights yolov5s.pt
    ```

## Evaluation
To evaluate the trained model:

1. **Run the evaluation script**:
    ```bash
    python yolov5/val.py --data data/hand_gestures.yaml --weights runs/train/exp/weights/best.pt --img 640
    ```

## Deployment
To deploy the application:

1. **Build the Docker image**:
    ```bash
    docker build -t sign-language-detection .
    ```
2. **Run the Docker container**:
    ```bash
    docker run -p 5000:5000 sign-language-detection
    ```

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements
Special thanks to the developers and contributors of the YOLOv5, TensorFlow, and Keras libraries.

## Contact
For any queries or issues, please contact Gourang Patidar at [your-email@example.com].
```

---

