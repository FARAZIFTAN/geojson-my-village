# Peta Jaringan Jalan Desa Nangalili (Tugas Praktek GeoJSON)

Repositori ini menyimpan data spasial jaringan jalan dan gang di Desa Nangalili yang disusun untuk keperluan tugas praktek mata kuliah Geo-Informatika. Data disimpan dalam format GeoJSON sesuai spesifikasi RFC 7946.

## Detail Data GeoJSON

- Tipe Utama: `FeatureCollection`.
- Jumlah Fitur: 30 (asumsi: dataset berisi 30 jalan/gang — jika jumlah sebenarnya berbeda, harap perbarui nilai ini).
- Tipe Geometri: `LineString` (poliline), digunakan untuk merepresentasikan segmen jalan/gang.
- Sistem Koordinat: WGS 84 (Longitude, Latitude), sesuai RFC 7946.

## Struktur Properti (properties)

Setiap objek `Feature` merepresentasikan satu jalan atau gang dan memiliki atribut non-spasial berikut:

- `name`: Nama resmi jalan atau gang.

Contoh nilai:

```
"name": "Jalan Utama Nangalili"
```

## Catatan dan Asumsi

- Jumlah fitur ditetapkan ke 30 berdasarkan instruksi tugas (asumsi ini dapat diubah setelah verifikasi data aktual di file GeoJSON).
- Pastikan setiap `Feature` memiliki properti `name` dan geometri `LineString` dengan koordinat dalam urutan [longitude, latitude].

Jika Anda ingin, saya bisa juga menghitung jumlah fitur secara otomatis dari file `village_road.geojson` dan mengganti nilai asumsi dengan jumlah yang akurat.

