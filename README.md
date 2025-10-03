# Sign Language Interpreter (SLI) - Letter Level

## About the Project
This project is a **real-time Sign Language Translator/Interpreter (SLI)** at the **letter level**, designed to recognize hand gestures corresponding to the **English alphabet (A-Z)**. It utilizes **MediaPipe** for hand landmark extraction and employs deep learning models to classify gestures.

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
- **Nour Hany**
- **Laila Khaled**
- **Yasmine Mohammed**
- **Ahmed Sameh**

## Usage
- Run SLT.py, you can run starting from the step of loading the model.
- Make sure your webcam is enabled.
- Perform a hand gesture corresponding to an English letter.
- The system will recognize and display the predicted letter.

## Future Improvements
- Implement **word-level recognition** using LSTMs or transformers.
- Enhance accuracy with **more training data**.
- Support for **multiple sign languages**.



