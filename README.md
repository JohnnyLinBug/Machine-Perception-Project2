
# NeRF 3D Reconstruction Project

## Overview
This project explores the use of Neural Radiance Fields (NeRF) for 3D object and scene reconstruction. Using the Nerfstudio framework, we trained NeRF models on public and custom datasets, comparing the quality and efficiency of reconstructions. The project aims to understand the training process, evaluate dataset impact, and generate 3D videos from captured images.

## Features
- **Framework**: Nerfstudio for NeRF implementation and interactive training monitoring.
- **Datasets**: Public datasets and custom datasets captured from various viewpoints.
- **Training Process**:
  - Verification of dependencies (e.g., COLMAP, Python version).
  - Image preprocessing and parameter tuning.
  - Real-time interactive monitoring via Nerfstudio Viewer.
- **Output**: High-quality 3D reconstructions and custom 3D videos from trained models.

## Project Highlights
1. **Dataset Analysis**: Public datasets provided clearer outputs due to diverse and high-quality image coverage.
2. **Training Process**: Iterative optimization using the Nerfstudio Viewer for real-time feedback on convergence and quality.
3. **3D Video Generation**: Custom camera paths were designed to render videos showcasing the reconstructed models.

## Dependencies
- Python 3.10
- Nerfstudio
- COLMAP
- tinycudann
- Public and custom image datasets

## Installation
1. Verify Python version:
   ```bash
   python --version
   ```
   Ensure Python 3.10 is installed.

2. Install dependencies:
   ```bash
   pip install tinycudann-1.7-cp310-cp310-linux_x86_64.whl
   pip install nerfstudio
   ```

3. Install COLMAP:
   Follow [COLMAP installation instructions](https://colmap.github.io/).

4. Load datasets:
   - For public datasets, download images from a trusted source.
   - For custom datasets, ensure consistent resolution and format.

## Usage
1. Preprocess images using COLMAP.
2. Launch Nerfstudio Viewer for interactive parameter adjustment:
   ```bash
   nerfstudio viewer
   ```
3. Start training and monitor metrics such as rays/sec, loss, and output quality.
4. Use the viewer to create custom camera paths and render 3D videos:
   ```bash
   nerfstudio render --path /path/to/camera/settings
   ```

## Results
- **Custom Images**: Initial reconstructions showed artifacts and blurriness, improving over time but limited by coverage and resolution.
- **Public Images**: Outputs were clearer and more detailed, with faster training convergence due to dataset quality.
- **3D Videos**: Smooth and high-quality videos were created from reconstructed models using custom camera paths.

## Discussion
The project demonstrates the critical role of dataset quality and diversity in NeRF training. Public datasets provided better reconstruction, while custom datasets required careful planning. The Nerfstudio framework enhanced the efficiency and flexibility of the training process, offering valuable tools for real-time monitoring and adjustments.

## Team Members
- Johnny (Zhongyu) Lin
- Matt (Zitong) Wei
- Boshen Pan

--- 

Feel free to adjust details as needed!
