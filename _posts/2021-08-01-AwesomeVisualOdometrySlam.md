---
title: Awesome Visual Odometry Slam
date: 2021-08-07
categories: [Research]
tags: [research, awesome, visual, odometry, slam]
pin: true
toc: true
toc_sticky: true
description: List of Visual Odometry, SLAM Contents
---

## Learning

### Courses

### Books

- Multiple View Geometry in Computer Vision, Hartley and Zisserman, 2004
- Computer Vision: Algorithms and Applications, Szeliski, 2010

## Paper

### Survey, Review

- [Visual Odometry [Tutorial], Scaramuzza and Fraundorfer, RAM 2011](https://ieeexplore.ieee.org/abstract/document/6096039)
- [Visual Odometry : Part II: Matching, Robustness, Optimization, and Applications, Scaramuzza and Fraundorfer, RAM 2012](https://ieeexplore.ieee.org/abstract/document/6153423)
- [An Overview to Visual Odometry and Visual SLAM: Applications to Mobile Robotics, Yousif et al.,  Intell Ind Syst 2015](https://link.springer.com/article/10.1007/s40903-015-0032-7)
- [The Future of Real-Time SLAM: Sensors, Processors, Representations, and Algorithms, Davison, ICCV 2015 Workshop](https://wp.doc.ic.ac.uk/thefutureofslam/) / [15 Years of Visual SLAM, Davison, ICCV 2015 Workshop](http://wp.doc.ic.ac.uk/thefutureofslam/wp-content/uploads/sites/93/2015/12/slides_ajd.pdf)
- [Past, present, and future of simultaneous localization and mapping: Toward the robust-perception age, Cadena et al., T-RO 2016](https://ieeexplore.ieee.org/abstract/document/7747236)
- [Event-based Vision: A Survey, Gallego et al., arXiv 2019](https://arxiv.org/abs/1904.08405)
- [A Survey on Deep Learning for Localization and Mapping: Towards the Age of Spatial Machine Intelligence, Chen et al., arXiv 2020](https://arxiv.org/abs/2006.12567)



### VO/SLAM

#### Learning
#### Feature Tracking

|Year|Title|Name|Doc|Code|Website|
|:-:|:-:|:-:|:-:|:-:|:-:|
|2003|Real-time simultaneous localisation and mapping with a single camera|-|[Pdf][PaperRTSLAMSC]|-|-|
|2004|Visual Odometry|-|[Pdf][PaperVO]|-|-|
|2004|An efficient solution to the five-point relative pose problem|-|[Pdf][PaperESFPRPP]|-|-|
|2004|Distinctive Image Features from Scale-Invariant Keypoints|SIFT|[Pdf][PaperSIFT]|-|-|
|2006|Visual odometry for ground vehicle applications||[Pdf][PaperVOGVA]|-|-|
|2006|SURF: Speeded Up Robust Features|SURF|[Pdf][PaperSURF]|[Code][CodeSURF]|-|
|2006|Machine learning for high-speed corner detection|FAST|[Pdf][PaperFAST]|[Code][CodeFAST]|-|
|2010|Faster and Better: A Machine Learning Approach to Corner Detection|FAST-ER|[Pdf][PaperFAST_ER]|[Code][CodeFAST_ER]|-|
|2007|Parallel tracking and mapping for small AR workspaces|PTAM|[Pdf][PaperPTAM]|[Code][CodePTAM]|[Webpage][WebpagePTAM]|
|2007|MonoSLAM: Real-Time Single Camera SLAM|MonoSLAM|[Pdf][PaperMonoSLAM]|-|-|
|2008|Improving the Agility of Keyframe-based SLAM|-|[Pdf][PaperIAKBSLAM]|-|-|
|2008|Real-time stereo visual odometry for autonomous ground vehicles|-|[Pdf][PaperRTSVOAGV]|-|-|
|2008|Make3D: Learning 3D Scene Structure from a Single Still Image|Make3D|[Pdf][PaperMake3D]|[Code][CodeMake3D]|[Webpage][WebpageMake3D]|
|2011|ORB: An efficient alternative to SIFT or SURF|ORB|[Pdf][PaperORB]|-|-|
|2011|KinectFusion: Real-time dense surface mapping and tracking|KinectFusion|[Pdf][PaperKinectFusion]|-|-|
|2011|Real-Time Visual Odometry from Dense RGB-D Images|-|[Pdf][PaperRTVODRGBDI]|-|-|
|2011|DTAM: Dense tracking and mapping in real-time|DTAM|[Pdf][PaperDTAM]|-|-|
|2011|StereoScan: Dense 3d reconstruction in real-time|VISO2|[Pdf][PaperVISO2]|[Code][CodeVISO2]|[Webpage][WebpageVISO2]|
|2013|Online Global Loop Closure Detection for Large-Scale Multi-Session Graph-Based SLAM|-|[Pdf][PaperOGLCDLSMSGBSLAM]|-|-|
|2013|Robust Odometry Estimation for RGB-D Cameras||[Pdf][PaperROERGBDC]|-|-|
|2013|Dense Visual SLAM for RGB-D Cameras|-|[Pdf][PaperDVSLAMRGBDC]|-|-|
|2013|Semi-Dense Visual Odometry for a Monocular Camera|LSD-SLAM|[Pdf][PaperLSD_SLAM1]|[Code][CodeLSD_SLAM1]|[Webpage][WebpageLSD_SLAM1]|
|2014|LSD-SLAM: Large-Scale Direct Monocular SLAM|LSD-SLAM|[Pdf][PaperLSD_SLAM2]|[Code][CodeLSD_SLAM2]|[Webpage][WebpageLSD_SLAM2]|
|2014|Real-time Large Scale Dense RGB-D SLAM with Volumetric Fusion|-|[Pdf][PaperRTLSDRGBDSLAMVF]|-|-|
|2014|Scalable Nearest Neighbor Algorithms for High Dimensional Data|FLANN|[Pdf][PaperFLANN]|[Code][CodeFLANN]|-|
|2014|SVO: Fast semi-direct monocular visual odometry||[Pdf][PaperSVO]|[Code][CodeSVO]|[Webpage][WebpageSVO]|
|2015|Learning visual odometry with a convolutional network|-|[Pdf][PaperLVOCN]|-|-|
|2015|PoseNet: A Convolutional Network for Real-Time 6-DOF Camera Relocalization|PoseNet|[Pdf][PaperPoseNet]|[Code][CodePoseNet]|-|
|2015|Very High Frame Rate Volumetric Integration of Depth Images on Mobile Device|-|[Pdf][PaperVHFRVIDIMD]|-|-|
|2015|Dynamicfusion: Reconstruction and tracking of non-rigid scenes in real-time|Dynamicfusion|[Pdf][PaperDynamicfusion]|-|-|
|2015|ElasticFusion: Dense SLAM without a pose graph|ElasticFusion|[Pdf][PaperElasticFusion1]|[Code][CodeElasticFusion1]|-|
|2016|ElasticFusion: Real-time dense SLAM and light source estimation|ElasticFusion|[Pdf][PaperElasticFusion2]|[Code][CodeElasticFusion2]|-|
|2015|ORB-SLAM: A Versatile and Accurate Monocular SLAM System|ORB-SLAM|[Pdf][PaperORBSLAM]|[Code][CodeORBSLAM]|-|
|2017|ORB-SLAM2: an Open-Source SLAM System for Monocular, Stereo and RGB-D Cameras|ORB-SLAM2|[Pdf][PaperORBSLAM2]|[Code][CodeORBSLAM2]|-|
|2021|ORB-SLAM3: An Accurate Open-Source Library for Visual, Visual-Inertial and Multi-Map SLAM|ORB-SLAM3|[Pdf][PaperORBSLAM3]|[Code][CodeORBSLAM3]|-|
|2015|Depth and Surface Normal Estimation From Monocular Images Using Regression on Deep Features and Hierarchical CRFs|-|[Pdf][Paper20152]|-|-|
|2016|Unsupervised CNN for Single View Depth Estimation: Geometry to the Rescue|-|[Pdf][Paper20161]|[Code][Code20161]|-|
|2016|Real-time 3D reconstruction and 6-DoF tracking with an event camera|-|[Pdf][PaperRT3DR6DOFTEC]|-|-|
|2016|EVO: A Geometric Approach to Event-Based 6-DOF Parallel Tracking and Mapping in Real Time|EVO|[Pdf][PaperEVO]|[Code][CodeEVO]|-|
|2016|Simultaneous Optical Flow and Intensity Estimation From an Event Camera|-|[Pdf][PaperSOFIEEC]|-|-|
|2016|Deep Image Homography Estimation|-|[Pdf][PaperDIHE]|-|-|
|2017|DSO: Direct Sparse Odometry|DSO|[Pdf][PaperDSO]|[Code][CodeDSO]|-|
|2017|DeepVO: Towards End-to-End Visual Odometry with Deep Recurrent Convolutional Neural Networks|DeepVO|[Pdf][PaperDeepVO]|-|-|
|2017|UnDeepVO: Monocular Visual Odometry through Unsupervised Deep Learning|UnDeepVO|[Pdf][PaperUnDeepVO]|-|-|
|2017|GMS: Grid-based Motion Statistics for Fast, Ultra-robust Feature Correspondence||[Pdf][PaperGMS]|[Code][CodeGMS]|-|
|2017|LF-Net: Learning Local Features from Images|LF-Net|[Pdf][PaperLF_Net]|-|-|
|2017|Co-Fusion: Real-time Segmentation, Tracking and Fusion of Multiple Objects|Co-Fusion|[Pdf][PaperCo_Fusion]|[Code][CodeCo_Fusion]|-|
|2017|Unsupervised Learning of Depth and Ego-Motion from Video||[Pdf][PaperULDEMV]|-|-|
|2017|Unsupervised Learning of Depth and Ego-Motion From Video|SfM-Learner|[Pdf][Paper20171]|[Code][Code20171]|-|
|2017|Multi-Scale Continuous CRFs as Sequential Deep networks for Monocular Depth Estimation|MS-CRF|[Pdf][Paper20172]|[Code][Code20172]|-|
|2018|Unsupervised Learning of Depth and Ego-Motion From Monocular Video Using 3D Geometric Constraints|Vid2Depth|[Pdf][Paper20181]|[Code][Code20181]|[Webpage][Webpage20181]|
|2018|GeoNet: Unsupervised Learning of Dense Depth, Optical Flow and Camera Pose|GeoNet|[Pdf][Paper20182]|[Code][Code20182]|-|
|2018|Unsupervised Learning of Monocular Depth Estimation and Visual Odometry With Deep Feature Reconstruction|Depth-VO-Feat|[Pdf][Paper20183]|[Code][Code20183]|-|
|2018|Unsupervised Learning of Depth and Ego-Motion From Monocular Video Using 3D Geometric Constraints|-|[Pdf][Paper20183]|-|-|
|2018|CodeSLAM - Learning a Compact, Optimisable Representation for Dense Visual SLAM|CodeSLAM|[Pdf][PaperCodeSLAM]|-|-|
|2018|Deep Virtual Stereo Odometry: Leveraging Deep Depth Prediction for Monocular Direct Sparse Odometry|-|[Pdf][PaperDVSO]|-|-|
|2018|DynaSLAM: Tracking, Mapping and Inpainting in Dynamic Scenes|DynaSLAM|[Pdf][PaperDynaSLAM]|[Code][CodeDynaSLAM]|[Webpage][WebpageDynaSLAM]|
|2018|Digging Into Self-Supervised Monocular Depth Estimation|-|[Pdf][PaperDSSMDE]|-|-|
|2018|SuperPoint: Self-Supervised Interest Point Detection and Description|SuperPoint|[Pdf][PaperSuperPoint]|[Code][CodeSuperPoint]|-|
|2018|Ultimate SLAM? Combining Events, Images, and IMU for Robust Visual SLAM in HDR and High-Speed Scenarios|-|[Pdf][PaperUSLAMCEIIRVSLAMHDRHSS]|-|-|
|2018|Deep Ordinal Regression Network for Monocular Depth Estimation|DORN|[Pdf][Paper20184]|[Code][Code20184]|-|
|2019|Sequential Adversarial Learning for Self-Supervised Deep Visual Odometry|-|[Pdf][Paper20191]|-|-|
|2019|OpenVSLAM: A Versatile Visual SLAM Framework|OpenVSLAM|[Pdf][PaperOpenVSLAM]|-|-|
|2019|GANVO: Unsupervised Deep Monocular Visual Odometry and Depth Estimation with Generative Adversarial Networks|GANVO|[Pdf][PaperGANVO]|-|-|
|2019|Pose Graph Optimization for Unsupervised Monocular Visual Odometry|-|[Pdf][PaperPGOUMVO]|-|-|
|2019|R2D2: Repeatable and Reliable Detector and Descriptor|R2D2|[Pdf][PaperR2D2]|-|-|
|2019|D2-Net: A Trainable CNN for Joint Description and Detection of Local Features|D2-Net|[Pdf][PaperD2-Net]|[Code][CodeD2-Net]|[Webpage][WebpageD2-Net]|
|2019|Deep Graphical Feature Learning for the Feature Matching Problem|-|[Pdf][PaperDGFLFMP]|-|-|
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
|2020|Kimera: an Open-Source Library for Real-Time Metric-Semantic Localization and Mapping|Kimera|[Pdf][PaperKimera]|[Code][CodeKimera]|-|
|2020|DXSLAM: A Robust and Efficient Visual SLAM System with Deep Features|DXSLAM|[Pdf][PaperDXSLAM]|[Code][CodeDXSLAM]|-|
|2020|SuperGlue: Learning Feature Matching with Graph Neural Networks|SuperGlue|[Pdf][PaperSuperGlue]|[Code][CodeSuperGlue]|[Webpage][WebpageSuperGlue]|
|2020|High-dimensional Convolutional Networks for Geometric Pattern Recognition|-|[Pdf][PaperHighDimConvNets]|-|[Webpage][WebpageHighDimConvNets]|
|2021|Generalizing to the Open World: Deep Visual Odometry with Online Adaptation|-|[Pdf][PaperGOWDVOOA]|-|-|
|2021|Tight Integration of Feature-based Relocalization in Monocular Direct Visual Odometry|-|[Pdf][PaperTIFBRMDVO]|-|-|
|2021|LoFTR: Detector-Free Local Feature Matching with Transformers|LoFTR|[Pdf][PaperLoFTR]|[Code][CodeLoFTR]|[Webpage][WebpageLoFTR]|
|2021|Combining Events and Frames using Recurrent Asynchronous Multimodal Networks for Monocular Depth Prediction|-|[Pdf][PaperCEFURAMNMDP]|[Code][CodeCEFURAMNMDP]|[Webpage][WebpageCEFURAMNMDP]|


***

[PaperDSO]: https://ieeexplore.ieee.org/abstract/document/7898369
[CodeDSO]: https://github.com/JakobEngel/dso
[PaperDeepVO]: https://ieeexplore.ieee.org/abstract/document/7989236
[PaperUnDeepVO]: https://ieeexplore.ieee.org/abstract/document/8461251
[PaperGMS]: https://openaccess.thecvf.com/content_cvpr_2017/html/Bian_GMS_Grid-based_Motion_CVPR_2017_paper.html
[CodeGMS]: https://github.com/JiawangBian/GMS-Feature-Matcher
[PaperLF_Net]: https://arxiv.org/abs/1805.09662
[PaperCo_Fusion]: https://ieeexplore.ieee.org/abstract/document/7989518
[CodeCo_Fusion]: https://github.com/martinruenz/co-fusion
[PaperULDEMV]: https://openaccess.thecvf.com/content_cvpr_2017/html/Zhou_Unsupervised_Learning_of_CVPR_2017_paper.html
[PaperRTSLAMSC]: https://ieeexplore.ieee.org/abstract/document/1238654
[PaperVO]: https://ieeexplore.ieee.org/abstract/document/1315094
[PaperESFPRPP]: https://ieeexplore.ieee.org/abstract/document/1288525/
[PaperSIFT]: https://link.springer.com/article/10.1023/B:VISI.0000029664.99615.94
[PaperVOGVA]: https://onlinelibrary.wiley.com/doi/abs/10.1002/rob.20103
[PaperSURF]: https://www.sciencedirect.com/science/article/pii/S1077314207001555
[CodeSURF]: https://github.com/herbertbay/SURF
[PaperPTAM]: https://ieeexplore.ieee.org/abstract/document/4538852
[CodePTAM]: https://github.com/t-thanh/PTAM-linux-cv2.3
[WebpagePTAM]: https://www.robots.ox.ac.uk/~gk/PTAM/
[PaperMonoSLAM]: https://ieeexplore.ieee.org/abstract/document/4160954
[PaperIAKBSLAM]: https://link.springer.com/chapter/10.1007/978-3-540-88688-4_59#enumeration
[PaperRTSVOAGV]: https://ieeexplore.ieee.org/abstract/document/4651147
[PaperFAST]: https://link.springer.com/chapter/10.1007/11744023_34
[CodeFAST]: https://github.com/edrosten/fast-C-src
[PaperFAST_ER]: https://ieeexplore.ieee.org/abstract/document/4674368
[CodeFAST_ER]: https://github.com/edrosten/fast-er
[PaperORB]: https://ieeexplore.ieee.org/abstract/document/6126544
[PaperKinectFusion]: https://ieeexplore.ieee.org/abstract/document/6162880
[PaperRTVODRGBDI]: https://ieeexplore.ieee.org/abstract/document/6130321
[PaperDTAM]: https://ieeexplore.ieee.org/abstract/document/6126513
[PaperOGLCDLSMSGBSLAM]: https://ieeexplore.ieee.org/abstract/document/6942926
[PaperROERGBDC]: https://ieeexplore.ieee.org/abstract/document/6631104
[PaperDVSLAMRGBDC]: https://ieeexplore.ieee.org/abstract/document/6696650
[PaperRTLSDRGBDSLAMVF]: https://journals.sagepub.com/doi/abs/10.1177/0278364914551008
[PaperLSD_SLAM1]: https://openaccess.thecvf.com/content_iccv_2013/html/Engel_Semi-dense_Visual_Odometry_2013_ICCV_paper.html
[CodeLSD_SLAM1]: https://github.com/tum-vision/lsd_slam
[WebpageLSD_SLAM1]: https://vision.in.tum.de/research/vslam/lsdslam?redirect=1
[PaperLSD_SLAM2]: https://link.springer.com/chapter/10.1007/978-3-319-10605-2_54
[CodeLSD_SLAM2]: https://github.com/tum-vision/lsd_slam
[WebpageLSD_SLAM2]: https://vision.in.tum.de/research/vslam/lsdslam?redirect=1
[PaperFLANN]: https://ieeexplore.ieee.org/abstract/document/6809191
[CodeFLANN]: https://github.com/flann-lib/flann
[PaperSVO]: https://ieeexplore.ieee.org/abstract/document/6906584
[CodeSVO]: https://github.com/uzh-rpg/rpg_svo
[WebpageSVO]: http://uzh-rpg.github.io/rpg_svo/doc/namespaces.html
[PaperLVOCN]: https://www.scitepress.org/papers/2015/52993/52993.pdf
[PaperPoseNet]: https://openaccess.thecvf.com/content_iccv_2015/html/Kendall_PoseNet_A_Convolutional_ICCV_2015_paper.html
[CodePoseNet]: https://github.com/alexgkendall/caffe-posenet
[PaperVHFRVIDIMD]: https://ieeexplore.ieee.org/abstract/document/7165673
[PaperElasticFusion1]: https://spiral.imperial.ac.uk/bitstream/10044/1/23438/2/whelan2015rss.pdf
[CodeElasticFusion1]: https://github.com/mp3guy/ElasticFusion
[PaperElasticFusion2]: https://journals.sagepub.com/doi/abs/10.1177/0278364916669237
[CodeElasticFusion2]: https://github.com/mp3guy/ElasticFusion
[PaperDynamicfusion]: https://www.cv-foundation.org/openaccess/content_cvpr_2015/html/Newcombe_DynamicFusion_Reconstruction_and_2015_CVPR_paper.html
[PaperRT3DR6DOFTEC]: https://link.springer.com/chapter/10.1007/978-3-319-46466-4_21
[PaperEVO]: https://ieeexplore.ieee.org/abstract/document/7797445
[CodeEVO]: https://github.com/uzh-rpg/rpg_dvs_evo_open
[PaperSOFIEEC]: https://openaccess.thecvf.com/content_cvpr_2016/html/Bardow_Simultaneous_Optical_Flow_CVPR_2016_paper.html
[PaperDIHE]: https://arxiv.org/abs/1606.03798
[PaperCodeSLAM]: https://openaccess.thecvf.com/content_cvpr_2018/html/Bloesch_CodeSLAM_--_Learning_CVPR_2018_paper.html
[PaperDVSO]: https://openaccess.thecvf.com/content_ECCV_2018/html/Nan_Yang_Deep_Virtual_Stereo_ECCV_2018_paper.html
[PaperDynaSLAM]: https://ieeexplore.ieee.org/abstract/document/8421015
[CodeDynaSLAM]: https://github.com/BertaBescos/DynaSLAM
[WebpageDynaSLAM]: https://bertabescos.github.io/DynaSLAM/
[PaperDSSMDE]: https://openaccess.thecvf.com/content_ICCV_2019/html/Godard_Digging_Into_Self-Supervised_Monocular_Depth_Estimation_ICCV_2019_paper.html
[PaperSuperPoint]: https://openaccess.thecvf.com/content_cvpr_2018_workshops/w9/html/DeTone_SuperPoint_Self-Supervised_Interest_CVPR_2018_paper.html
[CodeSuperPoint]: https://github.com/magicleap/SuperPointPretrainedNetwork
[PaperUSLAMCEIIRVSLAMHDRHSS]: https://ieeexplore.ieee.org/abstract/document/8258997
[PaperOpenVSLAM]: https://dl.acm.org/doi/abs/10.1145/3343031.3350539
[PaperGANVO]: https://ieeexplore.ieee.org/abstract/document/8793512
[PaperPGOUMVO]: https://ieeexplore.ieee.org/abstract/document/8793706
[PaperR2D2]: https://arxiv.org/abs/1906.06195
[PaperD2-Net]: https://openaccess.thecvf.com/content_CVPR_2019/html/Dusmanu_D2-Net_A_Trainable_CNN_for_Joint_Description_and_Detection_of_CVPR_2019_paper.html
[CodeD2-Net]: https://github.com/mihaidusmanu/d2-net
[WebpageD2-Net]: https://dsmn.ml/publications/d2-net.html
[PaperDGFLFMP]: https://openaccess.thecvf.com/content_ICCV_2019/html/Zhang_Deep_Graphical_Feature_Learning_for_the_Feature_Matching_Problem_ICCV_2019_paper.html
[PaperKimera]: https://ieeexplore.ieee.org/abstract/document/9196885
[CodeKimera]: https://github.com/MIT-SPARK/Kimera
[PaperDXSLAM]: https://ieeexplore.ieee.org/abstract/document/9340907
[CodeDXSLAM]: https://github.com/ivipsourcecode/dxslam
[PaperSuperGlue]: https://openaccess.thecvf.com/content_CVPR_2020/html/Sarlin_SuperGlue_Learning_Feature_Matching_With_Graph_Neural_Networks_CVPR_2020_paper.html
[CodeSuperGlue]: https://github.com/magicleap/SuperGluePretrainedNetwork
[WebpageSuperGlue]: https://psarlin.com/superglue/
[PaperHighDimConvNets]: https://openaccess.thecvf.com/content_CVPR_2020/html/Choy_High-Dimensional_Convolutional_Networks_for_Geometric_Pattern_Recognition_CVPR_2020_paper.html
[WebpageHighDimConvNets]: https://chrischoy.github.io/publication/highdimconvnet/
[PaperGOWDVOOA]: https://openaccess.thecvf.com/content/CVPR2021/html/Li_Generalizing_to_the_Open_World_Deep_Visual_Odometry_With_Online_CVPR_2021_paper.html
[PaperTIFBRMDVO]: https://arxiv.org/abs/2102.01191
[PaperLoFTR]: https://openaccess.thecvf.com/content/CVPR2021/html/Sun_LoFTR_Detector-Free_Local_Feature_Matching_With_Transformers_CVPR_2021_paper.html
[CodeLoFTR]: https://github.com/zju3dv/LoFTR
[WebpageLoFTR]: https://zju3dv.github.io/loftr/
[PaperCEFURAMNMDP]: https://ieeexplore.ieee.org/abstract/document/9359329
[CodeCEFURAMNMDP]: https://github.com/uzh-rpg/rpg_ramnet
[WebpageCEFURAMNMDP]: http://rpg.ifi.uzh.ch/RAMNet.html

[PaperMake3D]: https://ieeexplore.ieee.org/abstract/document/4531745
[CodeMake3D]: https://make3d.cs.cornell.edu/code.html
[WebpageMake3D]: http://make3d.cs.cornell.edu/

[PaperVISO2]: https://ieeexplore.ieee.org/abstract/document/5940405
[CodeVISO2]: https://github.com/srv/viso2
[WebpageVISO2]: https://wiki.ros.org/viso2

[PaperORBSLAM]: https://ieeexplore.ieee.org/abstract/document/7219438
[CodeORBSLAM]: https://github.com/raulmur/ORB_SLAM

[PaperORBSLAM2]: https://ieeexplore.ieee.org/abstract/document/7946260
[CodeORBSLAM2]: https://github.com/raulmur/ORB_SLAM2

[PaperORBSLAM3]: https://ieeexplore.ieee.org/abstract/document/9440682
[CodeORBSLAM3]: https://github.com/UZ-SLAMLab/ORB_SLAM3

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

## Project

- [An Invitation to 3D Vision: A Tutorial for Everyone](https://awesomeopensource.com/project/sunglok/3dv_tutorial)
- [LVI-SAM: Tightly-coupled Lidar-Visual-Inertial Odometry via Smoothing and Mapping](https://awesomeopensource.com/project/TixiaoShan/LVI-SAM)

## Dataset
|Name|Website|
|:-:|:-:|
|nuScenes|[Site][DatasetWebsitenuscenes]|
|KITTI|[Site][DatasetWebsitekitti]|
|Waymo Open Dataset|[Site][DatasetWebsitewaymo]|
|Lyft Level 5 AV Dataset 2019|[Site][DatasetWebsiteLyft]|
|KAIST Urban Dataset|[Site][DatasetWebsiteKAIST]|
|TUM RGB-D|[Site][DatasetWebsiteTUM_RGB_D]|
|TUM MonoVO|[Site][DatasetWebsiteTUM_MonoVO]|
|TUM VI|[Site][DatasetWebsiteTUM_VI]|
|UNI-Freiburg|[Site][DatasetWebsiteUNI_Freiburg]|
|ADVIO|[Site][DatasetWebsiteADVIO]|
|Oxford RobotCar Dataset|[Site][DatasetWebsiteOxford]|
|HRI (Honda Research Institute) Driving Datasets|[Site][DatasetWebsiteHRI]|
|Argoverse|[Site][DatasetWebsiteArgoverse]|
|EuRoC Dataset|[Site][DatasetWebsiteEuRoC]|
|Malaga|[Site][DatasetWebsiteMalaga]|
|ICL-NUIM|[Site][DatasetWebsiteICL_NUIM]|
|Cityscapes|[Site][DatasetWebsiteCityscapes]|
|NYUv2|[Site][DatasetWebsiteNYUv2]|


[DatasetWebsitenuscenes]: https://www.nuscenes.org/

[DatasetWebsitekitti]: http://www.cvlibs.net/datasets/kitti/eval_odometry.php

[DatasetWebsitewaymo]: https://waymo.com/open/

[DatasetWebsiteLyft]: https://level-5.global/data/

[DatasetWebsiteKAIST]: https://irap.kaist.ac.kr/dataset/

[DatasetWebsiteTUM_RGB_D]: https://vision.in.tum.de/data/datasets/rgbd-dataset/download

[DatasetWebsiteTUM_MonoVO]: https://vision.in.tum.de/data/datasets/mono-dataset

[DatasetWebsiteTUM_VI]: https://vision.in.tum.de/data/datasets/visual-inertial-dataset

[DatasetWebsiteUNI_Freiburg]: https://lmb.informatik.uni-freiburg.de/resources/datasets/SceneFlowDatasets.en.html

[DatasetWebsiteADVIO]: https://github.com/AaltoVision/ADVIO

[DatasetWebsiteOxford]: https://robotcar-dataset.robots.ox.ac.uk

[DatasetWebsiteHRI]: https://usa.honda-ri.com/honda-driving-datasets

[DatasetWebsiteArgoverse]: https://www.argoverse.org/data.html#download-link

[DatasetWebsiteEuRoC]: https://projects.asl.ethz.ch/datasets/doku.php?id=kmavvisualinertialdatasets

[DatasetWebsiteMalaga]: https://www.mrpt.org/MalagaUrbanDataset

[DatasetWebsiteICL_NUIM]: https://www.doc.ic.ac.uk/~ahanda/VaFRIC/iclnuim.html

[DatasetWebsiteCityscapes]: https://www.cityscapes-dataset.com/

[DatasetWebsiteNYUv2]: https://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html
