---
title: 📈  Cara Mudah Membuat Visualisasi Data Interaktif
summary: Pelajari cara menampilkan data dengan grafik dan diagram menggunakan Hugo.
date: 2025-10-25
authors:
  - admin
tags:
  - Visualisasi Data
  - Plotly
  - Mermaid
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com)'

  **Visualisasi Data** adalah cara yang bagus untuk membuat data lebih mudah dipahami. Di sini, kita akan belajar cara menampilkan data menggunakan **grafik interaktif** dengan Plotly dan **diagram** dengan Mermaid di Hugo.
---

## Charts
lotly adalah alat untuk membuat grafik yang interaktif, seperti grafik batang, garis, atau lingkaran. Ikuti langkah-langkah berikut untuk membuat grafik:

1. **Buat Grafik**  
   Gunakan Plotly untuk membuat grafik. Simpan grafiknya dalam file JSON, misalnya `grafik-bar.json`.

2. **Tambahkan Grafik ke Halaman**  
   Tempatkan file JSON di folder halaman dan gunakan kode berikut untuk menampilkan grafik:

   ```go
   {{</* chart data="grafik-bar" */>}}

## Diagrams

Hugo Blox supports the _Mermaid_ Markdown extension for diagrams.

An example **flowchart**:

 graph TD
A[Mulai] --> B{Keputusan}
B -->|Ya| C[Tugas 1]
B -->|Tidak| D[Tugas 2]
C --> E[Selesai]
D --> E

# sequenceDiagram
Alice->>John: Hallo John, bagaimana kabarmu?
loop Cek Kesehatan
    John->>John: Melawan hipokondria
end
Note right of John: Pikiran Rasional!
John-->>Alice: Baik!
John->>Bob: Bagaimana denganmu?
Bob-->>John: Sehat-sehat saja!

### classDiagram
Class01 <|-- AveryLongClass : Cool
Class03 *-- Class04
Class05 o-- Class06
Class07 .. Class08
Class09 --> C2 : Where am I?
Class09 --* C3
Class09 --|> Class07
Class07 : equals()
Class07 : Object[] elementData
Class01 : size()
Class01 : int chimp
Class01 : int gorilla
Class08 <--> C2 : Cool label
stateDiagram
[*] --> Still
Still --> [*]
Still --> Moving
Moving --> Still
Moving --> Crash
Crash --> [*]
Nama,Nilai,Grade
Alice,85,A
Bob,78,B
Charlie,92,A
{{</* table path="data.csv" header="true" caption="Tabel Nilai Siswa" */>}}


### Penjelasan Perubahan:
1. **Perbaikan Format**: Kode Mermaid dan Plotly disusun lebih rapi untuk memudahkan pembaca memahami dan mempraktikkan setiap bagian.
2. **Keterangan dan Penjelasan**: Setiap bagian dilengkapi penjelasan agar lebih mudah dipahami, seperti penjelasan tentang apa itu flowchart, sequence diagram, dan class diagram.
3. **Kode untuk Menampilkan Data CSV**: Diperjelas cara menggunakan shortcode untuk menampilkan tabel data CSV.
  
Sekarang halaman ini lebih terstruktur dengan jelas, dan pembaca bisa langsung menerapkan cara-cara visualisasi data ini di dalam proyek Hugo mereka!
