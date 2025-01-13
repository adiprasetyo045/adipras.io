---
title: "Visualisasi Data dengan ggplot2"
authors:
- adi prasetyo
date: "2025-04-07T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2025-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["tutorial"]

# Publication name and optional abbreviated publication name.
publication: "Tutorial Visualisasi Data"
publication_short: "Tutorial ggplot2"

abstract: Paket ggplot2 dalam R menyediakan kerangka kerja yang kuat untuk membuat berbagai jenis grafik dengan cara yang elegan dan terstruktur. Tutorial ini membahas dasar-dasar visualisasi data menggunakan ggplot2, mulai dari membuat grafik dasar hingga kustomisasi tingkat lanjut.

# Summary. An optional shortened abstract.
summary: Tutorial ini membahas konsep visualisasi data menggunakan ggplot2 di R, termasuk pembuatan grafik dasar, kustomisasi, dan contoh penggunaan.

tags:
- Data Visualization
- ggplot2
- R Programming

featured: true

links:
- name: Dokumentasi ggplot2
  url: https://drive.google.com/file/d/1Yvd09aRp1ZyIg0rhciL_4vAbzopJBou3/view?usp=drive_link
url_pdf: '#'
url_code: 'https://github.com/adiprasetyo045/dataviz_ggplot.git'
url_dataset: '#'
url_poster: '#'
url_project: ''
url_slides: ''
url_source: '#'
url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- internal-project

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ggplot2-tutorial
---

## Pengantar ggplot2
Paket **ggplot2** adalah bagian dari tidyverse yang dirancang untuk membuat visualisasi data dengan cara yang konsisten dan intuitif. Dengan menggunakan prinsip *grammar of graphics*, ggplot2 memungkinkan pengguna untuk membangun grafik melalui lapisan-lapisan visualisasi.

### Cara Menggunakan ggplot2
Untuk menggunakan ggplot2, pastikan Anda telah menginstalnya di R:
```r
install.packages("ggplot2")
library(ggplot2)

# Scatterplot dengan ggplot2
ggplot(data = mtcars, aes(x = wt, y = mpg)) +
  geom_point(color = "blue") +
  labs(title = "Hubungan Berat Kendaraan dan Konsumsi BBM",
       x = "Berat Kendaraan (1000 lbs)",
       y = "Konsumsi BBM (mpg)")
# Scatterplot dengan garis regresi
ggplot(data = mtcars, aes(x = wt, y = mpg)) +
  geom_point(color = "blue") +
  geom_smooth(method = "lm", color = "red", se = FALSE) +
  labs(title = "Hubungan Berat Kendaraan dan Konsumsi BBM dengan Garis Regresi",
       x = "Berat Kendaraan (1000 lbs)",
       y = "Konsumsi BBM (mpg)")
# Scatterplot dengan tema minimal
ggplot(data = mtcars, aes(x = wt, y = mpg)) +
  geom_point(color = "blue") +
  theme_minimal() +
  labs(title = "Hubungan Berat Kendaraan dan Konsumsi BBM (Tema Minimal)",
       x = "Berat Kendaraan (1000 lbs)",
       y = "Konsumsi BBM (mpg)")
#Kesimpulan
        Paket ggplot2 memberikan fleksibilitas tinggi dalam membuat visualisasi data yang menarik dan informatif. Dengan memahami konsep dasar dan kustomisasi lebih lanjut, Anda dapat membuat grafik yang sesuai dengan kebutuhan analisis data Anda.

        Konten di atas memberikan penjelasan dasar tentang **visualisasi data dengan ggplot2** beserta contoh kode. Anda dapat menyesuaikannya sesuai dengan kebutuhan atau menambahkan materi lebih lanjut jika diperlukan. 😊
