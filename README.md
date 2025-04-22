# 🥦 Vegetable Classification using CNN
This project leverages Convolutional Neural Networks (CNN) for image classification to classify 15 different vegetable types.
The model is trained from scratch on a carefully curated dataset to automate the process of vegetable identification.
Ideal for smart agriculture, food processing, or any use case that requires the classification of vegetable images into distinct categories.

📁 **Dataset**
The dataset used in this project contains labeled images of 15 vegetable types, each with multiple images under varying conditions (light, angle, size). The vegetable classes include:

Beans
Bitter Gourd
Bottle Gourd
Brinjal
Broccoli
Cabbage
Capsicum
Carrot
Cauliflower
Cucumber
Papaya
Potato
Pumpkin
Radish
Tomato

**Data Size**: Over **2000 images** split into training, validation, and test sets.

## 🔧 **Preprocessing Steps**

Before training the model, several preprocessing steps were implemented to improve the quality of the data and prepare it for efficient training:

**Resizing:**

All images were resized to a consistent shape (e.g., 224x224 pixels) to maintain uniformity for model input.

**Data Augmentation:**

We applied augmentation techniques to artificially expand the dataset by:

Random Rotation

Flipping Horizontally

Zooming

Width and Height Shifts This step increases the model's ability to generalize on unseen data, simulating real-world variations in vegetable images.

**Normalization:**

Image pixel values were scaled to a range of 0 to 1 by dividing by 255 to normalize input features.

**Splitting the Data:**

The dataset was split into **70% Training, 15% Validation, and 15% Testing** sets to ensure proper model evaluation.

🧠 **Model Architecture**
The model is a Convolutional Neural Network (CNN), specifically designed to learn spatial hierarchies and perform multi-class classification.

# Layers:
**Input Layer:** 224x224x3 (RGB Images)

**Convolutional Layers:** 32, 64, 128 filters with ReLU activation to learn spatial features.

**MaxPooling Layers** to reduce spatial dimensions.

**Dropout Layers** to prevent overfitting.

**Fully Connected Layers** with ReLU activation to merge features learned by convolutional layers.

**Final Output Layer:** Softmax with 15 nodes (representing the 15 vegetable classes).

**Activation Function:** ReLU for hidden layers and Softmax for output layer.

**Loss Function:** Categorical Cross-Entropy (for multi-class classification).

**Optimizer:** Adam optimizer, chosen for its efficiency and fast convergence.




# 📊  **Model Performance**

Training Accuracy: 98%

Validation Accuracy: 95%

Test Accuracy: 94.7%

Loss Curve: Smooth convergence with minimal overfitting.



