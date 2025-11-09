# 🌊 Marine Debris Classification (CNN)

This project is a Convolutional Neural Network (CNN) model built with TensorFlow and Keras to classify images as containing **Debris** or **Non_Debris**. The goal is to create a simple, effective tool for automatically identifying marine pollution from images.

 

---

## 🎯 Project Overview

The model is a **binary classifier** that was trained on the [Marine Debris Images Dataset](https://www.kaggle.com/datasets/zienabesam/marine-debris-images-dataset) from Kaggle. It learns to distinguish between photos containing various forms of beach/ocean waste and photos of the natural environment (sand, water, etc.).

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

The final model achieved a validation accuracy of approximately **[Enter your best val_accuracy here, e.g., 94%]**.

### Training Performance
*(I strongly recommend you save your graphs from the notebook and add them to your repository!)*

| Loss Plot | Accuracy Plot |
| :---: | :---: |
| ![Loss vs Val_Loss](path/to/your/loss_graph.png) | ![Accuracy vs Val_Accuracy](path/to/your/accuracy_graph.png) |

---

## 💡 Future Improvements
* **Move to Object Detection:** Upgrade the project to an object detection model (like YOLOv8) to find *multiple* objects and their locations in a single image.
* **Add More Classes:** Train on a more complex dataset to identify specific types of debris (e.g., `plastic_bottle`, `fishing_net`, `styrofoam`).

---
