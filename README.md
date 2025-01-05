# Analisis Popularitas Lagu Spotify Berdasarkan Karakteristik Musik dan Preferensi Playlist

Semua asset dan asset dapat diakses dari Github ini, Apabila dataset tidak tertera bisa diakses melalui [LINK](https://www.dropbox.com/sh/qj0ueimxot3ltbf/AACzMOHv7sZCJsj3ErjtOG7ya?dl=1)

<div align="center">
  <img src="https://github.com/user-attachments/assets/48633f16-3793-4dec-b2ae-283c28ef1dc3" alt="Spotify Big data" width="480">
</div>

## Langkah-langkah Analisis Data

1. Instalasi Java Development Kit (JDK)
   ```
   !apt-get install openjdk-8-jdk-headless -qq > /dev/null
   ```
2. Unduh Apache Spark Versi 3.5.1 dengan dukungan Hadoop 3
   ```
   !wget -q http://archive.apache.org/dist/spark/spark-3.5.1/spark-3.5.1-bin-hadoop3.tgz
   ```
3. Ekstrak File Spark
   ```
   !tar xf spark-3.5.1-bin-hadoop3.tgz
   ```
4. Instal Library Spark
   ```
   !pip install -q findspark
   ```
5. (Optional) Verifikasi Spark
   ```
   !tar xf spark-3.5.1-bin-hadoop3.tgz
   ``` 
## Daftar isi
- [Pendahuluan](#pendahuluan)
- [Alur Penelitian](#alur-penelitian)
- [Kesimpulan](#kesimpulan)
## Pendahuluan
Musik adalah salah satu hiburan yang sangat diminati oleh banyak orang, saat ini banyak plaform digital yang telah memberi pelayanan untuk kita memutar musik sesuai dengan selera dan bahkan memberikan rekomendasi berdasarkan lagu yang sering kita putar. Dari waktu ke waktu genre musik semakin berkembang, sebagai contoh, di beberapa tahun lalu hanya terdapat Pop, Classic, Rock, dan lain sebagainya namun di era kini terdapat banyak genre lain seperti Accoustic, Edm, Post Rock dan Lain sebagainya. Oleh karena itu tidak bisa dipungkiri apabia terdapatnya campur tangan _Machine Learning_ dalam hal ini agar dapat memproses data-data lagu yang ada pada suatu Platform, sebagai contoh Spotify.

## Alur Penelitian
- Library

  Import Library yang Diperlukan
  Sebagai contoh dibawah
```
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import numpy as np
```
- Preprocessing dan EDA

  Untuk menghindari adanya null data(data yang kosong), data yang rusak, Missing Values dan lain sebagainya, tidak lupa juga dilakukan EDA (Exploratory Data Anlysis) proses ini dilakukan untuk mencari berbagai      wawasan maupun informasi tentng dataset secara keseluruhan. Sebagai contoh seperti distribusi setiap kelas, kolerasi antar kelas, Informasi tipe data dan lain sebagainya

  <img width="480" alt="BigData#1" src="https://github.com/user-attachments/assets/51b7271e-5712-4e0e-8fd8-49bc7983e196" />
  <img width="480" alt="BigData#2" src="https://github.com/user-attachments/assets/6ea9f266-92b7-4ab3-a6dd-b6c20af010a4" />

- Splitting Data, Modeling and Model Training

  Proses ini adalah proses dimana kita melakukan splitting atau pemisahan data menjadi Data Latih dan Data Uji menjadi beberapa rasio seperti contoh 80:20.
  Proses selanjutnya yaitu Modelling atau membuat model, model dibuat berdasarkan informasi atau wawasan yang kita dapat setelah kita melakukan EDA dan Model akan disesuakan kembali dengan data yang akan Di Latih.
  Setelah Splitting dan Modeling dilakukan, Data akan diuji dan akan diketahui bagaimana model atau algoritman yang kita pakai memproses Data tersebut
  
  <img width="320" alt="BigData#4" src="https://github.com/user-attachments/assets/db23a97d-11aa-4595-95d7-830606202a2d" />
  <img width="320" alt="BigData#5" src="https://github.com/user-attachments/assets/b451d3b2-fc57-4b52-9915-ab003befb53c" />

- Evaluation

  Proses Evaluasi dilakukan untuk melihat kembali hail train dari model mulai dari melihat Classification Report, Confussion Matrix, Learning Curves dan lain sebagainya. Hal ini sangat penting dilakukan agar kita dapat mengetahui pola-pola Machine Learning dalam melakukan train, kita juga dapat melihat beberapa kelebihan dan kelemahan pada setiap model yang digunakan sehingga kita bisa mendapatkan informasi yang diperlukan dan digunakan untuk memperbaiki model, maupun bagian lain agar model dapat bekerja lebih optimal.

## Kesimpulan

Data Spotify yang telah diteliti memberikan wawasan yang dapat diterjemahkan menjadi aksi nyata untuk meningkatkan keterlibatan pengguna. Analisis karakteristik lagu populer, sistem rekomendasi personal, dan playlist tematik turut membantu dalam memenuhi kebutuhan audiens, sementara segmentasi audiens memungkinkan penyusunan kampanye pemasaran yang lebih relevan dan efektif. Penelitian ini masih kurang dari kata sempurna sehingga diharapkan untuk di waktu kedepan diadakan penelitian yang dapat menyempurnakan dan memberikan informasi yang lebih dari penelitian yang telah dilakukan.
