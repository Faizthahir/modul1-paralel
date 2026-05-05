# 📊 Laporan Modul 1 - Eksplorasi Paralelisme Dasar

## 🧑‍🎓 Informasi Mahasiswa

* **Nama:** Fa’iz Thahir Nasution
* **NIM:** 24343035
* **Mata Kuliah:** Komputasi Paralel dan Terdistribusi

---

## 📌 Deskripsi Project

Project ini merupakan implementasi perbandingan antara program **serial** dan **paralel (multiprocessing)** dalam menghitung nilai π (pi).

Tujuan utama dari praktikum ini adalah untuk menganalisis:

* Waktu eksekusi program
* Speedup yang dihasilkan
* Efisiensi paralelisme
* Dampak overhead terhadap performa sistem

---

## ⚙️ Teknologi yang Digunakan

* Python
* Jupyter Notebook (`.ipynb`)
* Library:

  * `multiprocessing`
  * `time`
  * `math`

---

## 🚀 Cara Menjalankan Program

1. Pastikan Python sudah terinstall (disarankan menggunakan Miniconda / Anaconda)
2. Jalankan Jupyter Notebook:

   ```bash
   jupyter lab
   ```
3. Buka file `.ipynb`
4. Jalankan semua cell (Run All)

---

## 📈 Hasil Pengujian

### 🔹 Program Serial

* Waktu eksekusi: ± 0.2199 detik
* Hasil π: 3.141592653589793

### 🔹 Program Paralel (Multiprocessing)

| Jumlah Proses | Waktu (detik) | Speedup | Efficiency |
| ------------- | ------------- | ------- | ---------- |
| 1             | 2.4212        | 0.0908  | 0.0908     |
| 2             | 1.3228        | 0.1662  | 0.0831     |
| 4             | 0.9092        | 0.2418  | 0.0806     |
| 8             | 0.6619        | 0.3322  | 0.0415     |
| 16            | 0.5922        | 0.3713  | 0.0232     |
| 32            | 0.6104        | 0.3602  | 0.0112     |

---

## 📊 Analisis Singkat

Hasil menunjukkan bahwa program paralel tidak selalu lebih cepat dibandingkan program serial. Hal ini disebabkan oleh adanya overhead seperti:

* pembuatan proses
* komunikasi antar proses
* context switching

Selain itu, ukuran masalah yang kecil menyebabkan keuntungan paralelisme tidak optimal.

---

## 📉 Kesimpulan

Paralelisme tidak selalu menghasilkan peningkatan performa. Efektivitasnya sangat bergantung pada:

* ukuran data
* jumlah proses
* dan overhead sistem

Untuk kasus ini, program serial justru lebih efisien dibandingkan paralel.
