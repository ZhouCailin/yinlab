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

<!-- **A High-Fidelity, Large-Scale 3D Forest Plant Area Density Product Derived From Open-Access Airborne Lidar Data** -->

<!-- > **FoScenes: A high-fidelity, large-scale 3D forest plant area density product derived from open-access airborne lidar data**
> Zhou, C., Yin, T., Wei, S., Cook, B.D., Tan, W., Yan, W.Y., Chen, Q., Gastellu-Etchegorry, J.-P., 
> *Remote Sensing of Environment*, 2026. -->

> Zhou, C., Yin, T., Wei, S., Cook, B. D., Tan, W., Yan, W. Y., ... & Gastellu-Etchegorry, J. P. (2026). FoScenes: A high-fidelity, large-scale 3D forest plant area density product derived from open-access airborne lidar data. *Remote Sensing of Environment*, 333, 115150.

**Data Portal**: <https://foscenes.3msi.net/> \
**Access paper**: <https://doi.org/10.1016/j.rse.2025.115150>

The preliminary version of FoScenes releases 40 seamless scenes over 28 diverse sites, with individual area ranging from 50 to about 11,000 hectares, using ALS data acquired by NASA Goddard’s LiDAR, Hyperspectral & Thermal Imager [(G-LiHT)](https://glihtdata.gsfc.nasa.gov/).

![FoScenes Sites](/assets/img/foweb.png "FoScenes Sites")

### Updates
[News] The data access portal is now online. Download 3D scenes and DART simulation by interactive webpage.

[v2.2] 2026-05-21 Fix inconsistency in delimiter, now 'space' for all data.

[v2.1] 2026-01-10 Fix inconsistency between sites and data files.

[v2.0 ] 2026-01-10
- Add **Incompletely Explored** voxels to scenes for more accurate representation, without affecting PAI.

- `vox_pad.txt` is now the only released vox PAD file 
(previously named `vox_pad_coord.txt` or `real_vox_pad_coord.txt`).

- `dtm_dart.txt` and `vox_pad_ind.txt` are no longer included in the data release. These files can be generated via the updated `clip.py`
  (see the following *Use FoScenes in DART* section).

[v1.0] 2025-01-08 Initial release

<!-- ### Publications

[DOI](https://doi.org/10.1016/j.rse.2025.115150) | [Sciencedirect](https://www.sciencedirect.com/science/article/pii/S0034425725005541?via%3Dihub#t0005) | [PDF](https://pdf.sciencedirectassets.com/271745/1-s2.0-S0034425725X0002X/1-s2.0-S0034425725005541/main.pdf?X-Amz-Security-Token=IQoJb3JpZ2luX2VjEAUaCXVzLWVhc3QtMSJIMEYCIQDdyjBljs%2BdVH49slQhYUXxm3fYEc%2BXnHpCmpUBngPbFwIhAKcraoblLTulsF%2BDubx2AxjdYPjREpuH9vG10p%2B%2BgcQfKrwFCM7%2F%2F%2F%2F%2F%2F%2F%2F%2F%2FwEQBRoMMDU5MDAzNTQ2ODY1Igx7hkKQXJSqaJ5UkLEqkAVTK1tZRHLEjzSuc%2BUCHbxmRFBtGkBKKpy8HXDEaHQPrQUrVURokgqi1C4c2KMfL0tVch5qzg%2B1%2F4CNh0XoWyb2l%2BVZ0I4TS7Z9pB0kP1cHSlYPL7vabLjT9AsGeyVfBsKZYcTgI1CmmrsmkkGRshgZ3492EYKkPGbokfhNFA5RWDggYFCmQZQbrkUZWRvlpUsBIl4kNfbE5r1B1irWU0yFGRS04ETz6A82EV%2FsSg9RBgxj7RJng7mJ18YKv4fmGVFXVMIMS%2FpQ4qvwc8cZe61kDiaZod9458zFH8kxPTvJqs6kIEnLmqZxY8sfno1BAmCAWe2ZcdyTlgdWcl%2BR%2FA1UKovB8USm8NL1uehN9fUAmsESJmdeTFjbKK%2BGzPdCjCc0BdKgWVsTyTOB4eGHTgt6bJaFEMF2lJmrqbG6AhrnR7hzVEgXnqh4CqJ%2BvwqX6RzkkB3xcXOXSE2pELRRgKCiN%2FFpAThffr9DAqO%2B7WCBXZsAmIc4rgw%2F5okNrVCwFvW5WAsnZwlvcHPbtB1%2FHeB2AQhQNSG4Rsx74lhOowVE%2B%2FZ8PZ8LE1EvhtsDB%2BAg%2B84z9hxIk5Sg2zBswFE%2Bb953QRjheEnOx4I7vbhh4kgi2izjBSnN3%2BAO7Etcx8zITuUWNWU7w2i1sq%2BS2ZNuw63fMcZqeDaM2cc31tgiqV22Aupg9uPv9uDkVdWvPN2dHdlYVr8ahOujv4V6Ms%2BJ0VrGbJbAzmFWpaHSFzXz%2F7%2F9Xvpz%2FrsA5s%2BHhuUqNr7n6uxrC9LfT05Ijt7LS0tNzwAUD63Jc6nvCXuWpTWKcOkPF9HW%2FbTMDgHOtCgxoKn%2BRZa3p%2Bog2ocoRx6%2FKZ3TCK8SG21Mqgeoikj7oHFcKuytRjD30YzLBjqwAb524Y1H30gvvVUKzp5qJ2j8G9dFpRDirZHBT32KgxZ2QZqaqGv2QaOe8eTULsGhHDl7OKpyp5QJgD44FuAhJZwVehqvdlbRkcSyQwmjpOHJmB7cjIsOLOAm9sSz6a9ani96Vpr0m53VZoFVVD%2BS4GXvSEw8l4LL7Y6W1m8Z%2B47ZYtZrIobpZ3JQ4zhxhhb1o2qyvnlWi3DJlJfbPTSJolLmeyNbDDyHnz8Id2gEFK8a&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20260111T051013Z&X-Amz-SignedHeaders=host&X-Amz-Expires=299&X-Amz-Credential=ASIAQ3PHCVTY6LU52FAH%2F20260111%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Signature=82f4e25fe98c9a258fef5b825d8bf0dbf5b70fa6e6cc88668e4f535255ac8341&hash=792cf7dd72f70b56858177ab09d5dc7e32bff50440c02cc2b922ac50859c4114&host=68042c943591013ac2b2430a89b270f6af2c76d8dfd086a07176afe7c76c2c61&pii=S0034425725005541&tid=spdf-7d6d01b9-1068-40dd-aafb-4fb5e4f05feb&sid=0b56c7d251470642a149730877dc101815aegxrqa&type=client&tsoh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&rh=d3d3LnNjaWVuY2VkaXJlY3QuY29t&ua=1c055b060d50055a51&rr=9bc1e806af7c6bdc&cc=sg&kca=eyJrZXkiOiJHWkdUQzUrdnM2MDE5OGh0bzlLK1pDNFhGYS8xNG1rT1RKVTgyVkJsZmdNRy8xOUE0TWhNZXFDc3M2N2RWRU1ZRGUrL25uWVgydm9XTnJOVDVOZm52UFZJTEdJVUtMS1FOVUZoaUdNYU13am5ienlXZFBvQTFhQ0RoWHZ0dmQ1ZnNOa0ZMejdUUS8yWEZUWFB2amtOeUNINFRUcmthcVpXbFo4Qm1aaGo4L1EzUFo0TUd3PT0iLCJpdiI6ImYzMmI1ZTE0ZTdlNGJkNGFhYjI2OWExMDgyOTYwNDY1In0=_1768108244660) | [Google](https://scholar.google.com/citations?view_op=view_citation&hl=zh-CN&user=NyTZ_kMAAAAJ&citation_for_view=NyTZ_kMAAAAJ:u5HHmVD_uO8C)

![FoScenes Sites](/assets/img/foweb.png "FoScenes Sites")

> **FoScenes: A high-fidelity, large-scale 3D forest plant area density product derived from open-access airborne lidar data**
> Zhou, C., Yin, T., Wei, S., Cook, B.D., Tan, W., Yan, W.Y., Chen, Q., Gastellu-Etchegorry, J.-P., 
> *Remote Sensing of Environment*, 2026.


>**Absract:** The accurate three-dimensional (3D) distribution of plant area density (PAD) within forests is crucial for understanding canopy structure and provides essential scene inputs for 3D Radiative Transfer Models (RTMs) to facilitate remote sensing interpretation. However, current lidar-based voxelization methods that estimate detailed PAD distributions often cover limited areas, constraining their applications in conducting broad forest studies and interpreting Earth Observation Satellite (EOS) data of various scales and resolutions. To address this, we developed the Large-Scale Path Volume Leaf Area Density (LS-PVlad), a novel forest 3D reconstruction workflow capable of producing extensive high-resolution 3D voxelized forest scenes (up to 100 km2 with ≤2 m voxel size) from worldwide open-access airborne lidar scanning (ALS) data. By applying LS-PVlad to the ALS data acquired during the extensive NASA Goddard's LiDAR, Hyperspectral & Thermal Imager (G-LiHT) campaigns, we developed the first release of FoScenes—a high-fidelity PAD product comprising 40 seamless scenes from 28 diverse forest sites, with individual area ranging from ∼50 to ∼11,000 ha. The leaf area estimates of LS-PVlad have been validated by two-year field-measured leaf area index (LAI) from litter collection (best RMSE = 0.35 m2/m2) and digital hemispherical photography (DHP) images (RMSE = 0.46 m2/m2) across multiple plots at a deciduous forest site. Additionally, a broad comparison between FoScenes and MODIS plant/leaf area index product demonstrates high consistency (R2 = 0.70, RMSE = 0.86 m2/m2). By providing multi-dimensional forest characterizations, FoScenes enables temporal insights into structure dynamics. Its integration with the discrete anisotropic radiative transfer (DART) model underscores the potential of FoScenes for extensive 3D RTM applications at various scales. -->


### Download
<!-- - **FoScenes datasets [v2.2]**:
[Google Drive](https://drive.google.com/drive/folders/1nSVK-AbvBKE0Tx32bIpyhj6gediMHpmr?usp=drive_link) -->

![portal](/assets/img/fsc-portal.png "FoScenes Sites")

-  **Data Access Portal**: <https://foscenes.3msi.net/>

-  **Tools and DART-DAO**:
[Google drive](https://drive.google.com/drive/folders/1bZ2u3NTwQxyV7xGP2b72Zh2y50q1qFki?usp=sharing)
  
The list of sites is provided in paper [Table of sites](https://www.sciencedirect.com/science/article/pii/S0034425725005541?via%3Dihub#t0005).

### Data Description

#### 1. 3D Space
The 3D voxel space is defined by the projection system, minimum borders, and spatial extents.

- `proj.txt`: Well-known text (WKT) string of the projection system.
- `bord_size.txt`:  
  [*Min_UTM_X, Min_UTM_Y, Elev_Lowest, Size_Of_X, Size_Of_Y, Size_Of_Z*]

All values are in meters. Elevation is referenced to the EGM96 geoid.

---

#### 2. Voxel Plant Area Density (PAD) Files
Each row records either the **voxel center coordinates** or the **voxel indices** in the 3D voxelized space, together with its PAD value.

- `vox_pad.txt`: [*x, y, z, PAD*]
- `vox_pad_ind.txt`: [*i, j, k, PAD*]
- `vox_pad_coord.txt`: [*x, y, z, PAD*]

---

#### 3. Digital Terrain Model (DTM)
The terrain point cloud is generated from a 1-m resolution DTM grid, provided in either the UTM coordinate system or the DART image coordinate system.

- `dtm_cloud.txt`: [*x, y, z*]
- `dtm_dart.txt`: [*col, row, z*]

---

#### 4. Plant Area Index (PAI) Map
- GeoTIFF files: Plant Area Index (PAI) maps derived by vertical integration of PAD, primarily used for quality control.

  - Vegetated pixels: LAI > 0  
  - Non-vegetated pixels: LAI = 0  
  - Insufficient LiDAR sampling: LAI = −1


<!-- ### Use FoScenes in DART
1. Download `clip.py` and `DARTDAO` from [Tools](https://drive.google.com/drive/folders/1bZ2u3NTwQxyV7xGP2b72Zh2y50q1qFki?usp=sharing).
2. Run `clip.py`
```python
python clip.py  --base /FoScenes/SERC_Jun2012/  --out /FoScenes/SERC_Jun2012/aoi/ --vs 2 --minxy 364600 4305700 --sizexy 100 100
```
3. Create a base simulation of DART.
4. Configure parameters and run scripts of DARTDAO (FT/Lux) following `readme.txt`. -->

### Citation
```bibtex
@article{zhou2026foscenes,
  title   = {FoScenes: A high-fidelity, large-scale 3D forest plant area density product derived from open-access airborne lidar data},
  journal = {Remote Sensing of Environment},
  volume  = {333},
  pages   = {115150},
  year    = {2026},
  issn    = {0034-4257},
  doi     = {10.1016/j.rse.2025.115150}
}
```

### Contact & Collaboration

We welcome collaborations in various forms. If you have your own lidar data and are interested in forest structure reconstruction on your sites, please feel free to reach out.

For general inquiries regarding FoScenes, please contact  
**Cailin**: [cailinzhou.polyu@gmail.com](mailto:cailinzhou.polyu@gmail.com)

For collaboration opportunities and further details, please contact  
**Tiangang**: [tiangang.yin@polyu.edu.hk](mailto:tiangang.yin@polyu.edu.hk)
