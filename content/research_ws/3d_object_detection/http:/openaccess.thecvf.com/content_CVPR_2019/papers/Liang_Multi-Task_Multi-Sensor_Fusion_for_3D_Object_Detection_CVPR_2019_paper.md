http://openaccess.thecvf.com/content_CVPR_2019/papers/Liang_Multi-Task_Multi-Sensor_Fusion_for_3D_Object_Detection_CVPR_2019_paper.pdf

Multi-Task Multi-Sensor Fusion for 3D Object Detection
=========

Abstract :
---------
We present an end-to-end learnable architecture that
reasons about 2D and 3D object detection as well as ground
estimation and depth completion. 

fusing information at
various levels.


Introduction :
--------------
Recently, several attempts [5, 17, 12, 13] have been developed to fuse information from multiple sensors.

[17 6] adopt cascade approach. Camera in first stage and reasoning in LiDAR point clouds in second stage.
> 17: Frustum pointnets for 3d object detection from rgb-d data. In CVPR, 2018  
> 6: A general pipeline for 3d detection of vehicles. In ICRA, 2018  

Others [5, 12, 13] have proposed to fuse multisensor features instead

**Single-stage detectors** [13] fuse multi-sensor feature maps per LiDAR point, 
where local nearest neighbor interpolation is used to densify the correspondence. 
However, the fusion is still limited when LiDAR points become extremely sparse at long range. 

> 13: Deep continuous fusion for multi-sensor 3d object detection. In ECCV, 2018

**Twostage detectors** [5, 12] fuse multi-sensor features per object
region of interest (ROI). However, the fusion process is typically slow (as it involves thousands of ROIs) and imprecise
(either using fix-sized anchors or ignoring object orientation).

> [5] Multi-view 3d object detection network for autonomous driving. In CVPR 2017  
> [12]  Joint 3d proposal generation and object detection from view aggregation. In IROS, 2018 

**This paper**  
* develops a multi-sensor detector that reasons about 2D and 3D object detection, ground estimation and depth completion.  
* Importantly, our model can be learned end-to-end and performs all these tasks at once.  
* Leverages the advantages from both point-wise and ROIwise feature fusion  
. estimates an accurate voxel-wise ground location 

