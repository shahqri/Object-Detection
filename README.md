# Object-Detection
# ♻️ SmartVision AI – Recyclable Material Classification

## 📌 Pengenalan

**SmartVision AI** ialah aplikasi berasaskan Artificial Intelligence (AI) yang dibangunkan untuk mengenal pasti dan mengelaskan bahan kitar semula berdasarkan imej.

Sistem menggunakan **Google Teachable Machine** untuk melatih model **Image Classification** dengan tiga kategori bahan kitar semula:

* 🧴 Plastic Bottle
* 📦 Paper / Cardboard
* 🥫 Aluminium Can

Model yang telah dilatih kemudiannya diintegrasikan ke dalam aplikasi supaya pengguna boleh memberikan input melalui **imej atau webcam** dan mendapatkan keputusan klasifikasi bersama **confidence score**.

## 🎯 Objektif Projek

1. Membangunkan model AI Image Classification untuk mengenal pasti tiga kategori bahan kitar semula.
2. Menguji model menggunakan imej baharu dan menilai keputusan prediction serta confidence score.
3. Membangunkan aplikasi yang membolehkan pengguna mengesan objek menggunakan webcam untuk mendapatkan keputusan klasifikasi.

## ♻️ Kelas Bahan Kitar Semula

| Kelas                | Contoh                      |
| -------------------- | --------------------------- |
| 🧴 Plastic Bottle    | Botol air dan botol plastik |
| 📦 Paper / Cardboard | Kertas dan kotak            |
| 🥫 Aluminium Can     | Tin minuman aluminium       |

## ⚙️ Fungsi Sistem

* 📹 **Webcam** – Pengguna boleh memberikan input melalui kamera.
* 🤖 **AI Prediction** – Model AI menganalisis imej yang diberikan.
* 📊 **Confidence Score** – Sistem memaparkan tahap keyakinan prediction.
* 🏷️ **Class Result** – Sistem memaparkan kategori bahan yang dikenal pasti.
* 🔄 **Reset** – Pengguna boleh membuat prediction baharu.

## 🧠 Teknologi Yang Digunakan

* Artificial Intelligence (AI)
* Image Classification
* Neural Network / CNN
* Google Teachable Machine
* TensorFlow.js
* HTML
* Visual Studio Code
* GitHub

Model digunakan secara **client-side melalui TensorFlow.js**, jadi versi semasa tidak memerlukan backend Python untuk menjalankan inferens.

## 📊 Dataset

Dataset terdiri daripada tiga kelas bahan kitar semula:

| Kelas             | Dataset |
| ----------------- | ------: |
| Plastic Bottle    |  171 imej |
| Paper / Cardboard |  100 imej |
| Aluminium Can     |  95 imej |

Dataset mengambil kira variasi seperti:

* Sudut objek
* Jarak objek
* Pencahayaan
* Kedudukan objek
* Latar belakang

## 🏋️ Training Model

Model dilatih menggunakan **Google Teachable Machine Image Project**.

### Proses Training

```text
Kumpul & Susun Dataset
        ↓
Muat Naik ke Teachable Machine
        ↓
Latih Model
        ↓
Eksport Model
        ↓
Uji dengan Imej Baharu
        ↓
Integrasi ke Aplikasi
```

Model melalui sekurang-kurangnya dua eksperimen dengan perubahan pada dataset, variasi imej dan parameter latihan.

## 🔬 Eksperimen Model

### Eksperimen 1 – Model Asal

* Dataset: 366 imej/class
* Epoch: 50
* Batch Size: 16
* Learning Rate: 0.001

### Eksperimen 2 – Model Penambahbaikan

Penambahbaikan dibuat melalui:

* Penambahan jumlah imej
* Penambahan variasi latar belakang
* Penambahan variasi sudut
* Perubahan parameter training

## 🖥️ Aplikasi

Aplikasi menerima input daripada pengguna dan menjalankan proses prediction menggunakan model AI.

```text
Image / Webcam
      ↓
Input Image
      ↓
AI Model
      ↓
Image Classification
      ↓
Class Prediction
      ↓
Confidence Score
      ↓
Status Keputusan
```

## 📁 Struktur Projek

```text
Object-Detection/
│
├── model/
│   ├── model.json
│   └── metadata.json
│
├── images/
│   └── sample/
│
├── index.html
└──  README.md
```

> Struktur folder boleh disesuaikan mengikut fail sebenar dalam repository.

## 🚀 Cara Menjalankan Projek

### 1. Clone Repository

```bash
git clone https://github.com/shahqri/Object-Detection.git
```

### 2. Buka Fail Projek

Buka fail:

```text
Object-Detection.html
```

### 3. Jalankan Aplikasi


### 4. Berikan Input

* Gunakan webcam

Sistem akan memproses objek dan memaparkan kategori bahan serta confidence score.

## 🐙 GitHub

GitHub digunakan untuk:

* Menyimpan source code projek.
* Mengurus versi kod.
* Merekod commit ahli kumpulan.
* Mendokumentasikan pembangunan projek.

**Object-Detection**

## 🤖 AI Code Assistant

AI Code Assistant digunakan untuk membantu proses pembangunan seperti:

* Debugging kod.
* Refactoring fungsi.
* Menjana dokumentasi README.
* Membantu menyelesaikan masalah dalam fungsi prediction.

Semua kod yang dihasilkan menggunakan AI disemak, difahami dan diuji sebelum digunakan.

## ⚠️ Cabaran

Antara cabaran yang dihadapi semasa pembangunan:

* False positive dalam proses klasifikasi.
* Perbezaan pencahayaan dan latar belakang imej.
* Variasi sudut dan jarak objek.
* Ketepatan prediction model.

Penambahbaikan dibuat melalui penambahan dataset dan variasi imej serta pelarasan proses training.

## 🔮 Cadangan Penambahbaikan

* Menambah lebih banyak kelas bahan kitar semula.
* Menambah jumlah dan kepelbagaian dataset.
* Meningkatkan ketepatan model.
* Menambah fungsi pengesanan bahan yang tidak dikenali.
* Mengembangkan sistem kepada klasifikasi bahan kitar semula yang lebih menyeluruh.
  
Projek ini dibangunkan sebagai projek akademik untuk mengaplikasikan teknologi Artificial Intelligence, Computer Vision dan Image Classification dalam mengenal pasti kategori bahan kitar semula.
