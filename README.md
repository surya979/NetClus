# NetClus — Network-Based Clustering Plugin for QGIS
![icon](https://github.com/user-attachments/assets/755af5aa-8d93-496f-8d26-aec842f3d130)

[QGIS](https://img.shields.io/badge/QGIS-3.x-green.svg)
![License](https://img.shields.io/badge/license-GPL--2.0--or--later-blue)

**NetClus** is a QGIS plugin for performing *spatial clustering* based on **road network distance**, not Euclidean distance. It supports both small and large datasets (>1,000 features) using a hybrid approach (**KMeans + Graph-based Agglomerative Clustering**) and includes an *optional maximum distance constraint* within clusters.

---

## ✨ Key Features

- Clustering based on road network travel distance (instead of straight-line/Euclidean distance)
- **Direct Agglomerative** mode for small datasets
- **Hybrid Mode**: `KMeans → Agglomerative` for large datasets
- Optional **Max Distance Constraint** to limit the distance between cluster members
- Supports **point** and **polygon** input (polygon centroids are automatically used)
- Output is added directly to QGIS and can be exported to shapefile (`.shp`)

---

## 🧩 How to Use

1. Open QGIS and activate the **NetClus** plugin from the Plugin Manager.
2. Select input layers:
   - **Point / Polygon Layer**: features to be clustered (e.g., houses, facilities, schools, etc.)
   - **Road Network Layer**: must be a *LineString* vector layer
3. Choose the number of clusters or enable the `Max Distance` option.
4. Click **"Start Clustering"**.
5. The result will be added to the QGIS map as a new layer named `Clustering_Result`.

---

## 🛠️ Dependencies

- Python ≥ 3.7
- QGIS ≥ 3.16
- Libraries: `networkx`, `numpy`, `scipy`, `pandas`, `scikit-learn`, `shapely`, `tqdm`

---

## 📄 License

**GNU General Public License v2.0 or later**  
Copyright (C) 2025 — Surya Hafizh

---

## 🤝 Contributing

Pull requests are welcome.  
Feel free to report bugs, feature suggestions, or ideas via the [Issues tab](https://github.com/your-username/netclus/issues).

---

## 👤 Developer

**Surya Hafizh**  
📧 suryahafizh979@gmail.com  
📍 Department of Geography, Faculty of Social Sciences, Universitas Negeri Padang  

This plugin was developed to support real-world **network-based spatial analysis**, with applications in:
- Public facility planning
- Service delivery optimization
- Disaster mitigation using road network topology

