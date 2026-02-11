# CNN Visualizer for Handwritten Digit Recognition

An interactive **PyTorch + Tkinter** application that visualizes how a **Convolutional Neural Network (CNN)** processes handwritten digits in real time.

Instead of treating the model as a black box, this project focuses on **making the internal behavior of a CNN visible**, including prediction probabilities and hidden layer activations.

---

## Key Features

-  **Real-time drawing interface** (28×28 pixel grid)
-  **Live prediction probabilities** for digits 0–9
-  **Hidden layer visualization** to show intermediate CNN representations
-  Automatic model loading (or training if no saved model is found)
-  Designed for learning and explanation, not just accuracy

---

##  Motivation

Most CNN demos only show the final prediction.  
This project was built to **bridge the gap between theory and intuition** by answering questions like:

- What does a CNN actually “see” after convolution?
- How do hidden layers transform raw pixels into abstract features?
- How does confidence change as the input evolves?

The goal is **conceptual understanding**, especially for students learning deep learning.

---

##  Model Overview

- Input: 28×28 grayscale image
- Architecture:
  - Convolution + ReLU + MaxPooling layers
  - Fully connected layers for classification
- Output:
  - Probability distribution over digits (0–9)
  - Hidden layer activations for visualization


---
## Project Structure

Make sure your project folder looks like this:

```text
CNN-Visualizer-for-Handwritten-Digit-Recognition/
├─ requirements.txt
├─ README.md
├─ Hand Writing Recognition/
│  ├─ Handwritten_Digit_Recognition.py
│  └─ mnist_cnn.pth
```


##  How to Run (Windows)

```bash
python -m venv .venv
.\.venv\Scripts\activate
pip install -r requirements.txt
python "Hand Writing Recognition/Handwritten_Digit_Recognition.py"
