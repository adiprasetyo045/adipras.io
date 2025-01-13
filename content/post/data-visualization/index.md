---
title: "Cara Mudah Membuat Visualisasi Data Interaktif"
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
date: 2025-01-13
tags:
  - data
  - visualization
---

## Visualisasi Data

Visualisasi data adalah cara yang bagus untuk membuat data lebih mudah dipahami. Di sini, kita akan belajar cara menampilkan data menggunakan **grafik interaktif** dengan Plotly dan **diagram** dengan Mermaid di Hugo.

## Charts

Plotly adalah alat untuk membuat grafik yang interaktif, seperti grafik batang, garis, atau lingkaran. Ikuti langkah-langkah berikut untuk membuat grafik:

1. **Buat Grafik**  
   Gunakan Plotly untuk membuat grafik. Simpan grafiknya dalam file JSON, misalnya `grafik-bar.json`.

2. **Tambahkan Grafik ke Halaman**  
   Tempatkan file JSON di folder halaman dan gunakan kode berikut untuk menampilkan grafik:

   ```go
   {{</* chart data="grafik-bar.json" */>}}


## Diagrams

Hugo Blox supports the _Mermaid_ Markdown extension for diagrams.

Contoh **flowchart**:

 graph TD
A[Mulai] --> B{Keputusan}
B -->|Ya| C[Tugas 1]
B -->|Tidak| D[Tugas 2]
C --> E[Selesai]
D --> E

 ## sequenceDiagram
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
classDiagram
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
 ## tabel nilai 
Nama,Nilai,Grade
Alice,85,A
Bob,78,B
Charlie,92,A
{{</* table path="data.csv" header="true" caption="Tabel Nilai Siswa" */>}}