# Proyek Akhir Analisis Data: Bike Sharing dan Dashboard

# Analisis dilakukan di Google Collaboratory

Proyek Akhir Analisis Data Bike Sharing dapat dilihat selengkapnya di tautan berikut <a href='https://github.com/adinplb/Proyek_Analisis_Data_Dicoding/blob/main/notebook.ipynb'>Bike Sharing Analysis</a>

## Mendefinisikan Pertanyaan

1. Apa efek dari pergantian musim terhadap tingkat penyewaan sepeda?
2. Bagaimana kondisi cuaca berdampak pada jumlah orang yang menyewa sepeda?
3. Adakah perbedaan signifikan antara jumlah penyewaan oleh pelanggan biasa dan pelanggan yang sudah terdaftar?

# Menyiapkan Semua Library Yang Dibutuhkan

- import pandas as pd
- import plotly.express as px
- import warnings

## Data Wrangling:

- Gathering data
- Assessing data (Cek Tipe Data, Cek Missing Value, Cek Duplikasi Data, Deskripsif Statistics)
- Cleaning data

## Exploratory Data Analysis (Insights and Findings):

1. Dataset Hari (Day)

- Jumlah data(count): 731 rekaman data.
- Musim: Rata-rata berada di sekitar musim panas (season 2).
- Tahun: Paling sering muncul di tahun 2012 (yr = 1).
- Bulan: Rata-rata bulan adalah sekitar 6.52 berarti berada di bulan Juli (mnth 7).
- Hari Libur: Rata-rata menunjukkan sekitar 2.87% hari adalah hari libur.
- Hari dalam Seminggu: Rata-rata hari adalah sekitar 2.997, mendekati pertengahan minggu.
- Hari Kerja: Rata-rata menunjukkan sekitar 68.40% hari adalah hari kerja.
- Situasi Cuaca: Rata-rata cuaca adalah sekitar 1.395, menunjukkan mayoritas cuaca adalah cerah hingga berawan.
- Suhu: Rata-rata suhu adalah sekitar 0.495.
- Suhu Terasa: Rata-rata suhu terasa adalah sekitar 0.474.
- Kelembapan: Rata-rata kelembapan adalah sekitar 0.628.
- Kecepatan Angin: Rata-rata kecepatan angin adalah sekitar 0.19.
- Pengguna Kasual: Rata-rata pengguna kasual adalah sekitar 848.
- Pengguna Terdaftar: Rata-rata pengguna terdaftar adalah sekitar 3656.
- Jumlah Total Penyewaan: Rata-rata jumlah penyewaan sepeda adalah sekitar 4504 /hari.

2. Dataset Jam (Hour)

- Jumlah data(count): 17379 rekaman data.
- Musim: Rata-rata berada di sekitar musim panas (season 2).
- Tahun: Paling sering muncul di tahun 2012 (yr = 1).
- Bulan: Rata-rata bulan adalah sekitar 6.54 berarti berada di bulan Juli (mnth 7).
- Jam: Rata-rata jam adalah sekitar 11.55, menunjukkan bahwa data terkumpul sepanjang hari.
- Hari Libur: Rata-rata menunjukkan sekitar 2.88% hari adalah hari libur.
- Hari dalam Seminggu: Rata-rata hari adalah sekitar 3.00, mendekati pertengahan minggu.
- Hari Kerja: Rata-rata menunjukkan sekitar 68.3% jam adalah pada hari kerja.
- Situasi Cuaca: Rata-rata cuaca adalah sekitar 1.43, menunjukkan mayoritas cuaca adalah cerah hingga berawan.
- Suhu: Rata-rata suhu adalah sekitar 0.497 (setelah dikonversi menjadi sekitar 20.37°C).
- Suhu Terasa: Rata-rata suhu terasa adalah sekitar 0.476 (setelah dikonversi menjadi sekitar 23.79°C).
- Kelembapan: Rata-rata kelembapan adalah sekitar 0.627 (setelah dikonversi menjadi sekitar 62.72%).
- Kecepatan Angin: Rata-rata kecepatan angin adalah sekitar 0.19.
- Pengguna Kasual: Rata-rata pengguna kasual adalah sekitar 35.68.
- Pengguna Terdaftar: Rata-rata pengguna terdaftar adalah sekitar 153.79.
- Jumlah Total Penyewaan: Rata-rata jumlah penyewaan sepeda adalah sekitar 189.46.

## Visualization and Explanatory Analysis:

- Musim Gugur dan Musim Panas memimpin penyewaan sepeda, menunjukkan bahwa cuaca hangat meningkatkan minat masyarakat untuk menyewa.
- Visualisasi data menunjukkan penyewaan sepeda lebih tinggi saat cuaca cerah, menegaskan pengaruh cuaca terhadap jumlah penyewaan.
- Pengguna kasual cenderung menyewa sepeda pada akhir pekan atau hari libur, sedangkan pengguna terdaftar lebih sering menyewa sepeda pada hari kerja.

# Dashboard with Streamlit:

## Run Streamlit on Local

### Intall Dependencies

To install all the required libraries, open your terminal/command prompt/conda prompt, navigate to this project folder, and run the following command:
pip install -r requirements.txt
pip install streamlit

### Run Dashboard

Mengarahkan pathnya ke direktori file py dan dataset hour.csv nya dengan command cd dashboard pada Anaconda Prompt

Setelah berhasil, tuliskan perintah berikut streamlit run dashboard_streamlit_muhammad_adin_palimbani.py untuk mendapatkan link localhostnya
