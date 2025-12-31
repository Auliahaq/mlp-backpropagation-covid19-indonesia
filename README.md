# Prediksi Kasus Aktif COVID-19 Indonesia Menggunakan MLP Backpropagation

Proyek ini merupakan tugas mata kuliah **Jaringan Saraf Tiruan** yang
mengimplementasikan **Multilayer Perceptron (MLP)** dengan algoritma
**Backpropagation** dan **Adam Optimizer (manual)** untuk memprediksi
kasus aktif COVID-19 di Indonesia berbasis data time series.

## Dataset
- COVID-19 Indonesia Time Series Dataset
- Sumber: Kaggle (Hendratno)
- Fokus data: agregat nasional (Location = Indonesia)

Link dataset:
https://www.kaggle.com/datasets/hendratno/covid19-indonesia

## Metodologi
- Tipe data: Time Series (univariate)
- Lag window: 7 hari
- Normalisasi: Min-Max Scaling
- Split data: Chronological
  - Train: 70%
  - Validation: 15%
  - Test: 15%

## Arsitektur Model
- Input layer: 7 neuron
- Hidden layer 1: 32 neuron (ReLU)
- Hidden layer 2: 16 neuron (ReLU)
- Output layer: 1 neuron (Linear)
- Loss function: MSE
- Optimizer: Adam (manual implementation)

## Evaluasi
- MAE ≈ 600 kasus
- RMSE ≈ 867 kasus
- Model mampu mengikuti tren naik-turun kasus aktif dengan baik
  tanpa indikasi overfitting yang signifikan.

## Tools
- Python
- NumPy
- Pandas
- Google Colab

## Authors
- Aulia Haq
- Aurelia Salsabilla Yunanto Putri
- Rania Putri Zayyanti

## Catatan
Proyek ini dibuat untuk keperluan akademik dan pembelajaran.
