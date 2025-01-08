---
layout: page
# title: "FoScenes"
# subtitle: "Large-scale forest 3D Plant Area Density products derived from open-access airborne lidar data"
# feature-img: "assets/img/pexels/computer.jpeg"
permalink: /foscenes
hide: False
hide_title: True
---

# FoScenes

**A High-Fidelity, Large-Scale 3D Forest Plant Area Density Product Derived From Open-Access Airborne Lidar Data**

The preliminary version of FoScenes releases 40 seamless scenes over 28 diverse sites, with individual area ranging from 50 to about 11,000 hectares, using ALS data acquired by NASA Goddard’s LiDAR, Hyperspectral & Thermal Imager [(G-LiHT)](https://glihtdata.gsfc.nasa.gov/).

### Sites map

From the tropical rainforests in Puerto Rico to the broadleaf-needleleaf mixed forests in Northeast US, FoScenes provides realistc representations across major forest biomes in North America.

![FoScenes Sites](/assets/img/Figure_1.jpg "FoScenes Sites")

### A Sample

The largest scene (about 11,500 ha) is for the WLEF site located 24 km west of Park Falls, Wisconsin, in the Chequamegon Nicolet National Forest.

![WLEF](/assets/img/Figure_5.png "WLEF")

## Download
[Google Drive](https://drive.google.com/drive/folders/1MO6odlAwKpRAWvHlDw8XkZ8CHGD_FJK4?usp=drive_link)


## Description
- vox_pad_ind.txt: [*x_index, y_index, z_index, Plant Area Density*] of each voxel. Index start at 0.
- proj.txt: Well-known text (WKT) string of the coordinate system.
- bord_size.txt: West, south and lowest border (coordinate of the origin point) and sizes of the scene (in meter).
- dtm_cloud.txt: 3D coordinate (relative to the origin point) of ground points (ceter point of each grid in DTM).
- dtm_dart.txt: ground points in DART coordinate system.
- Geotiff file: PAI (plant area index) maps by vertical integration, can be used for quality control. (Good quality: LAI>0, Non-vegetated: LAI=0, Insufficient lidar sampled: LAI=-1)

## Use FoScenes in DART
FoScenes can be easily used in [DART](https://dart.omp.eu/) for various simulation with DAO tools 
([DAO python scripts](https://drive.google.com/drive/folders/1LwEC1xPIfSWLTACyEBj2goRh0qzAHd5H?usp=drive_link)).


## Contact

For inquiries regarding FoScenes, please reach out to [Cailin](mailto:cailinzhou.polyu@gmail.com) ✉️.



We are open to collaborations in various forms. Please contact [Dr.YIN](https://www.polyu.edu.hk/lsgi/people/academic-staff/prof-yin-tiangang/) for futher details.
