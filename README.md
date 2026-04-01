# Fashion Item Classifier

An application that classifies fashion items from images using a Convolutional Neural Network (CNN) trained on the Fashion MNIST dataset. The model is deployed as an interactive web application using Streamlit and containerized with Docker for easy deployment.

## Features

- **Image Classification**: Upload fashion item images to get real-time predictions
- **Pre-trained Model**: CNN model trained on Fashion MNIST dataset with 10 clothing categories
- **Web Interface**: User-friendly Streamlit application for easy interaction
- **Docker Support**: Containerized deployment for consistent environments
- **Grayscale Processing**: Handles color and grayscale images by converting to grayscale


### Interacting with the Application

1. Open the web application in your browser
2. Click "Browse files" to upload a fashion item image (JPG, JPEG, or PNG)
3. Click the "Classify" button to get the prediction
4. The app will display the uploaded image and the predicted clothing category

The model recognizes the following 10 fashion categories:
- T-shirt/top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle boot

## Model Details

### Model Type
- **Architecture**: Convolutional Neural Network (CNN)
- **Framework**: TensorFlow/Keras
- **Layers**: 3 Conv2D layers with MaxPooling, followed by Dense layers

### Dataset
- **Dataset**: Fashion MNIST
- **Size**: 60,000 training images, 10,000 test images
- **Image Format**: 28x28 grayscale images
- **Classes**: 10 fashion item categories

### Preprocessing Steps
1. **Normalization**: Pixel values scaled to [0, 1] range
2. **Reshaping**: Images reshaped to (28, 28, 1) for single-channel input
3. **Grayscale Conversion**: Color images converted to grayscale for consistency

### Training Configuration
- **Optimizer**: Adam
- **Loss Function**: Sparse Categorical Crossentropy
- **Metrics**: Accuracy
- **Epochs**: 10

### Evaluation Metrics
- **Test Accuracy**: 0.90
- **Validation**: Performed during training with test set

## Technologies Used

- **Python**: Core programming language
- **TensorFlow/Keras**: Deep learning framework for model development
- **Streamlit**: Web application framework
- **Pillow (PIL)**: Image processing library
- **NumPy**: Numerical computing
- **Matplotlib**: Data visualization (used in notebook)
- **Docker**: Containerization platform
- **Jupyter Notebook**: Development and experimentation environment
