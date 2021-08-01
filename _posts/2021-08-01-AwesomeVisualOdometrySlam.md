---
title: Awesome Visual Odometry Slam
date: 2021-08-07
categories: [Research]
tags: [research, awesome, visual, odometry, slam]
pin: true
toc: true
toc_sticky: true
description: 
---

## Table of Contents

## Learning

### Courses
### Books
- Multiple View Geometry in Computer Vision, Hartley and Zisserman, 2004
- Computer Vision: Algorithms and Applications, Szeliski, 2010

## Paper
### Survey, Review
- Visual Odometry [Tutorial], Scaramuzza and Fraundorfer, RAM 2011
- 15 Years of Visual SLAM, Davison, ICCV 2015 Workshop
- Past, present, and future of simultaneous localization and mapping: Toward the robust-perception age, Cadena et al., T-RO 2016
- Event-based Vision: A Survey, Gallego et al., arXiv 2019
- A Survey on Deep Learning for Localization and Mapping: Towards the Age of Spatial Machine Intelligence, Chen et al., arXiv 2020.

### Difference between VO(Visual Odometry) and SLAM(Simultaneous Localization and Mapping)
- [An Overview to Visual Odometry and Visual SLAM: Applications to Mobile Robotics](https://link.springer.com/article/10.1007/s40903-015-0032-7)

### VO
#### Learning
|Year|Title|Name|Doc|Code|Website|
|:-:|:-:|:-:|:-:|:-:|:-:|
|2008|Make3D: Learning 3D Scene Structure from a Single Still Image|Make3D|[Pdf][Paper20081]|[Code][Code20081]|[Webpage][Webpage20081]|
|2011|StereoScan: Dense 3d reconstruction in real-time|VISO2|[Pdf][Paper20111]|[Code][Code20111]|[Webpage][Webpage20111]|
|2015|ORB-SLAM: A Versatile and Accurate Monocular SLAM System|ORB-SLAM2|[Pdf][Paper20151]|-|-|
|2015|Depth and Surface Normal Estimation From Monocular Images Using Regression on Deep Features and Hierarchical CRFs|-|[Pdf][Paper20152]|-|-|
|2016|Unsupervised CNN for Single View Depth Estimation: Geometry to the Rescue|-|[Pdf][Paper20161]|[Code][Code20161]|-|
|2017|Unsupervised Learning of Depth and Ego-Motion From Video|SfM-Learner|[Pdf][Paper20171]|[Code][Code20171]|-|
|2017|Multi-Scale Continuous CRFs as Sequential Deep networks for Monocular Depth Estimation|MS-CRF|[Pdf][Paper20172]|[Code][Code20172]|-|
|2018|Unsupervised Learning of Depth and Ego-Motion From Monocular Video Using 3D Geometric Constraints|Vid2Depth|[Pdf][Paper20181]|[Code][Code20181]|[Webpage][Webpage20181]|
|2018|GeoNet: Unsupervised Learning of Dense Depth, Optical Flow and Camera Pose|GeoNet|[Pdf][Paper20182]|[Code][Code20182]|-|
|2018| Unsupervised Learning of Monocular Depth Estimation and Visual Odometry With Deep Feature Reconstruction|Depth-VO-Feat|[Pdf][Paper20183]|[Code][Code20183]|-|
|2018|Unsupervised Learning of Depth and Ego-Motion From Monocular Video Using 3D Geometric Constraints|-|[Pdf][Paper20183]|-|-|
|2018|Deep Ordinal Regression Network for Monocular Depth Estimation|DORN|[Pdf][Paper20184]|[Code][Code20184]|-|
|2019|Sequential Adversarial Learning for Self-Supervised Deep Visual Odometry|-|[Pdf][Paper20191]|-|-|
|2019|Digging Into Self-Supervised Monocular Depth Estimation|Monodepth2|[Pdf][Paper20192]|[Code][Code20192]|-|
|2019|Unsupervised Scale-consistent Depth and Ego-motion Learning from Monocular Video|SC-SfMLearner|[Pdf][Paper20193]|-|-|
|2021|Unsupervised Scale-consistent Depth Learning from Video|SC-SfMLearner|[Pdf][Paper20211]|[Code][Code20211]|[Webpage][Webpage20211]|
|2019|Moving Indoor: Unsupervised Video Depth Learning in Challenging Environments|-|[Pdf][Paper20194]|-|-|
|2019|Competitive Collaboration: Joint Unsupervised Learning of Depth, Camera Motion, Optical Flow and Motion Segmentation|-|[Pdf][Paper20195]|[Code][Code20195]|-|
|2020|Visual Odometry Revisited: What Should Be Learnt?|DF-VO|[Pdf][Paper20205]|[Code][Code20205]|-|
|2021|DF-VO: What Should Be Learnt for Visual Odometry?|DF-VO|[Pdf][Paper20212]|[Code][Code20212]|-|
|2020|D3VO: Deep Depth, Deep Pose and Deep Uncertainty for Monocular Visual Odometry|D3VO|[Pdf][Paper20202]|-|-|
|2020|Towards Better Generalization: Joint Depth-Pose Learning without PoseNet|TrianFlow|[Pdf][Paper20203]|[Code][Code20203]|-|
|2020|P2Net: Patch-Match and Plane-Regularization for Unsupervised Indoor Depth Estimation|-|[Pdf][Paper20204]|-|-|

[Paper20081]: https://ieeexplore.ieee.org/abstract/document/4531745
[Code20081]: https://make3d.cs.cornell.edu/code.html
[Webpage20081]: http://make3d.cs.cornell.edu/

[Paper20111]: https://ieeexplore.ieee.org/abstract/document/5940405
[Code20111]: https://github.com/srv/viso2
[Webpage20111]: https://wiki.ros.org/viso2

[Paper20151]: https://ieeexplore.ieee.org/abstract/document/7219438

[Paper20152]: https://openaccess.thecvf.com/content_cvpr_2015/html/Li_Depth_and_Surface_2015_CVPR_paper.html

[Paper20161]: https://link.springer.com/chapter/10.1007/978-3-319-46484-8_45
[Code20161]: https://github.com/Ravi-Garg/Unsupervised_Depth_Estimation

[Paper20171]: https://openaccess.thecvf.com/content_cvpr_2017/html/Zhou_Unsupervised_Learning_of_CVPR_2017_paper.html
[Code20171]: https://github.com/tinghuiz/SfMLearner

[Paper20172]: https://openaccess.thecvf.com/content_cvpr_2017/html/Xu_Multi-Scale_Continuous_CRFs_CVPR_2017_paper.html
[Code20172]: https://github.com/danxuhk/ContinuousCRF-CNN 

[Paper20181]: https://papers.nips.cc/paper/8299-unsupervised-scale-consistent-depth-and-ego-motion-learning-from-monocular-video.pdf
[Code20181]: https://sites.google.com/view/vid2depth/home#h.p_2UNFmTrz01jq
[Webpage20181]: https://sites.google.com/view/vid2depth/home

[Paper20182]: https://openaccess.thecvf.com/content_cvpr_2018/html/Yin_GeoNet_Unsupervised_Learning_CVPR_2018_paper.html
[Code20182]: https://github.com/yzcjtr/GeoNet

[Paper20183]: https://openaccess.thecvf.com/content_cvpr_2018/html/Zhan_Unsupervised_Learning_of_CVPR_2018_paper.html
[Code20183]: https://github.com/Huangying-Zhan/Depth-VO-Feat

[Paper20183]: https://openaccess.thecvf.com/content_cvpr_2018/html/Mahjourian_Unsupervised_Learning_of_CVPR_2018_paper.html

[Paper20184]: https://openaccess.thecvf.com/content_cvpr_2018/html/Fu_Deep_Ordinal_Regression_CVPR_2018_paper.html
[Code20184]: https://github.com/hufu6371/DORN

[Paper20191]: https://openaccess.thecvf.com/content_ICCV_2019/html/Li_Sequential_Adversarial_Learning_for_Self-Supervised_Deep_Visual_Odometry_ICCV_2019_paper.html

[Paper20192]: https://openaccess.thecvf.com/content_ICCV_2019/html/Godard_Digging_Into_Self-Supervised_Monocular_Depth_Estimation_ICCV_2019_paper.html
[Code20192]: www.github.com/nianticlabs/monodepth2

[Paper20193]: https://proceedings.neurips.cc/paper/2019/file/6364d3f0f495b6ab9dcf8d3b5c6e0b01-Paper.pdf

[Paper20211]: https://jwbian.net/Papers/SC_Depth_IJCV_21.pdf
[Code20211]: https://github.com/JiawangBian/SC-SfMLearner-Release
[Webpage20211]: https://jwbian.net/sc-sfmlearner

[Paper20194]: https://openaccess.thecvf.com/content_ICCV_2019/html/Zhou_Moving_Indoor_Unsupervised_Video_Depth_Learning_in_Challenging_Environments_ICCV_2019_paper.html

[Paper20195]: https://openaccess.thecvf.com/content_CVPR_2019/html/Ranjan_Competitive_Collaboration_Joint_Unsupervised_Learning_of_Depth_Camera_Motion_Optical_CVPR_2019_paper.html
[Code20195]: https://github.com/anuragranj/cc

[Paper20205]: https://ieeexplore.ieee.org/abstract/document/9197374
[Paper20212]: https://arxiv.org/abs/2103.00933
[Code20205]: https://github.com/Huangying-Zhan/DF-VO
[Code20212]: https://github.com/Huangying-Zhan/DF-VO

[Paper20202]: https://openaccess.thecvf.com/content_CVPR_2020/html/Yang_D3VO_Deep_Depth_Deep_Pose_and_Deep_Uncertainty_for_Monocular_CVPR_2020_paper.html

[Paper20203]: https://openaccess.thecvf.com/content_CVPR_2020/html/Zhao_Towards_Better_Generalization_Joint_Depth-Pose_Learning_Without_PoseNet_CVPR_2020_paper.html
[Code20203]: https://github.com/B1ueber2y/TrianFlow

[Paper20204]: https://link.springer.com/content/pdf/10.1007/978-3-030-58586-0_13.pdf

 
||||
[Paper]: 
[Code]: 
[Webpage]: 

||||
[Paper]: 
[Code]: 
[Webpage]: 

- In defense of the eight-point algorithm, Hartley, TPAMI 1997

- Real-time simultaneous localisation and mapping with a single camera, Davison, ICCV 2003

- Visual Odometry, Nistér et al., CVPR 2004
- SIFT: Distinctive Image Features from Scale-Invariant Keypoints, Lowe, IJCV 2004
- An efficient solution to the five-point relative pose problem, Nistér, TPAMI 2004

- SURF: Speeded Up Robust Features, Bay et al., ECCV 2006

- MonoSLAM: Real-Time Single Camera SLAM, Davison et al., TPAMI 2007 | code
- Parallel tracking and mapping for small AR workspaces, Klein and Murray, ISMAR 2007 | code
- Georg Klein and David Murray, "Parallel Tracking and Mapping for Small AR Workspaces", Proc. ISMAR 2007 

- Real-time stereo visual odometry for autonomous ground vehicles, Howard, IROS 2008
- Georg Klein and David Murray, "Improving the Agility of Keyframe-based SLAM", Proc. ECCV 2008

- Faster and Better: A Machine Learning Approach to Corner Detection, Rosten et al., TPAMI 2010.

- DTAM: Dense tracking and mapping in real-time, Newcombe et al., ICCV 2011
- Real-Time Visual Odometry from Dense RGB-D Images, Steinbruecker et al. ICCV 2011 | code
- KinectFusion: Real-time dense surface mapping and tracking, Newcombe et al., ISMAR 2011
- ORB: An efficient alternative to SIFT or SURF, Rublee et al., ICCV 2011

- Dense Visual SLAM for RGB-D Cameras (C. Kerl, J. Sturm, D. Cremers), In Proc. of the Int. Conf. on Intelligent Robot Systems (IROS), 2013. 
- Robust Odometry Estimation for RGB-D Cameras, Kerl et al. ICRA 2013 | code
- Online Global Loop Closure Detection for Large-Scale Multi-Session Graph-Based SLAM, 2014 Appearance-Based Loop Closure Detection for Online Large-Scale and Long-Term Operation, 2013 

- SVO: Fast semi-direct monocular visual odometry, Forster et al., ICRA 2014 | code
- LSD-SLAM: Large-Scale Direct Monocular SLAM, Engel et al., ECCV 2014 | code
- FLANN: Scalable Nearest Neighbor Algorithms for High Dimensional Data, Muja and Lowe, TPAMI 2014
- Real-time Large Scale Dense RGB-D SLAM with Volumetric Fusion, T. Whelan, M. Kaess, H. Johannsson, M.F. Fallon, J. J. Leonard and J.B. McDonald, IJRR '14

- Dynamicfusion: Reconstruction and tracking of non-rigid scenes in real-time, Newcombe et al., CVPR 2015
- ElasticFusion: Dense SLAM without a pose graph, Whelan et al. RSS 2015
- Kahler, O. and Prisacariu, V.~A. and Ren, C.~Y. and Sun, X. and Torr, P.~H.~S and Murray, D.~W. Very High Frame Rate Volumetric Integration of Depth Images on Mobile Device. IEEE Transactions on Visualization and Computer Graphics (Proceedings International Symposium on Mixed and Augmented Reality 2015
- PoseNet: A Convolutional Network for Real-Time 6-DOF Camera Relocalization, Kendall et al., ICCV 2015

- Real-time 3D reconstruction and 6-DoF tracking with an event camera, Kim et al., ECCV 2016
- EVO: A Geometric Approach to Event-Based 6-DOF Parallel Tracking and Mapping in Real Time, Rebecq et al., RA-L 2016
- Simultaneous Optical Flow and Intensity Estimation From an Event Camera, Bardow et al., CVPR 2016
- Deep Image Homography Estimation, DeTone et al., arXiv 2016

- ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras, Mur-Artal et al., T-RO 2017 
- DSO: Direct Sparse Odometry, Engel et al., TPAMI 2017 
- DeepVO: Towards End-to-End Visual Odometry with Deep Recurrent Convolutional Neural Networks
- UnDeepVO: Monocular Visual Odometry through Unsupervised Deep Learning
- GMS: Grid-based Motion Statistics for Fast, Ultra-robust Feature Correspondence, Bian et al., CVPR 2017
- LF-Net: Learning Local Features from Images, Ono et al., NeurIPS 2017
- Martin Rünz and Lourdes Agapito. Co-Fusion: Real-time Segmentation, Tracking and Fusion of Multiple Objects. 2017 IEEE International Conference on Robotics and Automation (ICRA)
- Unsupervised Learning of Depth and Ego-Motion from Video, Zhou et al., CVPR 2017

- Unsupervised Learning of Monocular Depth Estimation and Visual Odometry with Deep Feature Reconstruction, Zhan et al., CVPR 2018
- CodeSLAM - Learning a Compact, Optimisable Representation for Dense Visual SLAM, Bloesch et al., CVPR 2018
- Deep Virtual Stereo Odometry: Leveraging Deep Depth Prediction for Monocular Direct Sparse Odometry, Yang et al., ECCV 2018
- DynaSLAM: Tracking, Mapping and Inpainting in Dynamic Scenes, Bescos et al., RA-L, 2018 
- Digging Into Self-Supervised Monocular Depth Estimation
- SuperPoint: Self-Supervised Interest Point Detection and Description, DeTone et al., CVPR 2018 Workshop
- Ultimate SLAM? Combining Events, Images, and IMU for Robust Visual SLAM in HDR and High-Speed Scenarios, Vidal, RA-L 2018

- OpenVSLAM: A Versatile Visual SLAM Framework, Sumikura et al., ACM MM 2019 | code
- GANVO: Unsupervised Deep Monocular Visual Odometry and Depth Estimation with Generative Adversarial Networks
- Pose Graph Optimization for Unsupervised Monocular Visual Odometry |
- R2D2: Repeatable and Reliable Detector and Descriptor, Revaud et al., NeurIPS 2019
- D2-Net: A Trainable CNN for Joint Description and Detection of Local Features, Dusmanu et al., CVPR 2019
- Deep Graphical Feature Learning for the Feature Matching Problem, Zhang and Lee, ICCV 2019

- Kimera: an Open-Source Library for Real-Time Metric-Semantic Localization and Mapping, Rosinol et al., ICRA 2020 
- DXSLAM: A Robust and Efficient Visual SLAM System with Deep Features, Li et al., IROS 2020 
- ORB-SLAM3: An Accurate Open-Source Library for Visual, Visual-Inertial and Multi-Map SLAM, Campos et al., arXiv 2020
- SuperGlue: Learning Feature Matching with Graph Neural Networks, Sarlin et al., CVPR 2020
- High-dimensional Convolutional Networks for Geometric Pattern Recognition, Choy et al., CVPR 2020

- Generalizing to the Open World: Deep Visual Odometry with Online Adaptation, Li et al., CVPR 2021
- Tight Integration of Feature-based Relocalization in Monocular Direct Visual Odometry, Gladkova et al., ICRA 2021
- Unsupervised Scale-consistent Depth Learning from Video, 2021
- LoFTR: Detector-Free Local Feature Matching with Transformers, Sun et al., CVPR 2021
- Combining Events and Frames using Recurrent Asynchronous Multimodal Networks for Monocular Depth Prediction, Gehrig et al., RA-L, 2021



## Project
- [An Invitation to 3D Vision: A Tutorial for Everyone](https://awesomeopensource.com/project/sunglok/3dv_tutorial)
- [LVI-SAM: Tightly-coupled Lidar-Visual-Inertial Odometry via Smoothing and Mapping](https://awesomeopensource.com/project/TixiaoShan/LVI-SAM)

## Dataset
- [nuScenes](https://www.nuscenes.org/)
- [KITTI](http://www.cvlibs.net/datasets/kitti/eval_odometry.php)
- [Waymo Open Dataset](https://waymo.com/open/)
- [Lyft Level 5 AV Dataset 2019](https://level-5.global/data/)
- [KAIST Urban Dataset](https://irap.kaist.ac.kr/dataset/)
- [TUM RGB-D](https://vision.in.tum.de/data/datasets/rgbd-dataset/download)
- [TUM MonoVO](https://vision.in.tum.de/data/datasets/mono-dataset)
- [TUM VI](https://vision.in.tum.de/data/datasets/visual-inertial-dataset)
- [UNI-Freiburg](https://lmb.informatik.uni-freiburg.de/resources/datasets/SceneFlowDatasets.en.html)
- [ADVIO](https://github.com/AaltoVision/ADVIO)
- [Oxford RobotCar Dataset](https://robotcar-dataset.robots.ox.ac.uk)
- [HRI (Honda Research Institute) Driving Datasets](https://usa.honda-ri.com/honda-driving-datasets)
- [Argoverse](https://www.argoverse.org/data.html#download-link)
- [EuRoC Dataset](https://projects.asl.ethz.ch/datasets/doku.php?id=kmavvisualinertialdatasets)
- [Malaga](https://www.mrpt.org/MalagaUrbanDataset)
- [ICL-NUIM](https://www.doc.ic.ac.uk/~ahanda/VaFRIC/iclnuim.html)
- Cityscapes
- NYUv2
