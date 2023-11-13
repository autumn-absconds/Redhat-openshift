# Redhat-CodeShift-Hackathon


# Advanced Vision : Background Transformation, Masking, and Captioning with U²-Net and OpenVINO™
---
## Overview

This Jupyter Notebook project leverages the power of OpenVINO™ and U²-Net to perform advanced image background manipulation. The primary functionalities of this notebook include image masking, background removal, background replacement, and automatic caption generation.

## Diagram View oF Model :
https://excalidraw.com/#json=lFaRKR996j30qVJocqYv1,6fGVtl43EZKThoahfaKOvA

## Features

1. **Image Masking:**
   - The notebook provides the capability to create masks for images, highlighting specific regions of interest.
   - ![Frame 1 (1)](https://github.com/autumn-absconds/Redhat-openshift/assets/65112908/f4df6207-478e-4718-8b50-7fe50c4e6d8a)


2. **Background Removal:**
   - Utilizing U²-Net and OpenVINO™, the notebook performs image segmentation to remove the background, isolating the main subject.
   - ![wepik--20231113085605JNYl](https://github.com/autumn-absconds/Redhat-openshift/assets/65112908/77c1eabd-fa05-4eed-81ea-5bf8523c0efa)


3. **Background Replacement:**
   - Users can seamlessly replace the removed background with a new one, offering creative possibilities for image enhancement.
   - ![wepik--202311130856328mrU](https://github.com/autumn-absconds/Redhat-openshift/assets/65112908/cdd4bb1f-f96b-4b0f-9970-43d8df8afd07)


4. **Automatic Caption Generation:**
   - The notebook incorporates the ability to generate captions for processed images, adding context and descriptive elements.
  
5. **Background_Blending:**
   - Users can blend the background with foreground image.
   - ![wepik--202311130857073BWX](https://github.com/autumn-absconds/Redhat-openshift/assets/65112908/4191fe44-0887-4bb7-9015-9442610eec72)


## Project Structure

### Original Model Integration
The project starts by importing and loading the U²-Net model implemented in PyTorch. This model is then converted into OpenVINO™ Intermediate Representation (IR), enhancing its compatibility with the OpenVINO™ toolkit.

### Device Selection
Users have the flexibility to choose the target device for inference, with options including CPU, GPU, or the default setting with automatic device selection.

### Image Processing Pipeline
1. **Input Image Loading:**
   - Images to be processed are loaded into the notebook. It's important to note that OpenCV reads images in BGR format, while the OpenVINO™ IR model expects images in RGB format.

2. **U²-Net Inference for Segmentation:**
   - The notebook performs image segmentation using the loaded U²-Net model and OpenVINO™ runtime. This step generates masks that highlight the regions of interest.

3. **Background Replacement:**
   - After obtaining the segmentation masks, the notebook loads the target image that will replace the removed background. The necessary preprocessing is applied to align the image with the RGB format expected by the OpenVINO™ IR model. The new background is seamlessly inserted into the masked area.

## Usage Instructions

1. **Environment Setup:**
   - Ensure that the required dependencies, including OpenVINO™ and PyTorch, are installed in the environment.

2. **Run the Notebook:**
   - Execute the Jupyter Notebook cells sequentially, following the provided instructions.

3. **Interact with User Prompts:**
   - Choose the target device for inference and provide input images as instructed by the notebook.

4. **Explore Results:**
   - Examine the generated masks, images with removed backgrounds, and images with replaced backgrounds.

5. **Caption Generation:**
   - Optionally, explore automatic caption generation for the processed images.

## Conclusion

This project enhances the capabilities of OpenVINO™ for image processing, enabling users to manipulate backgrounds creatively. The integration of U²-Net further refines the segmentation process, leading to precise background removal and replacement. Whether for artistic expression or practical applications, this notebook provides a versatile toolkit for image enhancement.

---

