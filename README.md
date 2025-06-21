#  Image Stylization and Cartoonification Using OpenCV & PIL

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

##  Key Techniques Used

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


##  Sample Output Metrics

| Metric        | OpenCV Model | PIL + NumPy Model |
|---------------|--------------|-------------------|
| **SSIM**      | Higher       | Lower             |
| **PSNR**      | Higher       | Lower             |
| **MSE**       | Lower        | Higher            |
| **Std. Dev.** | Slightly higher | Lower         |
| **Speed**     | Faster       | Slower            |

 **Observation:**  
OpenCV outperforms PIL+NumPy in most quality metrics and is better suited for real-time and high-precision applications. PIL-based implementation is simpler but more suited for basic stylization and offline use.

---

##  Future Scope

- Add deep learning-based stylization (e.g., GANs)
- Extend support for video stylization
- Build a hybrid model using both PIL and OpenCV strengths
- Create a mobile-friendly version with TensorFlow Lite

---


