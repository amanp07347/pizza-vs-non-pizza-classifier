# pizza-vs-non-pizza-classifier# Pizza vs Not-Pizza Image Classifier

## Overview:
This project involves the creation of a feedforward neural network to perform image classification, distinguishing between "pizza" and "not pizza" images. The dataset consists of both pizza and non-pizza images, and the neural network is trained using binary cross-entropy loss. The model's performance is assessed on separate training and test datasets.

## Dependencies:
- Google Colab (for accessing Google Drive)
- Python
- NumPy
- PyTorch
- Matplotlib

## Code Structure:

1. **Import Libraries and Mount Google Drive:** The initial step involves importing the necessary libraries and establishing a connection to Google Drive for dataset access.

2. **Data Loader:** The `getdata` function is responsible for reading images from a specified path, with the assumption that each image has dimensions of 64x64x3.

3. **Data Paths:** The file paths for "pizza" and "not pizza" images are explicitly defined.

4. **Load and Visualize Data:** Images are loaded into tensor format, and a sample image is visualized using Matplotlib.

5. **Preprocess Data:** The dataset is divided into training and test sets. Images are reshaped and normalized, ensuring pixel values fall within the range of 0 to 1.

6. **Create Labels:** Supervised learning involves assigning labels to images; "pizza" images are labeled as 1, while "not pizza" images are assigned a label of 0.

7. **Model Architecture:** A straightforward neural network architecture is introduced, comprising two hidden layers employing ReLU activations. The output layer employs a sigmoid activation function to produce values ranging from 0 to 1.

8. **Train Model:** The model is trained utilizing binary cross-entropy loss. Gradient descent is applied to adjust the model's weights, and periodic updates of the training loss are displayed.

9. **Save Model:** Post-training, the model is saved to persistent storage.

10. **Test Model:** The model is tested using a sample test image, and the model's prediction for this image is displayed. Additionally, the overall accuracy of the model on both training and test datasets is presented.

## Final Notes:
This elementary neural network serves as an initial approach to image classification. Enhancing model performance may involve adopting more intricate architectures, employing data augmentation strategies, and conducting hyperparameter tuning to optimize classification accuracy.
