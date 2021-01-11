# IAI Kinect2 - Ubuntu18.04 Jetson Boards

This is a fork of [iai_Kinect2](https://github.com/code-iai/iai_kinect2) (**thank you again for your incredible work**), created and tested to work on Nvidia Jetson boards (TX2, Xavier, NX).

Follow the instructions on the original [source](https://github.com/code-iai/iai_kinect2) to install and to compile libfreenect2 for GPU acceleration support.

## Table of contents
- [Description](#description)
- [Tested configuration](#tested-configuration)
- [Launch with GPU acceleration OpenCL/CUDA](#launch-with-gpu-acceleration-opencl/cuda)
- [Citations](#citation)
- [Screenshots](#screenshots)

## Description

This code was edited to work with **OpenCV4** but should work with every board

## Tested configuration

- OpenCV4 compiled for CUDA
- Ubuntu 18.04 ROS Melodic
- Jetson TX2 8Gb RAM on Connectech Board Spaceley
- **Ubuntu 18.04**
- **Jetpack 4.4.1 L4T 32.4.4**
- **CUDA 10.2.89**
- **OpenCV 4.1.2 (compiled for CUDA)**
- TensorRT 7.1.3.0
- VPI: 0.4.4
- VisionWorks 1.6.0.501
- Vulkan 1.2.70
- cuDNN 8.0.0.100
- **OpenCL enabled ([source](https://gist.github.com/madelinegannon/237733e6c114f156b31366f47c1f3d32))**
- **Jetpack >= 4.4 (L4T 32.4.4 in my case)**

## Launch with GPU acceleration OpenCL/CUDA

Connect your sensor and run `kinect2_bridge`:

```bash
roslaunch kinect2_bridge kinect2_bridge.launch _reg_method:=cpu _depth_method:=opencl
```

## Credits

```
T. Wiedemeyer, “IAI Kinect2,” https://github.com/code-iai/iai_kinect2,
Institute for Artificial Intelligence, University Bremen, 2014 – 2015,
accessed June 12, 2015.
```
