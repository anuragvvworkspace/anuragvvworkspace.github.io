Image authenticity: Find out if the image is raw or ect...
We need a module that verifies authenticity of an image – whether it is raw, processed, forged or not.
This is a very mature area and has lots of work behind it. Multimedia forensics also come under the same topics. Let Anurag start with literature search and feature search in other software. The likes of PRNU and related techniques are very popular. It will be good to have the basic things in place.


An Overview on Image Forensics  2013  
==============================
https://sci-hub.tw/https://www.researchgate.net/publication/258394548_An_Overview_on_Image_Forensics  

**Two questions** about the history and credibility of an image can be raised:  
. Was the image acquired by the device it is claimed to be sensed with?  
. Is the image still depicting the captured original scene?  

Research in multimedia content security has proposed several approaches that can be frst of all classifed into  
**Active and Passive methods :**  
Active means some form of information compiled by the trusted camera is used to check the authenticity.  
Active : Fragile digital watermarking, cryptographic digital signatures.   

Passive means, only the digital content at disposal is present.  


**watermarkde :**  
Cameras need to have the watermarking signature. Manufactureres need to follow a protocol, which is very difficult in large scale.

Actuasition footproint  
Coding footprint  
Editing footprint


Digital Image Life Cycle
------------------------
Acquisition, Coding, and Editing  

**Acquisition**  
fltered by the CFA (Color Filter Array) before reaching sensor  
Acquasition: Light sensed by CMOS/CCD  to filter different colours.  
demosaicing process to combine all colours.  
In-camera processing like white balancing, color processing, image sharpening, contrast enhancement and gamma correction.  

**Coding**
lossy compressed in most cameras and JPEG in commercial devices.

**Postprocessing**
Any image editing that includes geometric transformation, sharpeining, contrast adjustment, image splicing ect.


**Def :  Image Ballastic ** - Signature of a camera type or even the individual camera that is left on an image by the individual stages of image acquasition.   


**Two main aims of image forensics:**  
1. Source Identification  
* 1. - obtain Image ballastics and classify it to specific model or device
2. Tampering detection  
* 1. - inconsistancy or absence of acquasition or coding fingureprints reveals presence of post processing
* or 
* 2. - detecting presence of editing fingureprints representing a given post processing

Image acquasition
-----------------
Lens, sensor and colour filter array.  

**Lens characteristics**  
. Lateral Chromatic abbaration:  This lens aberration causes different  
light wavelengths to focus on shifted points in the image  
plane represented by the sensor, when the source light is off  
the optical axis, resulting in a misalignment between color  
channels.  
[16] Lateral chromatic abberation. Each colour has a different focus point.  
Three parameters required to define the distortion per colour. image registration of sorts for detection shift.  
Unique to each lens.  
Johnson and Farid detect forgaries by looking for deviations in the above pattern.
[17] Mobile phone identification by feeding abberation parameters to SVM.  
[18] intrinsicl radial distrotion of lens instead of camera source identification.  
[19] Dust patterns are modeled in order to identify single device from an image.  
[20] Purple Fringing Abberation(PFA) more complex but more visible as purple halos around an object. Used for tampering detection.

**Sensor based footprints**  

Dominating component of sensor pattern noise is the photoresponse nonuniformity(**PRNU**)  
PRNU is a high frequency multiplicative noise, generally stable throughout the camera’s lifetime in normal operating  
conditions, that is, unique to each camera.  

**CFA Pattern**  
Demosaicing is the trace caused due to colour filters.  
two main classes:  
. algorithms aiming at estimating the parameters of the color interpolation algorithm and
the structure of the pattern filter  
. algorithms aiming at evaluating the presence/absence of demosaicing traces.  
First intended to classify sources and second focuses on forgery  


Conclusion
----------
1. 

Digital image forgery detection using passive techniques: A survey
==================================================================
http://sci-hub.tw/https://www.sciencedirect.com/science/article/pii/S1742287613000364


Digital image forgery detection: a systematic scrutiny 
======================================================
https://sci-hub.tw/https://www.tandfonline.com/doi/abs/10.1080/00450618.2018.1424241

**Taxonomy of digital image forgeries**  
important ones are copy-move forgery and image splicing  

**Classification of digital image forgery detection methods**  
. Source camera Identification  
. Discrimination  
. Digital Image Forgery Detection  
. . Active Methods  
. . . Watermarks  
. . Passive Methods  
. . . Forgery type dependent  
. . . . Copy-move forgery detection methods  
. . . . 1. Dividing image into segments  
. . . . 2. Feature extraction  
. . . . 3. Feature matching  
. . . . . . Block based  
. . . . . . Keypoint based   
https://www.youtube.com/watch?v=qtkUnkY1zE4  

. . . . Splicing based methods  
. . . . Fusion-based methods  

. . . Forgery type independent  
. . . . Inconsistency-based:
