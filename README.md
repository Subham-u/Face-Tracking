# Real-Time Face Tracking System

## 1. Introduction
The objective of this assignment is to create a real-time face tracking system that detects and tracks faces within a video stream. This document outlines the research, implementation steps, testing procedures, and final deliverables.

## 2. Research and Exploration

### Libraries and Models
**Identified Libraries:**
- **YOLO (You Only Look Once):** Fast and accurate object detection.
- **Mediapipe:** Provides high-fidelity solutions for face and hand tracking, developed by Google.
- **OpenCV:** Widely used for computer vision tasks.
- **GANs (Generative Adversarial Networks):** Advanced models for generating realistic images.

**Evaluation Metrics:**
- **Accuracy:** The precision of face detection.
- **Speed:** The latency of the system.
- **Ease of Integration:** Simplicity in incorporating the library into the system.

After evaluating the libraries, Mediapipe was chosen for its balance of accuracy, speed, and ease of integration.

## 3. Basic Face Tracking Implementation
**Single Face Detection and Tracking**
- Implemented a basic face detection algorithm using Mediapipe.
- [GitHub Repo](https://github.com/Subham-u/Face-Tracking/blob/main/Basic.py)

## 4. Intermediate Face Tracking
**Prototype Development**
- Developed a prototype application demonstrating real-time face detection and tracking with visual feedback (bounding boxes).
- [GitHub Repo](https://github.com/Subham-u/Face-Tracking/blob/main/Intermediate.py)

## 5. Advanced Face Tracking
**Multi-face Detection and Tracking**
- Modified the algorithm to handle multiple faces using Mediapipe, which supports multiple face detection out of the box.
- [GitHub Repo](https://github.com/Subham-u/Face-Tracking/blob/main/Advanced.py)

## 6. Testing and Benchmarks

### Testing
The system was tested on a laptop with the following specifications:
- **CPU:** Apple M2 chip
- **RAM:** 8GB
- **Camera:** Built-in webcam

### Benchmarks
**Performance Metrics:**
- **Detection Speed:** Approximately 15-20 frames per second (FPS).
- **Accuracy:** High accuracy in various lighting conditions.
- **Latency:** Minimal latency observed during real-time tracking.

## 7. Challenges and Solutions

### Challenges
- **Real-time Performance:** Ensuring the system runs in real-time without significant lag.
- **Multiple Face Tracking:** Handling multiple faces simultaneously and ensuring each face is tracked accurately.

### Solutions
- **Optimization:** Used efficient algorithms provided by Mediapipe for real-time performance.
- **Robustness:** Enhanced the robustness of face detection by fine-tuning detection confidence thresholds.

## 8. Conclusion
The real-time face tracking system was successfully developed using Mediapipe. It accurately detects and tracks multiple faces with minimal latency. The project demonstrates a robust application of face detection and tracking suitable for various real-world applications.

## 9. Setup and Usage Instructions

### Prerequisites
- Python 3.9 or higher
- OpenCV
- Mediapipe
- Terminal

```bash
pip install opencv-python mediapipe
```

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Subham-u/Face-Tracking.git
    ```
2. Navigate to the project directory:
    ```bash
    cd Face-Tracking
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

### Running the Application
Save the provided code into a Python script and run it:

```bash
python Basic.py  # or python3 Basic.py
python Intermediate.py  # or python3 Intermediate.py
python Advanced.py  # or python3 Advanced.py
```

### Usage
- **Start the Application:** The system will start the webcam and begin detecting faces.
- **Stop the Application:** Press `q` to quit the application.

## 10. Final Deliverables

**Submitted Materials:**
- **Code:** https://github.com/Subham-u/Face-Tracking
- **Documentation:** This detailed report.
- **Demonstration Video:** https://youtu.be/pGjFFZQKUaA
