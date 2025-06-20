# deep-learning-labs

# 🧠 Deep Learning Mini Projects – Vision Tasks

This repo contains two simple but complete computer vision experiments using PyTorch: neural style transfer and lightweight image super-resolution. Each is implemented in a standalone Jupyter notebook and demonstrates practical understanding of image preprocessing, model usage, and visualization.

---

## 🎨 1. Neural Style Transfer (Task1.ipynb)

**Goal:** Generate an image that combines the content of one image with the style of another using a pre-trained VGG19 model.

**Highlights:**
- Uses `torchvision.models.vgg19` features for both style and content representation
- Implements Gram matrix for style loss
- Custom total loss: content loss + style loss
- Optimized with L-BFGS
- Outputs stylized result image

**Usage:**  
Run the cells in order inside `Task1.ipynb` and modify content/style images as needed.

---

## 🔍 2. Lightweight Super-Resolution (Task2.ipynb)

**Goal:** Upsample a low-resolution image using a lightweight convolutional architecture based on SqueezeNet.

**Highlights:**
- Uses `torchvision.models.squeezenet1_1` as a base
- Adds a simple upsampling head (bilinear interpolation + Conv layers)
- Can upscale images by a fixed factor (default x2)
- Visualizes side-by-side: original vs. upsampled image

**Usage:**  
Run all cells in `Task2.ipynb`, can change input image path at the top.

---

## 📦 Requirements

- Python 3.8+
- PyTorch
- torchvision
- matplotlib
- PIL

Install with:

```bash
pip install torch torchvision matplotlib pillow
```

---

## 📁 File List

- `Task1.ipynb` — Neural Style Transfer
- `Task2.ipynb` — Super-Resolution with lightweight CNN

---


