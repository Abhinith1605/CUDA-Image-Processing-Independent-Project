# CUDA Image Processing Independent Project  
### GPU-Accelerated Gaussian Blur + Sobel Edge Detection on 100 Images

## Overview
This project implements **GPU-accelerated image processing** using **CUDA** and **OpenCV**.  
It processes **100 JPG images** using two CUDA kernels executed on the GPU:

**Gaussian Blur (CUDA)**  
**Sobel Edge Detection (CUDA)**  

The application loads all images from `data/input`, processes them on the GPU, and writes results to `data/output`.  
This fulfills all the requirements of the **CUDA at Scale Independent Project**, including:

- Using CUDA kernels  
- Handling large data (100 small images)  
- Public GitHub repository  
- Proof of code execution  
- Documentation (this README)


---

## Features

### GPU Gaussian Blur  
CUDA kernel using shared memory + 5×5 Gaussian filter.

### GPU Sobel Edge Detection  
CUDA kernel computing Sobel X and Y gradients + magnitude.

### Batch Processing  
Automatically processes all images in the input folder.

### OpenCV Integration  
Used for loading, converting, and saving images.

---

## Requirements

### Software
- **CUDA Toolkit 13.0+**
- **Visual Studio 2022 Build Tools (MSVC v143)**
- **CMake 3.25+**
- **OpenCV 4.10.0 (prebuilt Windows release)**

### Hardware
- NVIDIA GPU (Compute Capability 7.5 or higher recommended)

---

## Running the Project (Windows)

⚠ Use **"x64 Native Tools Command Prompt for VS 2022"** — NOT PowerShell.


---

## ▶Running the Program

### Standard run:

- The output is already uploaded in the repository. You can access it by going to Build --> Release --> data --> output.
- If you want to run it yourself again you may delete all the picture in the above mentioned folder. (200 jpg files)

- Note: Before running the command bellow make sure your directory is set to the release folder which is inside the build folder.

command: cuda_image_processor.exe "....\data\input" "....\data\output"

Now open the data folder.
Then open the output folder.

The output folder should contain the processed images both blurred and edge detected.


---

## Proof of Execution

Link: https://drive.google.com/file/d/1Dm-u7bDpmQj4roMJfyAE7rxhkAdDnHdL/view?usp=sharing

---

## Data Source (Images)

Link: https://github.com/YoongiKim/CIFAR-10-images