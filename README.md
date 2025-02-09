# image-to-stereo3d

## Overview
A module for creating stereoscopic 3D videos by applying depth effects to 2D videos/images. This module processes input images with their corresponding depth maps to generate side-by-side stereoscopic output.

## Module Inputs
- **image**: Main image/video frame input (BufferedImage)
- **depth**: Optional depth map image input (BufferedImage)
- **depth-scale**: Numerical value to control the intensity of the 3D effect (Number)

## Module Outputs
- **stereo-image**: Side-by-side stereoscopic image output (BufferedImage)

## Notes
- If no depth map is provided, one will be automatically generated using Depth Anything V2
- The depth-scale parameter controls how pronounced the 3D effect is - positive values create normal 3D while negative values create inverted 3D
- Output is formatted as a side-by-side stereoscopic image suitable for 3D displays
