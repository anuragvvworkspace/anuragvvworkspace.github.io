http://openaccess.thecvf.com/content_CVPR_2019/papers/Liang_Multi-Task_Multi-Sensor_Fusion_for_3D_Object_Detection_CVPR_2019_paper.pdf
Multi-Task Multi-Sensor Fusion for 3D Object Detection


### Abstract :
We present an end-to-end learnable architecture that
reasons about 2D and 3D object detection as well as ground
estimation and depth completion. 

fusing information at
various levels.


### Introduction :
[17 6] adopt cascade approach. Camera in first stage and reasoning in LiDAR point clouds in second stage.
17: Frustum pointnets for 3d object detection from rgb-d data. In CVPR, 2018
6: A general pipeline for 3d detection of vehicles. In ICRA, 2018

Others [5, 12, 13] have proposed to fuse multisensor features instead
Single-stage detectors [13] fuse multi-sensor feature maps per LiDAR point, 
where local nearest neighbor interpolation is used to densify the correspondence. 
However, the fusion is still limited when LiDAR points become extremely sparse at long range. 
