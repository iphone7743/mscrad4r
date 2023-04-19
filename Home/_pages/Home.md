---
title: "Home"
permalink: /home/
author_profile: true
use_math: true
---


<br/>
<br/>
<br/>


# [1] Abstract

As autonomous driving research has actively progressed, software for autonomous vehicles and embedded systems such as Apollo and AutoWare have also been developed, providing a complete set of self-driving modules, including perception, localization and mapping, path planning, prediction, decision making, and control. Most of the researchers currently use these software programs, but many researchers have also studied autonomous driving based on the middleware software termed robot operating system (ROS) before such software was released, especially in academia.
Accordingly, we intend to develop ROS-based unmanned RC car equipped with autonomous driving sensors such as LiDAR, radar, VIS/IR cameras, GPS, and IMUs that can provide ROS-based datasets to researchers studying self-driving cars and robots using ROS. In addition, unlike conventional datasets, we acquire dataset  not only on road but also pedestrian paths that can be used in both vehicles and robots and provides extreme environmental datasets such as snowfall environments. In this sense, the ROS dataset we created will be helpful to researchers studying autonomous vehicles and robots by using ROS.
<br/>
<br/>
<br/>
<br/>




# [2] Related Works
Datasets for autonomous vehicles have been developed and collected by many researchers for over a decade. To increase the accuracy of various tools using deep learning, such as detection and segmentation, training datasets are important, and the performance accuracy is greatly affected depending on these datasets.


* __Waymo Open__ 

The Waymo Open Datasets were released in 2019, and Waymo released the largest dataset using the car platform. One mid-range LiDAR, 4 short-range LiDARs, and 5 cameras were used, and 360 degree field of view (FOV) coverage was used to label 3D objects.

* __nuScenes__

The nuScenes dataset comprises data collected from Boston and Singapore, and it is possible to experimentally study urban driving situations by equipping a complete sensor set of a real autonomous vehicle. It is the first dataset to feature a fully autonomous vehicle sensor suite, including 6 cameras with 360-degree FOV, 5 radars and 1 LiDAR.

* __ApolloScape__ 

The ApolloScape dataset contains a large amount of data and precise labeling. The dataset, collected in China in 2018, relies on 2 cameras, 2 LiDARs, a GPS and an IMU. The dataset contains data from various environments, such as darkness and rain.

* __CADC__ 

The Canadian Adverse Driving Conditions Dataset (CADC) dataset was collected during winter in Canada and is the first dataset that focuses on adverse driving conditions specifically. This module was collected with 8 cameras, LiDAR, a GNSS and an INS.

* __Argoverse__ 

The Argoverse dataset was collected in Pittsburgh and Miami from Carnegie Mellon University in 2019. The sensor data was configured with 7 cameras overlapping fields of view and long range LiDAR. This dataset focused on perception tasks which included 3D tracking and motion forecasting.

* __One Thousand and One Hours__ 

The One Thousand and One Hours dataset was acquired in Palo Alto and California with 1,118 hours from Cambridge, USA. The sensor configuration included 7 cameras, 3 LiDARs, and 5 radars. The released dataset was obtained at a 6.8 miles route between the train station and the office.
<br/>
<br/>
<br/>
<br/>
<br/>



# [3] Our Contribution
Many datasets and data collection platforms have been developed and will be researched in the future. However, it is difficult for researchers to apply data to software or to find different data for each purpose depending on the target. The following are the main contributions of this paper.

* __Flexibility__ 

First, the platform we developed has high value as a dataset that can be flexibly applied to autonomous vehicles as well as unmanned robots. There is a stereotype that unmanned robots are associated with indoor data and autonomous vehicles are associated with outdoor data, but our RC car-based platform can be applied both indoors and outdoors, and datasets can be collected in various environments. Because the pole in the middle of the platform can adjust the position of the LiDAR and cameras, various viewpoints, such as those of vehicles and people, can be applied.

* __Simplicity__  

The second contribution is that the dataset can use a ROSbag file as integrated data and original raw files. Most researchers studying unmanned robots and autonomous vehicles mainly use the ROS software. ROS-based dataset can reduce the time and effort for existing researchers to synchronize the data of each sensor or to acquire the data of a desired part. In conclusion, the platform has an important meaning in that it is the first data opened in the form of ROSbag.

* __Diversity__  

Last, this dataset includes data for extreme environments as well as general environments. We acquired the dataset using visual sensors, including an infrared camera and LiDAR, radar, IMU, and GPS. In particular, unlike existing datasets, extreme environment datasets were acquired using not only VIS cameras and LiDAR but also radar and IR cameras that are robust against environmental changes.



