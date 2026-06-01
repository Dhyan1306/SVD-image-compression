# SVD Image Compression

A Python-based image compression project that uses Singular Value Decomposition (SVD) to reduce image storage requirements while preserving visual quality.

Overview

Traditional image compression techniques often rely on predefined encoding schemes. This project explores a mathematical approach using Singular Value Decomposition (SVD) to create low-rank approximations of images.

By keeping only the most significant singular values, the image can be reconstructed with reduced storage requirements while maintaining acceptable visual quality.

Features

- Grayscale image compression using SVD
- Adjustable rank (k) for compression control
- Compression Ratio calculation
- PSNR (Peak Signal-to-Noise Ratio) evaluation
- Reconstruction Error analysis
- Singular Value visualization
- Color image compression using channel-wise SVD
- Comparison with JPEG compression

Technologies Used

- Python
- NumPy
- Matplotlib
- Pillow (PIL)
- Linear Algebra (SVD)

How It Works

1. Load an image and convert it into a matrix.
2. Apply Singular Value Decomposition:

   A = UΣVᵀ

3. Retain only the top k singular values.
4. Reconstruct the compressed image using:

   Ak = Uk Σk Vkᵀ

5. Compare quality using:
   - Compression Ratio
   - PSNR
   - Reconstruction Error

Project Workflow

Image → Matrix Representation → SVD Decomposition → Rank-k Approximation → Reconstructed Image → Performance Evaluation

Results

The project demonstrates that:

- Lower values of k provide higher compression but lower quality.
- Higher values of k preserve more image details.
- PSNR increases with increasing k.
- SVD can achieve significant compression while maintaining acceptable visual quality.

Performance Metrics

Compression Ratio

Measures storage reduction achieved through compression.

PSNR (Peak Signal-to-Noise Ratio)

Measures reconstruction quality relative to the original image.

Reconstruction Error

Measures information loss after compression.

Repository Structure
