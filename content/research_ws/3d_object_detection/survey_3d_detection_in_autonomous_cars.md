http://sci-hub.tw/https://ieeexplore.ieee.org/document/8621614
A Survey on 3D Object Detection Methods for Autonomous Driving Applications

Abstract:  
This paper presents an overview of 3D object detection methods and prevalently used sensors and datasets in AVs. It then discusses and categorizes the recent  
works based on sensors modalities into monocular, point cloud-based, and fusion methods.  

WE divide3d object detection methods in three catagories.  
Monocular image, point cloud and fusion based methods:  

####  Monocular Image Based Methods:  
Mono3D:
  : Built on 3DOP(previous work of the author which uses depth images)   
Pham and Jeon [44] extends the 3DOP which is better performing than 3DOP or Mono3D   
  : re-ranks the proposals using both monocular images and depth  
  : Class independent proposals
3D Voxel Pattern (3DVP) [41] representation  
  : accounts for occlusion  
  : dependant on performance of Region Proposal Networks(RPNs)  
Extending 3DVP framework, same author proposes SubCNN  
  : Candidates are extracted using convolutional layers to predict heat maps for each subcategory at the RPN level.
  :3DVP methods modelled as classification into a set of orientations. Hence an arbitrary orientation might not fit well.
Deep MANTA [42] tackles the above prob, uses a many-task network to estimate vehicle position, part localization and shape based only on monocular images.  


#### Pointcloud methods:  
Three types :  
* Projection based
* Volumetric representation based
* POintNet

###### Projection methods
Li et al:
    * 
