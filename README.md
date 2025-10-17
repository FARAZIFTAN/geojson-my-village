# 🗺️ Peta Jaringan Jalan Desa Nangalili (Tugas Praktek GeoJSON)

Repositori ini berisi data jaringan jalan dan gang di **Desa Nangalili** (isi: [Ganti: Nama Kabupaten Anda]), disimpan dalam format **GeoJSON**.

Data dibuat sebagai tugas praktek untuk mata kuliah/pelajaran [Ganti: Nama Mata Kuliah/Pelajaran] dan mengikuti standar pertukaran data geografis.
---

## 💾 Detail Data GeoJSON

**File Utama:** `village_road.geojson`

| Deskripsi | Detail |
| :--- | :--- |
| **Tipe GeoJSON** | `FeatureCollection` |
| **Tipe Geometri** | `LineString` (Merepresentasikan garis jalan/gang) |
| **Jumlah Fitur** | **[Ganti: Tulis jumlah total jalan/gang yang Anda buat, idealnya 30]** |
| **Sistem Koordinat** | $\text{WGS } 84$ ($\text{Longitude, Latitude}$) |

### Struktur Properti (`properties`)

Setiap fitur jalan (`Feature`) memiliki atribut non-spasial di dalam objek $\text{JSON}$. Tambahkan atau sesuaikan properti bila diperlukan:
| Kunci (Key) | Deskripsi | Contoh Nilai |
| :--- | :--- | :--- |
| `name` | Nama jalan atau gang. | "Jalan Utama Nangalili" |
| `category` | Kategori atau tipe jalan (mis. "Jalan Desa"). | "Jalan Desa", "Jalan Penghubung" |
| `length_m` | Panjang jalan (perkiraan) dalam meter. | 550 |

---

## ✨ Verifikasi dan Visualisasi Online (GeoJSON.io)


> Catatan: Jika Anda belum memastikan validitas file `village_road.geojson`, saya bisa melakukan pemeriksaan (lint/validasi) dan menghitung jumlah fitur.

Data GeoJSON ini dapat dibuka secara interaktif di geojson.io untuk pemeriksaan cepat tanpa harus mengunduh file.

**Tautan tampilan:**

https://geojson.io/#data=https://raw.githubusercontent.com/FARAZIFTAN/geojson-my-village/refs/heads/main/village_road.geojson


---

## 🚀 Langkah Akhir: Penyimpanan Basis Data MongoDB

Data ini siap untuk disimpan ke basis data spasial, misalnya MongoDB.

- Contoh: impor data ke basis data **MongoDB**.
- Untuk kueri spasial yang efisien, buat index **2dsphere** pada field `"geometry"` di collection yang menyimpan fitur.


