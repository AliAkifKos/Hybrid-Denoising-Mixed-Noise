# Hybrid Denoising for Mixed Gaussian and Salt-and-Pepper Noise

This repository contains the implementation and experimental outputs of the Digital Image Processing final term project.

## Project Title

Confidence-Weighted Hybrid Image Denoising for Mixed Gaussian and Salt-and-Pepper Noise Removal

## Author

Ali Akif Köş  
Department of Mechanical Engineering  
Student ID: 2111041018

## Description

This project proposes a confidence-weighted hybrid image denoising framework for removing mixed Gaussian and salt-and-pepper impulse noise. The method first detects impulse-corrupted pixels using an adaptive local threshold, repairs corrupted pixels using median-based local statistics, applies BM3D for Gaussian denoising, and finally combines the repaired image and BM3D output using a spatial confidence map.

## Dataset

The experiments were conducted using grayscale images from the Kodak24 dataset. The images were resized before processing to reduce computational cost.

## Compared Methods

- Adaptive Median Filter
- Non-Local Means
- BM3D
- Proposed Confidence-Weighted Hybrid Method

## Evaluation Metrics

- PSNR
- SSIM
- Runtime

## Noise Conditions

Gaussian noise levels:

- sigma = 10
- sigma = 25

Salt-and-pepper impulse noise ratios:

- 5%
- 10%
- 20%

## Files

- `hybrid_denoising_colab_FINAL.ipynb`: Main Colab notebook
- `hybrid_denoising_final_outputs.zip`: Experimental outputs, figures, and result tables
- `full_results.csv`: Complete numerical results
- `summary_results_long.csv`: Average PSNR, SSIM, and runtime results
- `per_image_results.csv`: Per-image experimental results

## Requirements

The notebook uses the following Python libraries:

- numpy
- opencv-python
- matplotlib
- pandas
- scipy
- scikit-image
- bm3d

## Note

AI tools were used for language editing, structural organization, code debugging support, and formatting assistance. All experimental results and interpretations were reviewed and verified by the author.
