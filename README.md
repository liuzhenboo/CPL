# Camera-Calibration-through-Camera-Projection-Loss

Implementation of the paper "Camera Calibration through Camera Projection Loss": https://arxiv.org/pdf/2110.03479.pdf

Camera calibration is a necessity in various tasks including 3D reconstruction, hand-eye coordination for a robotic interaction, autonomous driving, etc. In this work we propose a novel method to predict extrinsic (baseline, pitch, and translation), intrinsic (focal length and principal point offset) parameters using an image pair. Unlike existing methods, instead of designing an end-to-end solution, we proposed a new representation that incorporates camera model equations as a
neural network in multi-task learning framework. We estimate the desired parameters via novel camera projection loss (CPL) that uses the camera model neural network to reconstruct the 3D points and uses the reconstruction loss to estimate the camera parameters. To the best of our knowledge, ours is the first method to jointly estimate both the intrinsic and extrinsic parameters via a multi-task learning methodology that combines analytical equations in learning framework
for the estimation of camera parameters. We also proposed a novel dataset using CARLA Simulator. Empirically, we demonstrate that our proposed approach achieves better performance with respect to both deep learning-based and traditional methods on 7 out of 10 parameters evaluated using both synthetic and real data.

# Code

Each model has been trained on the FAST-LUMS Camera Calibration Dataset while Tsinghua-Daimler Dataset has been used only for testing. 
Each folder contains 2 ipython notebooks, one for FAST-LUMS Dataset while the other for Tsinghua-Daimler Dataset.

# Weights and Logs

MTL-CPL-A: https://drive.google.com/drive/folders/16zR4Hn21VIgREbCr3AQlAAGMB6rT5rdw?usp=sharing

Deep-Homo: https://drive.google.com/drive/folders/1lrl1ccWgqRyb41rtZOW7CiL0DRA4SsF-?usp=sharing

MTL-Baseline: https://drive.google.com/drive/folders/1riHN9KyYmu06Pxvm7IXTiGGCdonAE5GO?usp=sharing

MTL-CPL-U: https://drive.google.com/drive/folders/1m1UHBzman_XJuF45HLeBHw1R3pbwdTif?usp=sharing

# Datasets

Format used for experiments: https://drive.google.com/drive/folders/1ScuaGjZSXslYPkFzGJMLzTze5QScvMKA?usp=sharing

Tsinghua-Daimler Dataset (Real Dataset): http://www.gavrila.net/Datasets/Daimler_Pedestrian_Benchmark_D/Tsinghua-Daimler_Cyclist_Detec/tsinghua-daimler_cyclist_detec.html

Some rellated articles are as follows:

How I got my MS Thesis Idea: https://thanifbutt.medium.com/how-i-got-my-thesis-idea-b64160a04d47

FAST-LUMS Camera Calibration Dataset: https://thanifbutt.medium.com/fast-lums-camera-calibration-dataset-98363918fcf6

# Citation

```
@article{butt2021camera,
  title={Camera Calibration through Camera Projection Loss},
  author={Butt, Talha Hanif and Taj, Murtaza},
  journal={arXiv preprint arXiv:2110.03479},
  year={2021}
}
```
