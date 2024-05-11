
# How to Install CUDA DLLs

If you're encountering issues with missing cublas and cudart DLLs, you can resolve these by installing the correct DLLs using the CUDA Toolkit installer.

This guide will specifically detail the steps for a custom installation to acquire only the necessary runtime components.
## Step 1: Download the CUDA Toolkit

Visit the NVIDIA CUDA Downloads page to download the appropriate version of the CUDA Toolkit.

- **URL**: [CUDA Toolkit Download](https://developer.nvidia.com/cuda-downloads?target_os=Windows&target_arch=x86_64)
- Choose version 10 or 11, depending on your Windows version.
  ![alt text](<images/Untitled 1.png>)

## Step 2: Select the Installer Type

There are two types of installers:

1. **Network Installer**: Recommended for cases where you're downloading only the needed packages.
2. **Local Installer**: Recommended for low-bandwidth networks, download the executable and proceed with installation.
   
![alt text](<images/Untitled 2.png>)

## Step 3: Installing CUDA DLLs with the NVIDIA Installer

Follow these steps to install CUDA on your system:

### System Check

The NVIDIA Installer will first perform a system check to ensure compatibility.

![alt text](<images/Untitled 3.png>)

### Software License Agreement

Read and accept the NVIDIA software license agreement to proceed with the installation.

![alt text](<images/Untitled 4.png>)

### Installation Options

Select the Custom installation option as we are only interested in specific components.

![alt text](<images/Untitled 5.png>)

### Custom Installation Options

Choose specific components to install. Ensure the CUDA Runtime and Libraries are selected.

![alt text](<images/Untitled 6.png>)
![alt text](<images/Untitled 7.png>)

### Select Installation Location

Choose the directory for CUDA Toolkit installation.

![alt text](<images/Untitled 8.png>)

### Download and Installation

Allow the installer to download and install the selected components.

![alt text](<images/Untitled 9.png>)

### Installation Complete

Review the installed components and their versions.

![alt text](<images/Untitled 10.png>)

## Step 4: Copy the DLL Files

After installation, navigate to the CUDA binaries folder:

- **Path**: `C:\Program Files\NVIDIA GPU Computing Toolkit\CUDA\v12.4\bin`

Copy all DLL files from this directory.

## Step 5: Paste the DLL Files

Paste the copied DLL files into the Hyperspace installation folder:

- **Path**: `%localappdata%/Hyperspace`

![alt text](<images/Untitled 11.png>)

## Conclusion

After following these steps, you should be able to successfully run software that supports CUDA.
