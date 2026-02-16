# Implementasi Basic Information Retrieval (Boolean Model)

Repository ini berisi tugas praktikum mata kuliah **Sistem Temu Kembali Informasi (Information Retrieval)**. Proyek ini mendemonstrasikan cara kerja dasar mesin pencari menggunakan algoritma **Boolean Retrieval Model**.

## Struktur Repository

* **`basic_IR_booleanModel.ipynb`**: Notebook utama yang berisi kode program Python untuk simulasi sistem temu kembali informasi.
* **`.gitignore`**: Konfigurasi agar file sampah (seperti folder virtual environment) tidak ikut ter-upload.

## Konsep yang Dipelajari

Notebook dalam repository ini mencakup implementasi dari konsep-konsep berikut:

1.  **Preprocessing Teks**:
    * Tokenisasi kalimat menjadi kata-kata.
    * Ekstraksi kata unik (*unique terms*) dari korpus dokumen.

2.  **Term-Document Incidence Matrix**:
    * Membuat matriks biner (0 dan 1) untuk memetakan apakah sebuah kata muncul dalam dokumen tertentu.
    * Menggunakan library `pandas` untuk visualisasi matriks.

3.  **Boolean Retrieval Model**:
    * Melakukan query pencarian sederhana menggunakan logika Boolean (`AND`, `OR`, `NOT`).
    * Contoh kasus: Mencari dokumen yang mengandung kata "cow" **TAPI TIDAK** mengandung kata "tuesday".

4.  **Inverted Index (Indeks Terbalik)**:
    * Implementasi struktur data yang lebih efisien untuk memetakan kata ke ID dokumen.
    * Menghitung frekuensi kata (*Term Frequency*) dan membuat *Posting List*.

## Teknologi yang Digunakan

* **Python 3**
* **Pandas** (Untuk manipulasi data tabel)
* **NumPy** (Untuk operasi vektor matematika)
* **Jupyter Notebook** (Dijalankan di VSCode via WSL/Ubuntu)

## Referensi & Acknowledgements

Proyek ini dikerjakan dengan mengikuti panduan dan referensi kode dari:

* **Artikel**: [Basic Information Retrieval Problem — Boolean Retrieval Model](https://bajpaihimanshu.medium.com/basic-information-retrieval-problem-boolean-retrieval-model-ed05f3d74ddc) oleh Himanshu Bajpai.
* **Repository Asli**: [DataScienceProjects](https://github.com/HimanshuBajpai869/DataScienceProjects) oleh Himanshu Bajpai.

---
*Dibuat untuk memenuhi tugas Information Retrieval.*
