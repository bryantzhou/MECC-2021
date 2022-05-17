# Real-Time Adaptive Threshold Adjustment for Lane Detection Application under Different Lighting Conditions using Model-Free Control

This project uses model-free control (MFC) for lane detection tasks. Lane detection is performed in the hue/saturation/value (HSV) color space, without the need of edge-detection algorithms, filters, or post-processing. This method is based entirely on the color information of lane marks, and MFC is introduced to deal with the illumination variation. For detailed problem formulation and MFC explanation, we refer the reader to read our paper.

## Paper

For a full description of the algorithm itself and the lane detection resuls from a simulation study, please refer to the paper.

If you find this repository useful, please do cite the paper:

```
@article{zhou2021real,
  title={Real-Time Adaptive Threshold Adjustment for Lane Detection Application under Different Lighting Conditions using Model-Free Control},
  author={Zhou, Yujing and Wang, Zejiang and Wang, Junmin},
  journal={IFAC-PapersOnLine},
  volume={54},
  number={20},
  pages={147--152},
  year={2021},
  publisher={Elsevier}
}
```

## Primary Contributor

The primary contributor is Yujing "Bryant" Zhou, an incoming Ph.D. student at Princeton University. If you have specific questions about this repository, please post an issue.

## Language

MATLAB and Simulink are primarily used for this project. A minimum version of MATLAB-R-2020-a is required.

The [QUARC](https://www.quanser.com/products/quarc-real-time-control-software/) real-time control software is required to run the Simulink files for simulation tests.

## File Description

### Video Code

Algorithms in this folder are the lane detection implementation based on collected video from a sclaed car. In this folder, one file is without the proposed controller, which means that constant thresholds in the HSV color space are used. The other file is with the proposed adaptive thresholds. 

### Camera Code

Algorithms in this folder are the lane detection implementation with real-time camera data feeded to the controller. In this folder, one file is without the proposed controller, which means that constant thresholds in the HSV color space are used. The other file is with the proposed adaptive thresholds. 

## Data

Some collected video in the MATLAB data format can be accessed from [here](https://drive.google.com/drive/folders/1bZGDqvF4--pjeDhtrCnN2td2j0eXtXH3?usp=sharing)
