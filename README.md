# Fake Logo Detection using CNN

This is a final year project that uses a **Convolutional Neural Network (CNN)** to automatically identify and classify brand logos as either **Original** or **Fake**. The system includes a graphical user interface (GUI) for easy interaction and performance visualization.

## 📂 Project Structure
The repository is organized as follows to ensure the script runs correctly:

* **`Dataset/`**: Contains the raw logo images.
    * `original/`: Subfolder for authentic logo samples.
    * `fake/`: Subfolder for counterfeit logo samples.
* **`model/`**: Contains pre-trained data to skip training time.
    * `model_weights.hdf5`: Saved weights of the trained CNN.
    * `history.pckl`: Training history for generating accuracy/loss graphs.
    * `X.txt.npy` & `Y.txt.npy`: Preprocessed image and label arrays.
* **`FakeLogoDetection.py`**: The main Python application.
* **`run.bat`**: A Windows batch file to launch the program instantly.
* **`Fake Logo Detection.docx`**: Full project documentation and screenshots.

## 🚀 Features
* **Dataset Management**: Upload and automatically label images from the `Dataset/` folder.
* **Advanced Preprocessing**: Resizes images to 64x64 pixels, normalizes pixel values, and shuffles data for better training.
* **High Accuracy**: The model achieves approximately **94% accuracy** in detecting fake logos.
* **Visual Analytics**: Generates a **Confusion Matrix** to see prediction counts and a **Training Graph** to track accuracy and loss over 20 epochs.
* **Real-time Classification**: Allows users to upload a single test image to see the "Fake" or "Original" prediction displayed on screen.

## 🛠️ How to Run
1. **Prerequisites**: Install the required Python libraries:
   ```bash
   pip install tensorflow keras opencv-python scikit-learn matplotlib seaborn numpy

2. Launch:

--> Simply double-click run.bat on Windows.

--> Alternatively, run python FakeLogoDetection.py in your terminal.

📊 Results
Training/Testing Split: 80% of data used for training (248 images) and 20% for testing (62 images).

Metrics: Provides Precision, Recall, and F1-Score to validate model performance.
