CNN Traffic Sign Classifier (U-Turn vs. Stop Sign)
📝 Project Overview
This project is a Convolutional Neural Network (CNN) classifier built to distinguish between two specific traffic signs: U-Turn and Stop Sign. This model serves as an introduction to computer vision, demonstrating the full machine learning pipeline—from data generation and preprocessing to building a deep learning model from scratch.

🧠 Technical Approach
The model utilizes a custom Convolutional Neural Network (CNN) architecture to extract spatial features from images and perform binary classification.

Input Pipeline: Images are resized to 128x128 pixels and normalized to [0, 1] range.

Data Augmentation: To improve model generalization, the model includes:

RandomFlip (Horizontal)

RandomRotation (0.1)

RandomZoom (0.1)

Architecture: The model uses 3 blocks of Conv2D and MaxPooling2D layers, interleaved with Dropout (0.25) to prevent overfitting, ending with a Flatten layer and Dense classification layers.

🛠 Tech Stack
Language: Python

Deep Learning Framework: TensorFlow / Keras

Libraries: NumPy, Matplotlib, OS

📈 Model Performance
Final Training Accuracy: 75%

Final Validation Accuracy: 50%

Loss Function: Binary Crossentropy

Optimizer: Adam

💡 Lessons Learned
Data Handling: Implemented a dummy data generation strategy to test pipeline integrity before loading real images.

Overfitting Analysis: The model currently shows a performance gap between training (75%) and validation (50%). This indicates overfitting, where the model memorizes the training data. Future iterations will focus on increasing dataset size, applying stronger regularization, and optimizing hyperparameters.
