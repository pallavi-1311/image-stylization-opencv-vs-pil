# Image Stylization and Cartoonification Using OpenCV & PIL

This project compares two implementations for transforming images into artistic styles like cartoon, pencil sketch, watercolor, and comic book effects. One version uses **OpenCV**, while the other uses **PIL (Python Imaging Library)** and **NumPy**. The goal is to evaluate the output quality, visual metrics, and speed of each approach.

---

##  Project Goals

- Apply 4 stylization effects:
  - Cartoonify
  - Pencil Sketch
  - Watercolor
  - Comic Book
- Compare image quality using:
  - SSIM (Structural Similarity Index)
  - PSNR (Peak Signal-to-Noise Ratio)
  - MSE (Mean Squared Error)
  - Standard Deviation
- Measure execution time for each filter
- Help users decide which method is better for their needs: **OpenCV or PIL**

---

## Key Techniques Used

| Effect           | OpenCV-Based                             | PIL-Based                                |
|------------------|------------------------------------------|------------------------------------------|
| **Cartoonify**   | Adaptive threshold + bilateral filter     | Posterization + edge overlay             |
| **Pencil Sketch**| Gaussian blur + dodge blend              | Inversion + PIL blend + NumPy operations |
| **Watercolor**   | Edge-preserving filter                    | Posterization + soft blur approximation  |
| **Comic Book**   | Canny/Sobel + color quantization          | Posterization + contour + halftone       |

---

## Technologies & Libraries

- Python
- OpenCV
- PIL (Pillow)
- NumPy
- Matplotlib
- Skimage
- Google Colab

---

##  How It Works

1. Upload an image using Google Colab
2. Choose one or more stylization effects
3. The script:
   - Processes the image
   - Applies filters
   - Displays original vs stylized image side-by-side
   - Prints SSIM, PSNR, MSE, Std. Deviation
4. View which implementation performs better visually and computationally

---

##  Future Scope

- Add deep learning-based stylization (e.g., GANs)
- Extend support for video stylization
- Build a hybrid model using both PIL and OpenCV strengths
- Create a mobile-friendly version with TensorFlow Lite

---





