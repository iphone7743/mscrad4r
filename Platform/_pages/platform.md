---
title: "Platform"
permalink: /platform/
author_profile: true
use_math: true
header:
  overlay_image: /assets/images/fig1_IONIQ.png
  overlay_filter: 0.5
---


<br/>
<br/>
<br/>


# [1] IONIQ Test Vehicle
<br/>
<img src="/assets/images/fig1_IONIQ.png" width="100%" height="100%" title="CAD design of a ROS-based small unmanned platform" alt="1"/> 



Above figure shows the sensor coordinate systems and CAD design of the ROS-based small unmanned platform. The platform consists of the chassis and driving system based on __Traxxas 77086-4__. The driving system of Traxxas consists of a motor driver (VXL-8s, electronic speed controller), driving motor (1200XL, Velineon), steering motor (2085 servo, Traxxas), and additional encoder (RE30E-1000, Copal) for feedback control of platform speed. The whole driving system is powered by its own two 6700 mAh 14.8 V LiPo battery packs in parallel (2890c, Traxxas). In addition, we proceeded with the mobile PC Xavier for sensor acquisition and additional 3D design for autonomous sensors. Additionally, a monitoring desktop has been added to monitor ROS topic messages of sensors by a Wi-Fi router in real time1.
<br/>
<br/>
<br/>
<br/>



# [2] Sensor Configuration
<br/>
<img src="/assets/images/Sensor_com.png" width="100%" height="100%" title="CAD design of a ROS-based small unmanned platform" alt="1"/> 

Above figure shows the sensor architecture for autonomous driving of this platform, which includes __LiDAR, radar, stereo camera, thermal camera, IMU and GPS__. For a sufficient sensor power supply, the platform is equipped with an additional 40.8 Ah 12 V lithium-ion battery (18650, Lunavolt). Dimensions between each sensor are contained in the figure and are related to extrinsic parameters. Considering a real vehicle, the LiDAR height is set to 1,149 mm from the ground surface. Similarly, the height of the stereo RGB camera is set to 1,009 mm from the earth. The thermal camera, GPS, IMU and radar are located in the centerline with heights of 1,047 mm, 570 mm, 390mm and 150 mm, respectively. To prevent LiDAR oscillation in the roll/pitch direction, the velocity and stiffness of the suspension spring of the platform were limited. One important aspect of the proposed platform is waterproof cover design, which can help protect the sensors from rain, snow, dust and external impacts.
<br/>
<br/>
<br/>
<br/>



# [3] Sensor Specifications

<br/>

* __LIDAR : OS-1 Gen2__
  
Specification | Value
--- | ---
vertical resolution | 64 ch 
horizontal resolution | 1024 
precision | + - 0.7 ~ 5 cm
vertical FOV | 45 degree
rotation rate | 20 Hz 
range | 240 m         

<br/>


* __RADAR : ARS 408-21__
  
Specification | Value
--- | ---
frequency band |  77 GHz
range | 0.2 ~ 250 m       
vel accuracy | +- 0.1 km/h
azimuth accuracy | +-0.1 degree
cycle time | app. 0.72 ms  

<br/>


* __VIS CAMERA : BFS-U3-16S2C-CS__

Specification | Value
--- | ---
mage format | BayerRG12p
image format | YUYV  
sensor type  | 12-Bit RAW
resolution | 1440 x 1080  
pixel Size | 4.5 x 4.5 µm  
frame rate |  43 FPS 

<br/>

            
* __Thermal CAMERA : Boson__
        
Specification | Value
--- | ---
image format | YUV 
sensor type | 12-Bit RAW
resolution  | 640 x 512 
pixel pitch | 12 µm 
frame rate  | 30 FPS           

<br/>


* __GPS : MRP-2000__  

Specification | Value
--- | ---
satellites signal tracking | GPS, GLONASS, Beidou, Galileo, QZSS, SBAS             
 RTK accuracy |  +- 3 cm 
 sensing rate | 20 Hz      

<br/>


* __IMU : MTI-630R__

Specification | Value
--- | ---
roll(static)  | 0.2 degree RMS                        
pitch(static) | 0.2 degree RMS 
roll(dynamic) |  0.5 degree RMS   
pitch(dynamic) |0.5 degree RMS        
yaw | 1 degree RMS                 
