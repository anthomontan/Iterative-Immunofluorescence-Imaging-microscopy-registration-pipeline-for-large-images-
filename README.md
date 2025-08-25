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

## Usage

Use the Jupyter notebook

##  Parameters to edit :

cfg = RegistrationConfig(
    input_folder="/path/to/input",
    output_folder="/path/to/output",
    cache_folder="/path/to/cache",
    reference_dapi_file="/path/to/reference.tif",
    parallelization_strategy="pipeline",  # "rounds", "pipeline", or "tiles"
    use_padding=True,
    use_8bit_processing=True
)

##  Validation
The pipeline generates:

Alignment visualizations in the validation/ directory
Alignment metrics summary in alignment_summary.json
Registered images with _registered suffix

## Requirements:
torch>=2.0.0
opencv-python>=4.5.0
kornia>=0.6.0
pyvips>=2.1.16
tifffile>=2021.11.2
numpy>=1.21.0
matplotlib>=3.5.0

