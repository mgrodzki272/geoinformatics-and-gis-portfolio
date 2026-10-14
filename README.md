# Geoinformatics, Remote Sensing & GIS Portfolio

> A collection of engineering projects, spatial analysis reports, remote sensing studies, and geological maps developed using **ArcGIS Pro**, **QGIS**, **CloudCompare**, and open geospatial registries (**GUGiK Geoportal**, **Copernicus Sentinel-2**, **Landsat 8**).

![ArcGIS Pro](https://img.shields.io/badge/ArcGIS_Pro-Field_Maps_%26_Cartography-007AC2?style=for-the-badge&logo=arcgis&logoColor=white)
![QGIS](https://img.shields.io/badge/QGIS-Spatial_Analysis_%26_SCP-589632?style=for-the-badge&logo=qgis&logoColor=white)
![Remote Sensing](https://img.shields.io/badge/Remote_Sensing-Sentinel--2_%7C_Landsat_8-blueviolet?style=for-the-badge)
![LiDAR](https://img.shields.io/badge/CloudCompare-ALS_LiDAR_3D-FF8C00?style=for-the-badge)

---

## 🖼️ Visual Highlights (Selected Maps & Spatial Models)

<p align="center">
  <img src="https://github.com/user-attachments/assets/0539a7f7-f23c-4725-871d-77907c085936" alt="z1" width="32%" />
  <img src="https://github.com/user-attachments/assets/038eb9f7-417c-4ad4-821e-faf05163b4ed" alt="z2" width="32%" />
  <img src="https://github.com/user-attachments/assets/81287534-e1fa-4f10-be77-f52270ed8796" alt="z4" width="32%" />
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/e8794d73-3132-492d-9461-94be635ce083" alt="z5" width="32%" />
  <img src="https://github.com/user-attachments/assets/b3996ac3-ee76-4ba6-8c79-7c4efc3a0e7f" alt="z6" width="32%" />
  <img src="https://github.com/user-attachments/assets/d0323c8f-e3d5-489b-89e8-df3840d6a0c9" alt="z3" width="32%" />
</p>

---

## 🗺️ Project & Report Index (Quick PDF Links)

| No. | Domain | Project / Documentation (Click to open PDF) | Core Tools & Data |
| :-: | :--- | :--- | :--- |
| **01** | **Geological Cartography** | 🗺️ **[Geological Map of the Szczawa Region – Zasadne Sheet (1:10,000)](./01_Mapa_Geologiczna_Szczawa_Zasadne.pdf)** | `ArcGIS Pro`, `PUWG 1992 (EPSG:2180)`, `DEM Hillshade` |
| **02** | **Geology & Tectonics** | 📘 **[Explanatory Notes to the Detailed Geological Map (Szczawa – Zasadne)](./02_Objasnienia_SMGP_Szczawa_Zasadne.pdf)** | `ArcGIS Field Maps`, `ArcGIS Pro`, `Mobile GIS` |
| **03** | **Geohazards (SOPO)** | ⚠️ **[Landslide Registration Card No. 145 156 (Pietrzejowice)](./03_Karta_Rejestracyjna_Osuwiska_Pietrzejowice.pdf)** | `QGIS`, `ISOK LiDAR Hillshade`, `Orthophotomap` |
| **04** | **Remote Sensing & ML** | 🛰️ **[Sentinel-2 Supervised Classification & Error Matrix Analysis](./04_Klasyfikacja_Sentinel2_SCP_QGIS.pdf)** | `QGIS`, `SCP Plugin`, `Sentinel-2`, `EPSG:32634` |
| **05** | **Renewable Energy / MCA** | ☀️ **[Multi-Criteria Site Selection for Solar Farms (Pomeranian Voivodeship)](./05_Analiza_Lokalizacji_Fotowoltaika_Pomorskie.pdf)** | `QGIS`, `Landsat 8`, `Sentinel-2 (NDVI)`, `LiDAR DEM` |
| **06** | **Hydrology / Urbanization** | 💧 **[Multi-Temporal Impervious Surface Analysis (2003–2024)](./06_Analiza_Obszarow_Nieprzepuszczalnych.pdf)** | `QGIS`, `Shapefile (EPSG:2180)`, `GUGiK Orthophotos` |
| **07** | **3D Point Clouds** | 🌲 **[Airborne Laser Scanning (ALS LiDAR) Point Cloud Processing](./07_Przetwarzanie_Chmury_Punktow_LiDAR.pdf)** | `CloudCompare`, `LAZ / LAS`, `3D Cross-Sections` |
| **08** | **Infrastructure & DEM** | 📐 **[Spatial, Viewshed, and Volumetric Terrain Analyses](./08_Analizy_Przestrzenne_Geoportal_NMT.pdf)** | `GUGiK Geoportal`, `DTM / DSM`, `BDOT500 / GESUT` |

---

## 🔍 Detailed Project Descriptions

### 1. 🪨 Digital Geological Mapping & Landslide Hazard Assessment
- **Detailed Geological Map of the Szczawa Region – Zasadne Sheet (1:10,000) with Explanatory Notes** ([`Map PDF`](./01_Mapa_Geologiczna_Szczawa_Zasadne.pdf) | [`Notes PDF`](./02_Objasnienia_SMGP_Szczawa_Zasadne.pdf))
  * **Scope:** Field geological survey covering approx. $3.20\text{ km}^2$ in the Gorce Mountains (Bystrica Subunit of the Magura Nappe), integrated with real-time mobile data acquisition in **ArcGIS Field Maps**.
  * **Methodology & Results:** Digitization of outcrop observation points, strike and dip measurements, and lithostratigraphic boundaries (Upper Cretaceous to Lower Eocene: Białe, Szczawina, Ropianka with the Głębieniec Member, Łabowa, and Beloveža formations). Reconstruction of thrust-fold tectonics (the Zasadne thrust sheet overriding the Szczawa unit, dissected by 9 transverse strike-slip faults) and cartographic production in **ArcGIS Pro** over a LiDAR-derived hillshade relief model.
- **Landslide Registration Card in Pietrzejowice (Inventory No. 145 156)** ([`View PDF`](./03_Karta_Rejestracyjna_Osuwiska_Pietrzejowice.pdf))
  * **Scope:** Documentation of an active translational earth slide (area: $3.91\text{ ha}$, vertical relief: $35.8\text{ m}$) prepared in accordance with the Polish Landslide Counteracting System (SOPO) standards.
  * **Methodology & Results:** Vectorization of verified and inferred landslide boundaries, main scarps, and colluvial toes using a Digital Elevation Model (**Hillshade**) and high-resolution orthophotomaps, accompanied by field inspection of infrastructure damage.

---

### 2. 🛰️ Satellite Remote Sensing & Multi-Criteria Spatial Analysis (QGIS)
- **Sentinel-2 Supervised Land Cover Classification & ROI Optimization** ([`View PDF`](./04_Klasyfikacja_Sentinel2_SCP_QGIS.pdf))
  * **Scope:** Multispectral supervised classification across 6 land cover classes (*Water, Built-up, Forests, Meadows, Cropland, Bare Soil*) in `EPSG:32634` using the **Semi-Automatic Classification Plugin (SCP)** in QGIS.
  * **Methodology & Results:** Comparative evaluation of three classifiers: *Maximum Likelihood* (`OA = 45.68%`, $\kappa = 0.297$), *Minimum Distance* (`OA = 45.98%`, $\kappa = 0.254$), and *Spectral Angle Mapping – SAM* (`OA = 53.01%`, $\kappa = 0.350$). By analyzing the *Area-Based Error Matrix* (*Producer's & User's Accuracy*), spectral confusion between classes was diagnosed and resolved through iterative re-engineering of training polygons (ROIs). **As a result, the overall accuracy (OA) of the SAM model increased from `53.01%` to `68.16%` ($\kappa$ improved to `0.516`), while User's Accuracy (UA) for cropland jumped from `3.0%` to `79.84%`.**
- **Multi-Criteria Site Selection for Utility-Scale Solar Farms (Pomeranian Voivodeship)** ([`View PDF`](./05_Analiza_Lokalizacji_Fotowoltaika_Pomorskie.pdf))
  * **Scope:** Multi-Criteria Analysis (MCA) evaluating over $180\text{ ha}$ of potential investment plots across three sites: Swarożyn ($28.4\text{ ha}$), Lubieszewo ($57.12\text{ ha}$), and Lichnowy ($99.17\text{ ha}$).
  * **Methodology & Results:** Multi-source raster fusion in **QGIS**: extracting terrain slope $< 10^\circ$ and southern aspect ($135^\circ\text{–}225^\circ$) from **LiDAR DEM**, computing vegetation index $\text{NDVI} < 0.4$ from **Sentinel-2** imagery, and deriving Land Surface Temperature $> 10^\circ\text{C}$ from **Landsat 8** thermal bands to exclude wetlands. Spatial findings were synthesized with business feasibility (direct *Corporate PPA* potential adjacent to industrial warehouses in Swarożyn) and geotechnical/drainage constraints in the Żuławy region.

---

### 3. 💧 Urban Hydrology, 3D LiDAR & Terrain Modeling (DTM/DSM)
- **Multi-Temporal Impervious Surface Analysis (2003–2024)** ([`View PDF`](./06_Analiza_Obszarow_Nieprzepuszczalnych.pdf))
  * **Scope:** Photointerpretation and polygon vectorization (Shapefile, `EPSG:2180`) of impervious vs. biologically active surfaces over a 20-year period using archival and contemporary orthophotomaps of increasing spatial resolution ($25\text{ cm} \rightarrow 10\text{ cm} \rightarrow 6.7\text{ cm}$).
  * **Results:** Automated surface statistics via the QGIS Field Calculator, documenting an increase in the imperviousness index from `0.55` (2003) to `0.76–0.78` (2013–2024) driven by urban densification, along with an assessment of surface runoff and local flooding risks.
- **Airborne Laser Scanning (ALS LiDAR) Point Cloud Processing** ([`View PDF`](./07_Przetwarzanie_Chmury_Punktow_LiDAR.pdf))
  * **Scope:** Processing and 3D spatial analysis of dense `.LAZ` point clouds in **CloudCompare**.
  * **Methodology & Results:** Visualization of laser return scalar fields (*RGB*, *Intensity*, ASPRS *Classification*), spatial segmentation of building structures, generation of longitudinal and transverse structural profiles using the *Cross Section* tool, and 3D coordinate extraction ($X, Y, Z$) of roof ridge and corner vertices via *Point list picking*.
- **Spatial, Viewshed, and Volumetric Terrain Analyses using DTM/DSM** ([`View PDF`](./08_Analizy_Przestrzenne_Geoportal_NMT.pdf))
  * **Scope:** Applied spatial engineering utilizing high-resolution elevation models (`DTM 1m` / `DSM 1m` in `PL-EVRF2007-NH` and `PUWG 1992 / EPSG:2180`).
  * **Results:** Underground utility network inventory (GESUT: `ks160` sewage, `wo63` water, `gn63` gas, `eN` power), elevation profile generation across the Biała River valley, $360^\circ$ areal *Viewshed* and *Line of Sight* obstruction modeling, and volumetric earthwork calculation for the Kościuszko Mound ($V = 111,841.08\text{ m}^3$).

---

## 🛠️ Technologies & Geospatial Standards
- **GIS & 3D Software:** ArcGIS Pro, ArcGIS Field Maps, QGIS, CloudCompare.
- **Remote Sensing & Elevation Data:** Sentinel-2 (MSI), Landsat 8 (TIRS/OLI), Airborne Laser Scanning ALS (ISOK LiDAR `.laz`), DTM / DSM (NMT / NMPT), GUGiK Orthophotomaps.
- **Coordinate Systems & Standards:** `EPSG:2180` (PUWG 1992), `EPSG:32634` / `EPSG:32635` (UTM), `EPSG:4326` (WGS84), `PL-EVRF2007-NH`, OGC Web Services (`WMS`, `WMTS`, `WFS`).
