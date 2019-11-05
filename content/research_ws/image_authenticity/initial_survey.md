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


Image acquasition
-----------------
Lens, sensor and colour filter array.  

**Lens characteristics**  
. Lateral Chromatic abbaration  

**Sensor based footprints**  

Dominating component of sensor pattern noise is the photoresponse nonuniformity(**PRNU**)  
PRNU is a high frequency multiplicative noise, generally stable throughout the camera’s lifetime in normal operating  
conditions, that is, unique to each camera.

