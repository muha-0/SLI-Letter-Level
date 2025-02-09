# Sign Language Translation (SLT) - Letter Level

## About the Project
This project is a **real-time Sign Language Translator (SLT)** at the **letter level**, designed to recognize hand gestures corresponding to the **English alphabet (A-Z)**. It utilizes **MediaPipe** for hand landmark extraction and employs deep learning models to classify gestures.

### Features:
- **Real-time letter recognition** using a webcam
- **Hand landmark extraction** via **MediaPipe**
- **Deep learning models**:
  - **Convolutional Neural Network (CNN)** for feature extraction
  - **Dense Neural Network (DNN)** for classification
- **Softmax output layer** to classify 26 letters
- **Optimized without LSTMs**, as they did not improve performance

## Technologies Used
- **Python**
- **OpenCV** (for real-time video processing)
- **MediaPipe** (for hand tracking)
- **TensorFlow / Keras** (for deep learning models)
- **NumPy, Pandas** (for data handling)

## How It Works
1. **Hand landmark extraction:**
   - The system captures a frame from the webcam.
   - It processes the frame using **MediaPipe Hands**, extracting **21 key points** (each with x, y coordinates).
   - These 42 values are used as input features for the neural network.

2. **Model Prediction:**
   - The extracted features are fed into a **CNN or DNN model**.
   - The model predicts the letter based on hand position.
   - The letter is displayed in real-time.

## Team Members
- **Alice Johnson**
- **Bob Smith**
- **Charlie Davis**
- **David Lee**

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/YOUR_USERNAME/SLT_project_MP_images.git
   cd SLT_project_MP_images
   ```
2. Install dependencies:
   ```sh
   pip install torch torchvision transformers groundingdino opencv-python requests pandas numpy pillow mediapipe tensorflow keras
   ```
3. Run the real-time prediction:
   ```sh
   python run_slt.py
   ```

## Usage
- Make sure your webcam is enabled.
- Perform a hand gesture corresponding to an English letter.
- The system will recognize and display the predicted letter.

## Future Improvements
- Implement **word-level recognition** using LSTMs or transformers.
- Enhance accuracy with **more training data**.
- Support for **multiple sign languages**.

---
**License:** MIT


