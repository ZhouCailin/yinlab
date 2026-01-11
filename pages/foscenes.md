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

# NEWS 
## [v2.0] - 2026-01-10
- Add **Incompletely Explored** voxels to scenes for more accurate representation, without affecting PAI.

- `vox_pad.txt` is now the only released vox PAD file 
(previously named `vox_pad_coord.txt` or `real_vox_pad_coord.txt`).

- `dtm_dart.txt` and `vox_pad_ind.txt` are no longer included in the data release. These files can be generated via the updated `clip.py`
  (see the following *Use FoScenes in DART* section).

## [v1.0] - 2025-01-08
- Initial release.

### Paper

![FoScenes Sites](/assets/img/foweb.png "FoScenes Sites")

Zhou, C., Yin, T., Wei, S., Cook, B.D., Tan, W., Yan, W.Y., Chen, Q., Gastellu-Etchegorry, J.-P., 2026. FoScenes: A high-fidelity, large-scale 3D forest plant area density product derived from open-access airborne lidar data. Remote Sens. Environ. 333, 115150. <https://doi.org/10.1016/j.rse.2025.115150>


## Download
- [Data in Google Drive](https://drive.google.com/drive/folders/1hHOTD3q9l3F3n_Ft-4JbpavJbWs1HMLd?usp=sharing)

- [Tools in Google Drive](https://drive.google.com/drive/folders/1bZ2u3NTwQxyV7xGP2b72Zh2y50q1qFki?usp=sharing)

## Data Description

### 1. 3D Space
The 3D voxel space is defined by the projection system, minimum borders, and spatial extents.

- `proj.txt`: Well-known text (WKT) string of the projection system.
- `bord_size.txt`:  
  [*Min_UTM_X, Min_UTM_Y, Elev_Lowest, Size_Of_X, Size_Of_Y, Size_Of_Z*]

All values are in meters. Elevation is referenced to the EGM96 geoid.

---

### 2. Voxel Plant Area Density (PAD) Files
Each row records either the **voxel center coordinates** or the **voxel indices** in the 3D voxelized space, together with its PAD value.

- `vox_pad.txt`: [*x, y, z, PAD*]
- `vox_pad_ind.txt`: [*i, j, k, PAD*]
- `vox_pad_coord.txt`: [*x, y, z, PAD*]

---

### 3. Digital Terrain Model (DTM)
The terrain point cloud is generated from a 1-m resolution DTM grid, provided in either the UTM coordinate system or the DART image coordinate system.

- `dtm_cloud.txt`: [*x, y, z*]
- `dtm_dart.txt`: [*col, row, z*]

---

### 4. Plant Area Index (PAI) Map
- GeoTIFF files: Plant Area Index (PAI) maps derived by vertical integration of PAD, primarily used for quality control.

  - Vegetated pixels: LAI > 0  
  - Non-vegetated pixels: LAI = 0  
  - Insufficient LiDAR sampling: LAI = −1


## Use FoScenes in DART
1. Download `clip.py` and `DARTDAO` from [Tools in Google Drive](https://drive.google.com/drive/folders/1bZ2u3NTwQxyV7xGP2b72Zh2y50q1qFki?usp=sharing).
2. Run `clip.py`
```python
python3 clip.py  --base /FoScenes/SERC_Jun2012/  --out /FoScenes/SERC_Jun2012/aoi/ --vs 2 --minxy 364600 4305700 --sizexy 100 100
```
3. Create a base DART simulation of DART
4. Configure parameters and run scripts of DARTDAO (FT/Lux).

## Contact & Collaboration

We welcome collaborations in various forms. If you have your own lidar data and are interested in forest structure reconstruction on your sites, please feel free to reach out.

For general inquiries regarding FoScenes, please contact  
**Cailin**: [cailinzhou.polyu@gmail.com](mailto:cailinzhou.polyu@gmail.com)

For collaboration opportunities and further details, please contact  
**Tiangang**: [tiangang.yin@polyu.edu.hk](mailto:tiangang.yin@polyu.edu.hk)
