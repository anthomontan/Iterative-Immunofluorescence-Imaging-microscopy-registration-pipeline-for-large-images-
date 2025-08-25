# Iterative-Immunofluorescence-Imaging-microscopy-registration-pipeline-for-large-images-
"CENTERED padding-based microscopy multiplex image registration pipeline with 8-bit conversion and automatic hardware detection using a reference image and multiple rounds

A robust microscopy image registration pipeline using CENTERED padding strategy with automatic hardware detection (GPU/CPU).

## Features

- CENTERED padding for proper alignment across all images
- 8-bit conversion for memory efficiency
- Automatic hardware detection (uses all GPUs → 1 GPU → CPU)
- Comprehensive alignment validation with visualizations
- Multiple parallelization strategies
- Proper transformation matrix handling

## Requirements

- Python 3.10+
- PyTorch
- OpenCV
- Kornia
- PyVIPS
- Tifffile
- NumPy

## Installation

pip install torch opencv-python kornia pyvips tifffile numpy matplotlib
