# 6DOF Robot Grasping
This repositry is for saving collection of papers related to computer vision (CV) & geometry based 6DOF robot grasping. We only collect methods using RGB/RGB-D with Deep Learning. Note that grasp pose detection related papers are **ROUGHLY** divided based on their approaches. The list below will be updated in regular basis. 

## Table of Contents

- [6D Object Pose Estimation](#6d-object-pose-estimation)
    - [RGB based](#rgb-based)
    - [RGB-D based](#rgb-d-based)
    - [Survey (OPE)](#survey-ope)
    - [Datasets (OPE)](#datasets-ope)
- [6D Grasp Pose Detection](#6d-grasp-pose-detection)
    - [Sampler focused](#sampler-focused)
    - [Reconstruction focused](#reconstruction-focused)
    - [Discriminater focused](#discriminater-focused)
    - [Regression focused](#discriminater-focused)
    - [Survey (GPD)](#survey-gpd)
    - [Datasets (GPD)](#datasets-gpd)
- [Grasp Quality Metrics](#grasp-quality-metrics)
    - [Combined metrics](#combined-metrics)
- [ToDo Lists](#todo-lists)

---

## 6D Object Pose Estimation

### RGB based
- [PoseCNN: A Convolutional Neural Network for 6D Object Pose Estimation in Cluttered Scenes](https://arxiv.org/pdf/1711.00199.pdf)
- [SSD-6D: Making RGB-Based 3D Detection and 6D Pose Estimation Great Again](https://arxiv.org/pdf/1711.10006v1.pdf)
- [PVNet: Pixel-wise Voting Network for 6DoF Pose Estimation](https://arxiv.org/pdf/1812.11788.pdf)
- [Augmented Autoencoders: Implicit 3D Orientation Learning for 6D Object Detection](https://arxiv.org/pdf/1902.01275v2.pdf)
- [Pix2Pose: Pixel-Wise Coordinate Regression of Objects for 6D Pose Estimation](https://arxiv.org/pdf/1908.07433v1.pdf)
- [DPOD: 6D Pose Object Detector and Refiner](https://arxiv.org/pdf/1902.11020v3.pdf)
- [EPOS: Estimating 6D Pose of Objects with Symmetries](https://arxiv.org/pdf/2004.00605v1.pdf)
- [HybridPose: 6D Object Pose Estimation under Hybrid Representations](https://arxiv.org/pdf/2001.01869.pdf)
- [EfficientPose: An efficient, accurate and scalable end-to-end 6D multi object pose estimation approach](https://arxiv.org/pdf/2011.04307v2.pdf)
  
### RGB-D based
- [SegICP: Integrated Deep Semantic Segmentation and Pose Estimation](https://arxiv.org/pdf/1703.01661.pdf)
- [Drost-PPF: Going Further with Point Pair Features](https://arxiv.org/pdf/1711.04061.pdf)
- [DenseFusion: 6D Object Pose Estimation by Iterative Dense Fusion](https://arxiv.org/pdf/1901.04780.pdf)
- [PVN3D: A Deep Point-wise 3D Keypoints Voting Network for 6DoF Pose Estimation](https://arxiv.org/pdf/1911.04231.pdf)
- [MaskUKF: An Instance Segmentation Aided Unscented Kalman Filter for 6D Object Pose and Velocity Tracking](https://www.frontiersin.org/articles/10.3389/frobt.2021.594583/full)
- [FFB6D: A Full Flow Bidirectional Fusion Network for 6D Pose Estimation](https://arxiv.org/pdf/2103.02242.pdf)
- [Unseen Object 6D Pose Estimation: A Benchmark and Baselines](https://arxiv.org/pdf/2206.11808.pdf)
- [SO(3)-Pose: SO(3)-Equivariance Learning for 6D Object Pose Estimation](https://arxiv.org/pdf/2208.08338v1.pdf)

### Survey (OPE)
- [Pose Estimation of Specific Rigid Objects](https://arxiv.org/pdf/2112.15075.pdf)

### Datasets (OPE)
- [BOP: Benchmark for 6D Object Pose Estimation](https://bop.felk.cvut.cz/datasets/)
  
## 6D Grasp Pose Detection

### Sampler focused
- [6-DOF GraspNet: Variational Grasp Generation for Object Manipulation](https://arxiv.org/pdf/1905.10520.pdf)
- [6-DOF Grasping for Target-driven Object Manipulation in Clutter](https://arxiv.org/pdf/1912.03628.pdf)
- [GraspNet-1Billion: A Large-Scale Benchmark for General Object Grasping](https://openaccess.thecvf.com/content_CVPR_2020/papers/Fang_GraspNet-1Billion_A_Large-Scale_Benchmark_for_General_Object_Grasping_CVPR_2020_paper.pdf)
- [Volumetric Grasping Network: Real-time 6 DOF Grasp Detection in Clutter](https://arxiv.org/pdf/2101.01132.pdf)
- [Contact-GraspNet: Efficient 6-DoF Grasp Generation in Cluttered Scenes](https://arxiv.org/pdf/2103.14127.pdf)
- [RGB Matters: Learning 7-DoF Grasp Poses on Monocular RGBD Images](https://arxiv.org/pdf/2103.02184.pdf)
- [Graspness Discovery in Clutters for Fast and Accurate Grasp Detection](https://openaccess.thecvf.com/content/ICCV2021/papers/Wang_Graspness_Discovery_in_Clutters_for_Fast_and_Accurate_Grasp_Detection_ICCV_2021_paper.pdf)
- [Efficient and Accurate Candidate Generation for Grasp Pose Detection in SE(3)](https://arxiv.org/pdf/2204.01131.pdf)
- [REGNet: REgion-based Grasp Network for End-to-end Grasp Detection in Point Clouds](https://arxiv.org/pdf/2002.12647.pdf)
- [Hybrid Physical Metric For 6-DoF Grasp Pose Detection](https://arxiv.org/pdf/2206.11141.pdf)
    
    
### Reconstruction focused
- [Robotic Grasping through Combined Image-Based Grasp Proposal and 3D Reconstruction](https://arxiv.org/pdf/2003.01649.pdf)

### Discriminater focused
- [PointNetGPD: Detecting Grasp Configurations from Point Sets](https://web.cs.ucla.edu/~xm/file/pointnetgpd_icra19.pdf)
- [Collision-Aware Target-Driven Object Grasping in Constrained Environments](https://arxiv.org/pdf/2104.00776.pdf)
- [GPR: Grasp Pose Refinement Network for Cluttered Scenes](https://arxiv.org/pdf/2105.08502.pdf)
- [Simultaneous Semantic and Collision Learning for 6-DoF Grasp Pose Estimation](https://arxiv.org/pdf/2108.02425.pdf)

### Regression focused
- [S4G: Amodal Single-view Single-Shot SE(3) Grasp Detection in Cluttered Scenes](https://arxiv.org/pdf/1910.14218.pdf)
- [Synergies Between Affordance and Geometry: 6-DoF Grasp Detection via Implicit Representations](https://arxiv.org/pdf/2104.01542.pdf)
    
### Survey (GPD)
- [Robotic Grasping from Classical to Modern: A Survey](https://arxiv.org/pdf/2202.03631.pdf)
- [Deep Learning Approaches to Grasp Synthesis: A Review](https://arxiv.org/pdf/2207.02556.pdf)
- [Vision‑based robotic grasping from object localization, object pose estimation to grasp estimation for parallel grippers: a review](https://link.springer.com/content/pdf/10.1007/s10462-020-09888-5.pdf)

### Datasets (GPD)
- [GraspNet](https://graspnet.net/index.html)

## Grasp Quality Metrics

### Combined metrics
- [Characterisation of Grasp Quality Metrics](http://repositori.uji.es/xmlui/bitstream/handle/10234/168278/rubert_2017.pdf;jsessionid=20C8040BDAD3A1F806E56730E54A5FB9?sequence=1)
- [Grasp success prediction with quality metrics](https://arxiv.org/pdf/1809.03276v1.pdf)

## ToDo Lists
- [x] Divide subsection for different approaches in *6D Grasp Pose Detection*
