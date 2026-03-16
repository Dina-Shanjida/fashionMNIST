# Fashion MNIST Classification with PyTorch

A learning project to classify **Fashion MNIST** images using PyTorch. Uses a small subset of **6,000 images** in CSV format. This project helped me understand **data preprocessing, neural networks, training loops, and model evaluation** in PyTorch.

---

## Key Learnings

- How to **load and preprocess CSV image data**  
- Visualizing images with **Matplotlib**  
- Creating a **custom PyTorch Dataset and DataLoader**  
- Building a **feedforward neural network** from scratch  
- Implementing **training and evaluation loops**  
- Understanding **loss, accuracy, and overfitting**  

---

## Features

- **Data:** 28x28 grayscale images, 10 classes (T-shirt, Trouser, Pullover, Dress, Coat, Sandal, Shirt, Sneaker, Bag, Ankle Boot)  
- **Preprocessing:** Flattened, normalized to [0,1], train/test split (80/20)  
- **Visualization:** Sample 5x5 image grid with labels  
- **Custom Dataset:** PyTorch `Dataset` & `DataLoader` for batching  

---

## Model

- **Architecture:** Feedforward NN  
  - Input: 784  
  - Hidden: 128 → 64 (ReLU)  
  - Output: 10  
- **Loss:** CrossEntropy  
- **Optimizer:** SGD (lr=0.01, momentum=0.9)  
- **Training:** 50 epochs, batch size 32  

---

## Results

- Training Accuracy ~91%  
- Testing Accuracy ~88%  
- Observations: Model performs well on small dataset but has **room for improvement** with more data or better architecture  

---

## Improvements & Next Steps

- Implement **Convolutional Neural Networks (CNNs)** for better feature extraction  
- Use **Data Augmentation** (rotation, flipping) to increase dataset diversity  
- Explore **hyperparameter tuning** and **regularization** to reduce overfitting  
- Train on **full Fashion MNIST dataset** (60,000 images) for higher accuracy  
- Visualize **misclassified images** to understand model limitations  

---

## Dependencies

```bash
pip install torch pandas scikit-learn matplotlib
