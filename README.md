# ENERGY-EFFICIENT-CANNY-EDGE-DETECTOR-FOR-ADVANCE-MOBILE-VISION-APPLICATION

## 📌 Project Overview

This project implements a custom version of the **Canny Edge Detection algorithm**, optimized step-by-step for **energy-efficient edge detection**, specifically targeted toward **advanced mobile vision applications**. Traditional edge detection methods are computationally expensive for mobile devices. Hence, we analyze and visualize each stage of Canny processing, aiming to improve interpretability and pave the way for optimization in low-power devices.

## 🔍 Key Features

- Six-step breakdown of Canny edge detection:
  1. **Gaussian Filtering** (Noise Reduction)
  2. **Sobel Gradient Calculation** (Edge Direction Estimation)
  3. **Gradient Magnitude & Orientation**
  4. **Non-Maximum Suppression** (Edge Thinning)
  5. **Double Thresholding**
  6. **Hysteresis Thresholding** (Edge Connectivity)

- **Modular Visualization** using Matplotlib for each step.
- **Manual implementation** of Non-Maximum Suppression and Hysteresis, providing full control over edge refinement.
- Optimized to reduce **redundant computation** and enable **mobile-aware adaptation**.

## 🎯 Motivation

In mobile devices, **energy constraints** are crucial. Traditional implementations like OpenCV’s built-in Canny are accurate but can be opaque and inefficient for energy-sensitive platforms. This project aims to:
- Decompose the algorithm for **custom lightweight implementation**
- Make it easier to integrate into **mobile vision systems**
- Support **edge-aware processing** in real-time with lower compute cost

## 🧠 Technologies Used

- **Python 3**
- **OpenCV** for image handling
- **NumPy** for matrix operations
- **Matplotlib** for step-by-step visual output

## 📸 Input

A grayscale image (e.g., `cat-play.png`) is used as the input. The process is generalizable to any grayscale input.

## ✅ Output

- Visual breakdown of each Canny step
- Final edge-detected image
- Potential for further optimization toward mobile platforms

## 🧪 Sample Results

| Step                          | Output                               |
|------------------------------|--------------------------------------|
| Gaussian Filter              | Smoothed image                       |
| Sobel Gradient               | Approximate edge gradients           |
| Gradient Magnitude           | Overall edge strength                |
| Non-Maximum Suppression      | Thinned edges                        |
| Double Thresholding          | Strong and weak edges classification |
| Hysteresis Thresholding      | Final connected edge map             |

## ⚙️ How to Run

```bash
# Install dependencies
pip install numpy opencv-python matplotlib

# Run the Python script
python energy_efficient_canny.py
