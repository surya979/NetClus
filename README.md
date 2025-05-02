# NetClus Plugin for QGIS

[QGIS](https://img.shields.io/badge/QGIS-3.x-green.svg)
![License](https://img.shields.io/badge/license-GPL--2.0--or--later-blue)

**NetClus** adalah plugin QGIS untuk melakukan *clustering spasial* berdasarkan **jaringan jalan**, bukan jarak Euclidean. Plugin ini mendukung data besar (>1.000 fitur) dengan pendekatan hybrid (KMeans + Agglomerative Clustering berbasis graph), serta mendukung batasan jarak maksimal antar elemen dalam klaster (*optional max distance*).

---

## ✨ Fitur Utama

- Clustering spasial berdasarkan jarak tempuh jaringan jalan (bukan jarak lurus)
- Mode **Agglomerative langsung** untuk data kecil
- Mode **Hybrid** (KMeans → Agglomerative) untuk data besar
- Opsi **Max Distance Constraint** untuk membatasi jarak maksimal dalam satu klaster
- Mendukung input point atau polygon (polygon otomatis diambil centroid-nya)
- Hasil bisa langsung ditampilkan di QGIS dan diekspor sebagai shapefile

---

## 🧩 Cara Menggunakan

1. Buka QGIS dan aktifkan plugin NetClus
2. Pilih:
   - **Layer Titik/Polygon** (misalnya lokasi rumah, fasilitas, dll)
   - **Layer Jaringan Jalan** (harus berupa *LineString*)
3. Pilih jumlah klaster atau aktifkan opsi `Max Distance`
4. Klik tombol **"Start Clustering"**
5. Hasil ditampilkan sebagai layer baru bernama `Clustering_Result`

---
