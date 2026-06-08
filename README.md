# Real vs AI-Generated Image Classification

A deep learning project that classifies images as either **real-world photographs** or **AI-generated images** using a Convolutional Neural Network (CNN). The project explores computer vision techniques for synthetic media detection and demonstrates the application of deep learning in identifying AI-generated content.

---

## Overview

With the rapid advancement of generative AI models, distinguishing authentic images from AI-generated content has become increasingly important. This project implements a CNN-based image classification system capable of learning visual patterns and features that differentiate real images from synthetic ones.

The model is trained on a labeled dataset containing both real and AI-generated images and evaluated on unseen data to measure its classification performance.

---

## Objectives

- Classify images as **Real** or **AI-Generated**
- Explore CNN architectures for image classification
- Apply image preprocessing and data augmentation techniques
- Evaluate model performance on unseen data
- Understand challenges in synthetic image detection

---

## Dataset

The dataset consists of two classes:

- **Real Images**
- **AI-Generated Images**

### Dataset Split

| Dataset | Images |
|----------|---------|
| Training Set | 479 |
| Testing Set | 499 |
| Total | 978 |

Images were organized into class-specific directories and processed using TensorFlow data pipelines.

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- OpenCV

---

## Data Preprocessing

The following preprocessing steps were applied:

- Image resizing
- Pixel normalization
- Batch generation
- Data augmentation

### Data Augmentation Techniques

- Rotation
- Width Shift
- Height Shift
- Zoom
- Horizontal Flip

These techniques help improve model generalization and reduce overfitting.

---

## Model Architecture

The project uses a custom Convolutional Neural Network (CNN) consisting of:

- Convolutional Layers
- Max Pooling Layers
- Flatten Layer
- Fully Connected Dense Layers
- Sigmoid Output Layer for Binary Classification

### Classification Task

```text
Input Image
      ↓
Convolution Layers
      ↓
Pooling Layers
      ↓
Flatten
      ↓
Dense Layers
      ↓
Real / AI-Generated
```

---

## Training

The model was trained using:

- Binary Crossentropy Loss
- Adam Optimizer
- Mini-Batch Gradient Descent

Training performance was monitored using:

- Training Accuracy
- Validation Accuracy
- Training Loss
- Validation Loss

---

## Evaluation Metrics

The model was evaluated using:

- Accuracy
- Loss Curves
- Validation Performance

These metrics help assess how well the model generalizes to unseen images.

---

## Project Structure

```text
Real-and-Fake-Image-Classifier/
│
├── Real and Fake.ipynb
├── README.md
│
└── Dataset/
    ├── Train/
    │   ├── Real/
    │   └── Fake/
    │
    └── Test/
        ├── Real/
        └── Fake/
```

---

## How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/Real-and-Fake-Image-Classifier.git
cd Real-and-Fake-Image-Classifier
```

### 2. Install Dependencies

```bash
pip install tensorflow numpy matplotlib opencv-python
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open

```text
Real and Fake.ipynb
```

and run all cells.

---

## Applications

- AI-generated image detection
- Synthetic media analysis
- Fake content identification
- Digital media verification
- Computer vision research

---

## Future Improvements

- Train on larger and more diverse datasets
- Experiment with transfer learning models such as ResNet50 and EfficientNet
- Improve robustness against advanced generative AI models
- Deploy as a web application using Streamlit or FastAPI
- Add explainability techniques such as Grad-CAM

---

## Author

**Aryan Roy**

GitHub: https://github.com/YOUR_USERNAME

---

## License

This project is intended for educational and research purposes.
