# 🌊 Marine Debris Detection Project
A Convolutional Neural Network (CNN) model to detect and classify marine debris from images, contributing to sustainability and environmental conservation.

# 🧩 Problem Statement
Marine pollution has become one of the biggest threats to ocean life. Large amounts of plastic, metal, and other waste float on the ocean surface or settle underwater. Detecting and classifying this debris can assist in cleanup and recycling efforts, helping protect marine ecosystems.

# 🎯 Project Goal
To develop a Convolutional Neural Network (CNN) model that can detect and classify marine debris from images — contributing to sustainability and environmental conservation.

# 🌱 Why It Supports Sustainability
This project aligns with our Sustainable Development Goals. By identifying waste in marine environments, it helps:

Track pollution sources

Assist in cleanup operations

Promote recycling and awareness
 

---

## 🎯 Project Overview

The model is a **binary classifier** that was trained on the 
[Marine Debris Images Dataset]:(https://www.kaggle.com/datasets/zienabesam/marine-debris-images-dataset) from Kaggle. 
It learns to distinguish between photos containing various forms of beach/ocean waste and photos of the natural environment (sand, water, etc.).

### Technologies Used
* **Python**
* **TensorFlow** & **Keras**
* **Matplotlib** (for plotting training history)

---

## 🤖 Model Architecture

This project uses a custom sequential CNN model. The architecture consists of:
* `Conv2D` layers (using 'relu' activation) to find image features.
* `MaxPooling2D` layers to downsample and focus on the most important features.
* A `Flatten` layer to prepare the data for the classifier.
* `Dense` layers (the "brain" of the model).
* A final `Dense` layer with **1 neuron** and a **'sigmoid'** activation function, which outputs a probability (0 for 'Non_Debris', 1 for 'Debris').

---

## 📈 Training & Results

The model was trained for **20 epochs**, showing a healthy learning trend. The validation loss and accuracy closely followed the training loss and accuracy, indicating that the model **generalized well** and did not significantly overfit.

The final model accuracy is yet to be calculated.

### Training Performance

| Loss Plot | Accuracy Plot |
| :---: | :---: |
| <img width="547" height="461" alt="image" src="https://github.com/user-attachments/assets/0157fb92-d7f8-4bd1-85d6-efea5d19bb4e" />
| <img width="547" height="461" alt="image" src="https://github.com/user-attachments/assets/43e63d79-d6bd-43b9-8294-88c72597dd4f" />
 |

---

## 💡 Future Improvements
* **Move to Object Detection:** Upgrade the project to an object detection model (like YOLOv8) to find *multiple* objects and their locations in a single image.
* **Add More Classes:** Train on a more complex dataset to identify specific types of debris (e.g., `plastic_bottle`, `fishing_net`, `styrofoam`).

---
