# Implementasi Basic Information Retrieval (Boolean Model)

Repository ini berisi tugas praktikum mata kuliah **Sistem Temu Kembali Informasi (Information Retrieval)**. Proyek ini mendemonstrasikan cara kerja dasar mesin pencari menggunakan algoritma **Boolean Retrieval Model** dan **Inverted Index**.

Selain mengikuti panduan tutorial standar, repository ini juga menyertakan eksperimen mandiri menggunakan dataset kustom (kalimat Bahasa Indonesia) untuk menguji fleksibilitas algoritma.

## Struktur Repository

* **`basic_IR_booleanModel.ipynb`**: Notebook utama yang berisi implementasi sesuai dengan panduan tutorial (studi kasus kalimat Bahasa Inggris: "Cow/Tuesday").
* **`custom_boolean_model.ipynb`**: Notebook tambahan berisi eksperimen mandiri. Pada file ini, logika algoritma yang sama diterapkan pada dataset kalimat Bahasa Indonesia untuk membuktikan pemahaman konsep.
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

4.  **Inverted Index (Indeks Terbalik)**:
    * Implementasi struktur data yang lebih efisien untuk memetakan kata ke ID dokumen.
    * Menghitung frekuensi kata (*Term Frequency*) dan membuat *Posting List*.

## Eksperimen & Pengembangan Mandiri

Pada file **`custom_boolean_model.ipynb`**, dilakukan uji coba algoritma menggunakan kalimat:
1.  *"Saya suka belajar pemrograman Python"*
2.  *"Python adalah bahasa pemrograman yang populer"*
3.  *"Saya belajar Python di VSCode menggunakan WSL"*

Hasil eksperimen menunjukkan bahwa sistem berhasil melakukan tokenisasi dan pencarian (query) dengan akurat pada input bahasa yang berbeda, membuktikan bahwa logika Boolean Retrieval bersifat universal terhadap karakter teks.

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
*Dibuat untuk memenuhi tugas Sistem Temu Kembali Informasi.*
