# Low-Light Image Enhancement using Improved Retinex Model

## Overview

This project focuses on enhancing images captured in low-light conditions using an improved Retinex-based algorithm. The objective is to improve brightness, contrast, and visibility while preserving important details and minimizing noise.

The implementation is based on a research paper and combines multiple techniques such as multi-scale illumination estimation, guided filtering, Weber–Fechner law, and PCA-based fusion.

---

## Problem Statement

Images captured under poor lighting conditions often suffer from:

- Low brightness  
- Poor contrast  
- Noise  
- Loss of important details  

Traditional image enhancement methods may improve brightness but often lead to over-enhancement and unnatural appearance.

This project aims to solve these issues using a structured and perceptually motivated approach.

---

## Methodology

The enhancement pipeline consists of the following steps:

1. Convert RGB image to HSV color space  
2. Extract the brightness component (V channel)  
3. Estimate illumination using multi-scale guided filtering  
4. Compute reflection component  
5. Enhance illumination using Weber–Fechner law  
6. Enhance reflection using CLAHE and denoising  
7. Fuse illumination and reflection using PCA  
8. Apply adaptive saturation stretching  
9. Reconstruct the final enhanced image in RGB  

---

## Technologies Used

- Python  
- OpenCV  
- NumPy  
- Matplotlib  
- Scikit-image  
- Scikit-learn  

---

## Project Structure

low-light-image-enhancement-retinex

low_light_enhancement.ipynb
README.md
requirements.txt
input.jpg
output.jpg
paper.pdf


## How to Run

1. Install required libraries:

pip install -r requirements.txt

2. Place your input image in the project folder:

input.jpg


3. Run the program:

python main.py


4. The enhanced output will be saved as:


output.jpg


---

## Results

After applying the algorithm:

- Image brightness improves significantly  
- Dark regions become more visible  
- Edge details are preserved  
- Noise is reduced compared to basic methods  

---

## Limitations

- Requires parameter tuning for different images  
- Computationally expensive due to multi-scale processing  
- Slight over-enhancement may occur in some regions  
- Performance depends on input image quality  

---

## Future Scope

- Real-time implementation  
- Automatic parameter tuning  
- Integration with deep learning models  
- Testing on larger datasets  

---

## Citation

This project is based on the following research paper:

**"An Improved Retinex-Based Low-Light Image Enhancement Algorithm Using Multi-Scale Illumination Estimation and Guided Filtering"**

Please refer to the `Research Paper MSR.pdf` file included in this repository for complete details.

---

## Author
Shathakshi V
241EC250
NITK Surathkal
