# Smart Demand Forecasting for Beverage & Fresh Produce

## Deskripsi
Sistem Prediksi Penjualan & Kebutuhan Bahan Baku Berbasis ML ini dirancang untuk mengatasi masalah UMKM kuliner/minuman (seperti Usaha Jus Buah Segar) yang kesulitan memperkirakan stok bahan baku mentah yang mudah busuk. 

Solusi ini memproses data histori transaksi harian, tren hari, tanggal merah, serta faktor cuaca menggunakan algoritma Time Series Forecasting (seperti XGBoost atau Prophet) untuk mempredict jumlah porsi yang akan terjual. Hasilnya dikonversi menjadi rekomendasi kuantitas belanja bahan baku harian secara rinci guna mencegah overstock (bahan mentah terbuang) maupun understock (kehilangan penjualan).

## Struktur Project
* **`frontend/`**: Antarmuka dashboard manajemen inventaris untuk menampilkan rekomendasi belanja harian UMKM.
* **`backend/`**: REST API (FastAPI/Flask) yang menghubungkan model prediksi dengan dashboard dan database kasir (POS).
* **`model/`**: Kode pelatihan time-series, evaluasi matriks (MAE/RMSE), artefak model, serta skrip otomatisasi retraining.
* **`data/`**: Direktori data histori transaksi harian (`raw/`) dan data hasil preprocessing (`processed/`).
* **`tests/`**: Pengujian unit dan integrasi untuk memastikan keandalan pipeline data dan API backend.
* **`docs/`**: Laporan praktikum, rancangan alur kerja MLOps, dan dokumentasi teknis sistem.

## Tech Stack
* Language & Core: Python, Pandas, NumPy
* Machine Learning & Time Series: XGBoost, Prophet, Scikit-Learn
* Backend & API: FastAPI / Flask
* MLOps & Pipeline: Git, GitHub, Automated Retraining Pipeline
* Environment: Google Colab / Linux

## Team
Kelompok 11 - Sistem Informasi (Politeknik Caltex Riau)
* M Rizki Pradipta (NIM: 2357301070) - MLOps Engineer / Lead Developer
* Stevani Rosalinda (NIM: 2357301126) - Data & Business Analyst

Pembimbing:
* Dosen: Muhammad Mahrus Zain, S.S.T., M.T.I.
* PLP/ILB: Miftahul Huda, S.Tr.Kom

## Development Workflow
* Menggunakan fitur percabangan Git (feature/nama-fitur) untuk setiap pengembangan baru.
* Pesan commit dibuat bermakna (meaningful commit) sesuai perubahan kode.
* Penggabungan kode ke branch main dilakukan melalui Code Review dan verifikasi state.
