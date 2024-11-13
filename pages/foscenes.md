---
layout: page
title: "FoScenes"
subtitle: "Large-scale forest 3D Plant Area Density products derived from open-access airborne lidar data"
feature-img: "assets/img/pexels/computer.jpeg"
permalink: /foscenes
hide: True
---

# FoScenes V1
The preliminary version of FoScenes releases 40 seamless scenes over 29 selected sites of various forest types and observation time, 
with the area ranging from 50 to about 11,000 hectares, using ALS data acquired by NASA Goddard’s LiDAR, Hyperspectral & Thermal Imager [(G-LiHT)](https://glihtdata.gsfc.nasa.gov/).

## Download
[Google Drive](https://drive.google.com/drive/folders/10Uw_SXG-TfDQzeincIlaEy6j2apuAg1s?usp=sharing)
\\
[Tencent Weiyun] In progress

## Description
- vox_pad_ind.txt: *x_ind, y_ind, z_ind, Plant Area Density* of each voxel
- proj.txt: WKT string
- bord_size.txt: 3D border (x, y, z in projected system) and sizes of the scene (meter).
- dtm_cloud.txt: 3D relative coordinate of ground points (ceter point of each grid in DTM).
- dtm_dart.txt: same as dtm_cloud.txt but in DART coordinate system.
- LAI.tif: Generated LAI maps by vertical integration, can be used for quality control. (Good quality: LAI>0, Non-forest/vegetation: LAI=0, Low/no lidar sample: LAI=-1)

## Use FoScenes in DART
The 3D scenes provided by FoScenes can be easily used in [DART](https://dart.omp.eu/) for various simulation with DAO tools 
([DAO python scripts](https://drive.google.com/drive/folders/1LwEC1xPIfSWLTACyEBj2goRh0qzAHd5H?usp=drive_link)).
