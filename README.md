# Geoinformatics, Remote Sensing & GIS Portfolio

> Zbiór projektów inżynierskich, raportów z analiz przestrzennych, opracowań teledetekcyjnych oraz map geologicznych wykonanych z wykorzystaniem **ArcGIS Pro**, **QGIS**, **CloudCompare** oraz otwartych rejestrów geoprzestrzennych (**GUGiK Geoportal**, **Copernicus Sentinel-2**, **Landsat 8**).

![ArcGIS Pro](https://img.shields.io/badge/ArcGIS_Pro-Field_Maps_%26_Cartography-007AC2?style=for-the-badge&logo=arcgis&logoColor=white)
![QGIS](https://img.shields.io/badge/QGIS-Spatial_Analysis_%26_SCP-589632?style=for-the-badge&logo=qgis&logoColor=white)
![Remote Sensing](https://img.shields.io/badge/Remote_Sensing-Sentinel--2_%7C_Landsat_8-blueviolet?style=for-the-badge)
![LiDAR](https://img.shields.io/badge/CloudCompare-ALS_LiDAR_3D-FF8C00?style=for-the-badge)

---

## 🗺️ Zestawienie projektów i opracowań ( Szybki indeks PDF )

| Nr | Obszar tematyczny | Projekt / Dokumentacja (Kliknij, aby otworzyć PDF) | Główne narzędzia i dane |
| :-: | :--- | :--- | :--- |
| **01** | **Kartografia geologiczna** | 🗺️ **[Mapa Geologiczna Rejonu Szczawy – Arkusz Zasadne (1:10 000)](./01_Mapa_Geologiczna_Szczawa_Zasadne.pdf)** | `ArcGIS Pro`, `PUWG 1992 (EPSG:2180)`, `NMT Hillshade` |
| **02** | **Geologia i Tektonika** | 📘 **[Objaśnienia do Szczegółowej Mapy Geologicznej (Szczawa – Zasadne)](./02_Objasnienia_SMGP_Szczawa_Zasadne.pdf)** | `ArcGIS Field Maps`, `ArcGIS Pro`, `Mobile GIS` |
| **03** | **Geozagrożenia (SOPO)** | ⚠️ **[Karta Rejestracyjna Osuwiska nr 145 156 (Pietrzejowice)](./03_Karta_Rejestracyjna_Osuwiska_Pietrzejowice.pdf)** | `QGIS`, `ISOK LiDAR Hillshade`, `Ortofotomapa` |
| **04** | **Teledetekcja i ML** | 🛰️ **[Klasyfikacja Nadzorowana Sentinel-2 i Analiza Macierzy Błędów](./04_Klasyfikacja_Sentinel2_SCP_QGIS.pdf)** | `QGIS`, `SCP Plugin`, `Sentinel-2`, `EPSG:32634` |
| **05** | **OZE / Wielokryteriowa GIS** | ☀️ **[Analiza Przestrzenna Lokalizacji Farm Fotowoltaicznych (Woj. Pomorskie)](./05_Analiza_Lokalizacji_Fotowoltaika_Pomorskie.pdf)** | `QGIS`, `Landsat 8`, `Sentinel-2 (NDVI)`, `LiDAR DEM` |
| **06** | **Hydrologia / Urbanizacja** | 💧 **[Wieloczasowa Analiza Obszarów Nieprzepuszczalnych (2003–2024)](./06_Analiza_Obszarow_Nieprzepuszczalnych.pdf)** | `QGIS`, `Shapefile (EPSG:2180)`, `Ortofotomapy GUGiK` |
| **07** | **Chmury punktów 3D** | 🌲 **[Przetwarzanie Lotniczego Skaningu Laserowego ALS (LiDAR)](./07_Przetwarzanie_Chmury_Punktow_LiDAR.pdf)** | `CloudCompare`, `LAZ / LAS`, `3D Cross-Sections` |
| **08** | **Infrastruktura i NMT** | 📐 **[Analizy Przestrzenne, Widocznościowe (Viewshed) i Wolumetryczne](./08_Analizy_Przestrzenne_Geoportal_NMT.pdf)** | `Geoportal GUGiK`, `NMT / NMPT`, `BDOT500 / GESUT` |

---

## 🔍 Szczegółowy opis projektów w portfolio

### 1. 🪨 Cyfrowe Kartowanie Geologiczne i Analiza Osuwisk
* **Szczegółowa Mapa Geologiczna Rejonu Szczawy – Arkusz Zasadne (1:10 000) wraz z Objaśnieniami** ([`Mapa PDF`](./01_Mapa_Geologiczna_Szczawa_Zasadne.pdf) | [`Objaśnienia PDF`](./02_Objasnienia_SMGP_Szczawa_Zasadne.pdf))
  * **Zakres prac:** Terenowa inwentaryzacja geologiczna obszaru o powierzchni ok. $3{,}20\text{ km}^2$ w obrębie Gorców (jednostka bystrzycka płaszczowiny magurskiej) połączona z mobilną akwizycją danych w aplikacji **ArcGIS Field Maps**.
  * **Wyniki i metodologia:** Cyfryzacja punktów obserwacyjnych, biegów i upadów warstw oraz granic wydzieleń litostratygraficznych (od górnej kredy po eocen dolny: formacje z Białego, ze Szczawiny, ropianiecka z ogniwem z Głębieńca, z Łabowej oraz beloweska). Rekonstrukcja tektoniki łuskowej (nasunięcie łuski Zasadnego na łuskę Szczawy pocięte systemem 9 uskoków poprzecznych) i opracowanie finalnego arkusza mapy w **ArcGIS Pro** na podkładzie cieniowanego modelu terenu.
* **Karta Rejestracyjna Osuwiska w Pietrzejowicach (Nr ewid. 145 156)** ([`Zobacz PDF`](./03_Karta_Rejestracyjna_Osuwiska_Pietrzejowice.pdf))
  * **Zakres prac:** Opracowanie dokumentacji aktywnego osuwiska gruntowego (zsuw translacyjny o powierzchni $3{,}91\text{ ha}$ i rozpiętości pionowej $35{,}8\text{ m}$) zgodnie ze standardem instrukcji SOPO.
  * **Wyniki i metodologia:** Wektoryzacja granic pewnych i przypuszczalnych, skarp głównych oraz progów wewnątrzosuwiskowych (koluwium) na bazie numerycznego modelu rzeźby terenu (**Hillshade**) oraz ortofotomapy, wraz z dokumentacją terenową uszkodzeń infrastruktury.

---

### 2. 🛰️ Teledetekcja Satelitarna i Wielokryteriowe Analizy Przestrzenne (QGIS)
* **Klasyfikacja Nadzorowana Pokrycia Terenu (Sentinel-2) i Optymalizacja ROI** ([`Zobacz PDF`](./04_Klasyfikacja_Sentinel2_SCP_QGIS.pdf))
  * **Zakres prac:** Przeprowadzenie klasyfikacji wielospektralnej dla 6 klas pokrycia terenu (*Woda, Zabudowa, Lasy, Łąki, Uprawy, Gleby*) w układzie `EPSG:32634` przy użyciu wtyczki **Semi-Automatic Classification Plugin (SCP)** w QGIS.
  * **Wyniki i metodologia:** Porównanie trzech algorytmów klasyfikacji: *Maximum Likelihood* (`OA = 45.68%`, $\kappa = 0.297$), *Minimum Distance* (`OA = 45.98%`, $\kappa = 0.254$) oraz *Spectral Angle Mapping – SAM* (`OA = 53.01%`, $\kappa = 0.350$). Na podstawie analizy macierzy błędów (*Area-Based Error Matrix*, *Producer's & User's Accuracy*) zidentyfikowano problemy spektralnego nakładania się klas i przeprowadzono re-inżynierię poligonów treningowych ROI. **W efekcie poprawiono ogólną dokładność modelu SAM z `53.01%` do `68.16%` (wzrost $\kappa$ do `0.516`), a precyzję użytkownika (UA) dla klasy upraw podniesiono z `3.0%` do `79.84%`.**
* **Analiza Lokalizacyjna pod Wielkoskalowe Farmy Fotowoltaiczne w Woj. Pomorskim** ([`Zobacz PDF`](./05_Analiza_Lokalizacji_Fotowoltaika_Pomorskie.pdf))
  * **Zakres prac:** Wielokryteriowa analiza przestrzenna (MCA) ponad $180\text{ ha}$ gruntów inwestycyjnych w trzech lokalizacjach: Swarożyn ($28{,}4\text{ ha}$), Lubieszewo ($57{,}12\text{ ha}$) oraz Lichnowy ($99{,}17\text{ ha}$).
  * **Wyniki i metodologia:** Fuzja danych teledetekcyjnych i wysokościowych w **QGIS**: wyznaczenie nachylenia terenu $< 10^\circ$ oraz ekspozycji południowej ($135^\circ\text{–}225^\circ$) z danych **LiDAR DEM**, obliczenie wskaźnika wegetacji $\text{NDVI} < 0{,}4$ ze zobrazowań **Sentinel-2** oraz analiza termalna temperatury powierzchni $> 10^\circ\text{C}$ z satelity **Landsat 8** w celu eliminacji gruntów podmokłych. Zestawienie wyników algorytmu z uwarunkowaniami biznesowymi (potencjał linii bezpośredniej *Corporate PPA* w Swarożynie) oraz ryzykiem geotechniczno-melioracyjnym na Żuławach.

---

### 3. 💧 Hydrologia Miejska, LiDAR 3D i Analizy Terenowe NMT
* **Wieloczasowa Analiza Obszarów Nieprzepuszczalnych (2003–2024)** ([`Zobacz PDF`](./06_Analiza_Obszarow_Nieprzepuszczalnych.pdf))
  * **Zakres prac:** Fotointerpretacja i wektoryzacja poligonowa (Shapefile, `EPSG:2180`) powierzchni utwardzonych oraz biologicznie czynnych na przestrzeni 20 lat na podstawie archiwalnych i aktualnych ortofotomap o rosnącej rozdzielczości terenowej ($25\text{ cm} \rightarrow 10\text{ cm} \rightarrow 6{,}7\text{ cm}$).
  * **Wyniki:** Wyznaczenie statystyk powierzchniowych w kalkulatorze pól QGIS – udokumentowanie skoku wskaźnika nieprzepuszczalności z `0.55` (2003 r.) do `0.76–0.78` (2013–2024) wskutek postępującej urbanizacji oraz ocena wpływu uszczelnienia zlewni na spływ powierzchniowy i ryzyko podtopień.
* **Przetwarzanie Chmur Punktów Lotniczego Skaningu Laserowego (ALS LiDAR)** ([`Zobacz PDF`](./07_Przetwarzanie_Chmury_Punktow_LiDAR.pdf))
  * **Zakres prac:** Praca z gęstymi chmurami punktów w formacie `.LAZ` w środowisku **CloudCompare**.
  * **Wyniki i metodologia:** Analiza atrybutów skalarnych wiązki laserowej (*RGB*, *Intensity*, *Classification* ASPRS), segmentacja przestrzenna zabudowy, generowanie przekrojów podłużnych i poprzecznych bryły budynku narzędziem *Cross Section* oraz ekstrakcja współrzędnych 3D ($X, Y, Z$) narożników połaci dachowych za pomocą *Point list picking*.
* **Analizy Przestrzenne, Widocznościowe i Wolumetryczne na bazie NMT/NMPT** ([`Zobacz PDF`](./08_Analizy_Przestrzenne_Geoportal_NMT.pdf))
  * **Zakres prac:** Wykorzystanie usług sieciowych i modeli wysokościowych (`NMT 1m` / `NMPT 1m`, układ `PL-EVRF2007-NH` oraz `PUWG 1992 / EPSG:2180`).
  * **Wyniki:** Inwentaryzacja sieci uzbrojenia terenu (GESUT: `ks160`, `wo63`, `gn63`, `eN`), generowanie profili podłużnych terenu wzdłuż tras dojścia z identyfikacją wcięcia erozyjnego rzeki Białej, analiza widoczności obszarowej (*Viewshed* $360^\circ$) i liniowej (*Line of Sight*) z uwzględnieniem przeszkód terenowych oraz obliczenie objętości mas ziemnych bryły Kopca Kościuszki ($V = 111\,841{,}08\text{ m}^3$).

---

## 🛠️ Wykorzystywane technologie i standardy
* **Systemy GIS i 3D:** ArcGIS Pro, ArcGIS Field Maps, QGIS, CloudCompare.
* **Teledetekcja i dane wysokościowe:** Sentinel-2 (MSI), Landsat 8 (TIRS/OLI), Lotniczy Skaning Laserowy ALS (ISOK LiDAR `.laz`), NMT / NMPT, Ortofotomapy GUGiK.
* **Standardy i układy odniesienia:** `EPSG:2180` (PUWG 1992), `EPSG:32634` / `EPSG:32635` (UTM), `EPSG:4326` (WGS84), `PL-EVRF2007-NH`, usługi OGC (`WMS`, `WMTS`, `WFS`).
