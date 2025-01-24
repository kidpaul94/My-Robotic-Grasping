# My Robotic Grasping
This repositry is for saving papers related to CV- & geometry-based 6DOF robotic grasping. We **MAINLY** collect methods utilizing Deep Learning. Note that grasp pose detection related papers are **ROUGHLY** divided based on their approaches. The list below will be updated in regular basis. 

## Table of Contents

- [6D Object Pose Estimation](#6d-object-pose-estimation)
    - [RGB based](#rgb-based)
    - [RGB-D based](#rgb-d-based)
    - [Towards Generalization](#towards-generalization)
    - [Survey (OPE)](#survey-ope)
    - [Datasets (OPE)](#datasets-ope)
- [6D Grasp Pose Detection](#6d-grasp-pose-detection)
    - [Generative methods](#generative-methods)
    - [Reconstruction methods](#reconstruction-methods)
    - [Discriminative methods](#discriminative-methods)
    - [Regression methods](#regression-methods)
    - [Neural Representation methods](#neural-representation-methods)
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
- [ZebraPose: Coarse to Fine Surface Encoding for 6DoF Object Pose Estimation](https://openaccess.thecvf.com/content/CVPR2022/papers/Su_ZebraPose_Coarse_To_Fine_Surface_Encoding_for_6DoF_Object_Pose_CVPR_2022_paper.pdf)
  
### RGB-D based
- [SegICP: Integrated Deep Semantic Segmentation and Pose Estimation](https://arxiv.org/pdf/1703.01661.pdf)
- [DenseFusion: 6D Object Pose Estimation by Iterative Dense Fusion](https://arxiv.org/pdf/1901.04780.pdf)
- [PVN3D: A Deep Point-wise 3D Keypoints Voting Network for 6DoF Pose Estimation](https://arxiv.org/pdf/1911.04231.pdf)
- [MaskUKF: An Instance Segmentation Aided Unscented Kalman Filter for 6D Object Pose and Velocity Tracking](https://www.frontiersin.org/articles/10.3389/frobt.2021.594583/full)
- [FFB6D: A Full Flow Bidirectional Fusion Network for 6D Pose Estimation](https://arxiv.org/pdf/2103.02242.pdf)
- [Multi-path Learning for Object Pose Estimation Across Domains](https://openaccess.thecvf.com/content_CVPR_2020/papers/Sundermeyer_Multi-Path_Learning_for_Object_Pose_Estimation_Across_Domains_CVPR_2020_paper.pdf)
- [StablePose: Learning 6D Object Poses from Geometrically Stable Patches](https://openaccess.thecvf.com/content/CVPR2021/papers/Shi_StablePose_Learning_6D_Object_Poses_From_Geometrically_Stable_Patches_CVPR_2021_paper.pdf)
- [Unseen Object 6D Pose Estimation: A Benchmark and Baselines](https://arxiv.org/pdf/2206.11808.pdf)
- [SO(3)-Pose: SO(3)-Equivariance Learning for 6D Object Pose Estimation](https://arxiv.org/pdf/2208.08338v1.pdf)

### Towards Generalization

Researchers have recently started to investigate methods to make 6D Object Pose Estimation more generalizable. As approaches to enhance generalizability vary, we separated the list from the RGB- and RGBD-based approaches above. A lot of generalizable 6D Object Pose Estimation approaches (#-shot) are multi-stages, and utilize template matching (e.g., support images and CAD models) + classification that NNs are good at.

- [EPro-PnP: Generalized End-to-End Probabilistic Perspective-n-Points for Monocular Object Pose Estimation](https://arxiv.org/pdf/2303.12787v2.pdf)
- [OnePose: One-Shot Object Pose Estimation without CAD Models](https://openaccess.thecvf.com/content/CVPR2022/papers/Sun_OnePose_One-Shot_Object_Pose_Estimation_Without_CAD_Models_CVPR_2022_paper.pdf)
- [Templates for 3D Object Pose Estimation Revisited: Generalization to New Objects and Robustness to Occlusions](https://openaccess.thecvf.com/content/CVPR2022/papers/Nguyen_Templates_for_3D_Object_Pose_Estimation_Revisited_Generalization_to_New_CVPR_2022_paper.pdf)
- [OnePose++: Keypoint-Free One-Shot Object Pose Estimation without CAD Models](https://proceedings.neurips.cc/paper_files/paper/2022/file/e43f900f571de6c96a70d5724a0fb565-Paper-Conference.pdf)
- [POPE: 6-DoF Promptable Pose Estimation of Any Object, in Any Scene, with One Reference](https://arxiv.org/pdf/2305.15727.pdf)
- [Learning to Estimate 6DoF Pose from Limited Data: A Few-Shot, Generalizable Approach using RGB Images](https://arxiv.org/pdf/2306.07598.pdf)
- [OVE6D: Object Viewpoint Encoding for Depth-based 6D Object Pose Estimation](https://openaccess.thecvf.com/content/CVPR2022/papers/Cai_OVE6D_Object_Viewpoint_Encoding_for_Depth-Based_6D_Object_Pose_Estimation_CVPR_2022_paper.pdf)
- [GigaPose: Fast and Robust Novel Object Pose Estimation via One Correspondence](https://openaccess.thecvf.com/content/CVPR2024/papers/Nguyen_GigaPose_Fast_and_Robust_Novel_Object_Pose_Estimation_via_One_CVPR_2024_paper.pdf)
- [SAM-6D: Segment Anything Model Meets Zero-Shot 6D Object Pose Estimation](https://openaccess.thecvf.com/content/CVPR2024/papers/Lin_SAM-6D_Segment_Anything_Model_Meets_Zero-Shot_6D_Object_Pose_Estimation_CVPR_2024_paper.pdf)

### Survey (OPE)
- [Pose Estimation of Specific Rigid Objects](https://arxiv.org/pdf/2112.15075.pdf)

### Datasets (OPE)
- [BOP: Benchmark for 6D Object Pose Estimation](https://bop.felk.cvut.cz/datasets/)
  
## 6D Grasp Pose Detection

### Generative methods
- [6-DOF GraspNet: Variational Grasp Generation for Object Manipulation](https://arxiv.org/pdf/1905.10520.pdf)
- [UniGrasp: Learning a Unified Model to Grasp with Multifingered Robotic Hands](https://arxiv.org/pdf/1910.10900.pdf)
- [6-DOF Grasping for Target-driven Object Manipulation in Clutter](https://arxiv.org/pdf/1912.03628.pdf)
- [Graspness Discovery in Clutters for Fast and Accurate Grasp Detection](https://openaccess.thecvf.com/content/ICCV2021/papers/Wang_Graspness_Discovery_in_Clutters_for_Fast_and_Accurate_Grasp_Detection_ICCV_2021_paper.pdf)
- [Efficient and Accurate Candidate Generation for Grasp Pose Detection in SE(3)](https://arxiv.org/pdf/2204.01131.pdf)
- [UniDexGrasp: Universal Robotic Dexterous Graspingvia Learning Diverse Proposal Generation and Goal-Conditioned Policy](https://openaccess.thecvf.com/content/CVPR2023/papers/Xu_UniDexGrasp_Universal_Robotic_Dexterous_Grasping_via_Learning_Diverse_Proposal_Generation_CVPR_2023_paper.pdf)

### Reconstruction methods
- [Data-Efficient Learning for Sim-to-Real Robotic Grasping using Deep Point Cloud Prediction Networks](https://arxiv.org/pdf/1906.08989.pdf)
- [Robotic Grasping through Combined Image-Based Grasp Proposal and 3D Reconstruction](https://arxiv.org/pdf/2003.01649.pdf)
- [Amodal 3D Reconstruction for Robotic Manipulation via Stability and Connectivity](https://arxiv.org/pdf/2009.13146.pdf)
- [Volumetric Grasping Network: Real-time 6 DOF Grasp Detection in Clutter](https://arxiv.org/pdf/2101.01132.pdf)
- [GraspNeRF: Multiview-based 6-DoF Grasp Detection for Transparent and Specular Objects Using Generalizable NeRF](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10160842)

### Discriminative methods
- [Grasp Pose Detection in Point Clouds](https://arxiv.org/pdf/1706.09911.pdf)
- [PointNetGPD: Detecting Grasp Configurations from Point Sets](https://web.cs.ucla.edu/~xm/file/pointnetgpd_icra19.pdf)
- [Grasp Quality Evaluation Network for Surface-to-Surface Contacts in Point Clouds](https://ieeexplore.ieee.org/document/9216808)
- [Collision-Aware Target-Driven Object Grasping in Constrained Environments](https://arxiv.org/pdf/2104.00776.pdf)
- [GPR: Grasp Pose Refinement Network for Cluttered Scenes](https://arxiv.org/pdf/2105.08502.pdf)
- [Simultaneous Semantic and Collision Learning for 6-DoF Grasp Pose Estimation](https://arxiv.org/pdf/2108.02425.pdf)
- [DefGraspNets: Grasp Planning on 3D Fields with Graph Neural Nets](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10160986)
- [GraspMixer: Hybrid of Contact Surface Sampling and Grasp Feature Mixing for Grasp Synthesis](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10843724)

### Regression methods
- [S4G: Amodal Single-view Single-Shot SE(3) Grasp Detection in Cluttered Scenes](https://arxiv.org/pdf/1910.14218.pdf)
- [Contact-GraspNet: Efficient 6-DoF Grasp Generation in Cluttered Scenes](https://arxiv.org/pdf/2103.14127.pdf)
- [Synergies Between Affordance and Geometry: 6-DoF Grasp Detection via Implicit Representations](https://arxiv.org/pdf/2104.01542.pdf)
- [GraspNet-1Billion: A Large-Scale Benchmark for General Object Grasping](https://openaccess.thecvf.com/content_CVPR_2020/papers/Fang_GraspNet-1Billion_A_Large-Scale_Benchmark_for_General_Object_Grasping_CVPR_2020_paper.pdf)
- [RGB Matters: Learning 7-DoF Grasp Poses on Monocular RGBD Images](https://arxiv.org/pdf/2103.02184.pdf)
- [REGNet: REgion-based Grasp Network for End-to-end Grasp Detection in Point Clouds](https://arxiv.org/pdf/2002.12647.pdf)
- [Hybrid Physical Metric For 6-DoF Grasp Pose Detection](https://arxiv.org/pdf/2206.11141.pdf)

### Neural Representation methods

Researchers have recently started to investigate methods utilizing Neural Radiance Field (NeRF) and Implicit Neural Representation (INR). We separate these approaches as a new category of methods since they more focus on novel representation and sampling for robotic grasping. 

- [Neural Descriptor Fields: SE(3)-Equivariant Object Representations for Manipulation](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9812146)
- [NeuralGrasps: Learning Implicit Representations for Grasps of Multiple Robotic Hands](https://proceedings.mlr.press/v205/khargonkar23a/khargonkar23a.pdf) 
- [Neural Grasp Distance Fields for Robot Manipulation](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10160217)

### Survey (GPD)
- [Robotic Grasping from Classical to Modern: A Survey](https://arxiv.org/pdf/2202.03631.pdf)
- [Deep Learning Approaches to Grasp Synthesis: A Review](https://arxiv.org/pdf/2207.02556.pdf)
- [Vision‑based robotic grasping from object localization, object pose estimation to grasp estimation for parallel grippers: a review](https://link.springer.com/content/pdf/10.1007/s10462-020-09888-5.pdf)

### Datasets (GPD)
- [GraspNet](https://graspnet.net/index.html)

## Grasp Quality Metrics

### Combined metrics
- [Characterisation of Grasp Quality Metrics](https://link.springer.com/article/10.1007/s10846-017-0562-1)
- [Grasp success prediction with quality metrics](https://arxiv.org/pdf/1809.03276v1.pdf)

## ToDo Lists
| Categorization of approaches in *6D Grasp Pose Detection* | ![Progress](https://geps.dev/progress/100) |
| --- | --- |
