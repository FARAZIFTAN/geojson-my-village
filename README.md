# Data GeoJSON Desa Nangalili

Ini adalah berkas README yang menjelaskan data geografis (GeoJSON) untuk Desa Nangalili.

## 1. Ikhtisar Data

Berkas GeoJSON ini mendefinisikan jaringan jalan utama dan properti atribut untuk Desa Nangalili.

| Informasi                 | Deskripsi                                                                 |
|---------------------------|---------------------------------------------------------------------------|
| **Format Berkas**         | GeoJSON (`.geojson`)                                                     |
| **Sistem Referensi Koordinat (CRS)** | [Contoh: WGS 84 (EPSG: 4326)]                                        |
| **Cakupan Geografis**     | Jaringan jalan utama di Desa Nangalili, Kabupaten Manggarai Barat, NTT   |
| **Tujuan**                | Visualisasi, analisis spasial, dan pemetaan jaringan jalan desa          |

## 2. Struktur Berkas

Berkas utama data ini adalah:

| Nama Berkas              | Deskripsi                                                                 |
|--------------------------|---------------------------------------------------------------------------|
| `village_road.geojson`   | Berkas GeoJSON yang berisi geometri (garis) dan atribut data untuk jalan desa |

## 3. Isi Data (Atribut)

Setiap fitur (garis) dalam berkas GeoJSON memiliki properti atribut yang memberikan informasi tambahan mengenai jaringan jalan tersebut.

| Nama Atribut (Key) | Tipe Data | Deskripsi                              | Contoh Nilai                     |
|--------------------|-----------|----------------------------------------|-----------------------------------|
| `name`            | String    | Nama jalan                            | Jalan Desa Nangalili             |
| `description`     | String    | Deskripsi jalan                       | Jaringan jalan utama di Desa Nangalili |
| `category`        | String    | Kategori geometri                     | LineString                       |

[**Atribut Tambahan**] | [**Tipe Data**] | [**Deskripsi Atribut Tambahan**] | [**Nilai Contoh**]