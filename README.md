# 📱 Analisis Sentimen Aplikasi Canva (Google Play Store)

**Identitas Mahasiswa:**
* **Nama:** Terry Djong
* **NIM:** 14022300086

Proyek ini dibangunkan untuk menganalisis sentimen ulasan pengguna terhadap aplikasi **Canva** di Google Play Store sebagai bagian dari analisis Big Data.

## 🚀 Deskripsi Proyek
Proyek ini melakukan ekstraksi data (*web scraping*) ulasan Canva, memproses teks, dan mengklasifikasikan sentimen pengguna ke dalam kategori **Positif**, **Negatif**, atau **Netral**. Proses ini menggunakan model *Natural Language Processing* (NLP) berbasis RoBERTa. Hasil analisis kemudian divisualisasikan dalam bentuk grafik yang jelas dan mudah dipahami.

## 📂 Struktur File
* **`UTS_BIG_DATA_TERRY.ipynb`**: File utama Jupyter Notebook yang berisi kode untuk scraping ulasan, pemrosesan analisis sentimen, dan visualisasi data.
* **`ulasan_google_play.csv`**: Dataset mentah ulasan pengguna yang diekstrak langsung dari Google Play Store.
* **`image.png`**: Grafik visualisasi hasil analisis sentimen (Distribusi Sentimen, Jumlah per Sentimen, dan Hubungan Rating vs Sentimen).

## 🛠️ Teknologi & Library yang Digunakan
* **Python 3**
* **google-play-scraper**: Untuk mengambil data ulasan secara otomatis.
* **Pandas**: Untuk manipulasi, pembersihan data, dan manajemen kerangka data (DataFrame).
* **Hugging Face Transformers**: Model `w11wo/indonesian-roberta-base-sentiment-classifier` untuk klasifikasi sentimen teks bahasa Indonesia.
* **Matplotlib & tqdm**: Untuk menampilkan visualisasi grafik dan *progress bar*.

## 📊 Visualisasi & Ringkasan Hasil Analisis

Berikut adalah visualisasi dari hasil analisis sentimen yang telah dilakukan:

![Visualisasi Analisis Sentimen Canva](image.png)

Berdasarkan visualisasi data di atas, dapat ditarik kesimpulan sebagai berikut:
* **Sentimen Negatif (52.0%)**: Mendominasi ulasan, mayoritas berisi laporan pengguna mengenai masalah *loading* aplikasi, isu jaringan saat akan masuk (*login*), elemen error, dan kesulitan dalam membatalkan langganan Canva Pro/Bisnis.
* **Sentimen Positif (41.0%)**: Banyak pengguna memuji aplikasi karena sangat praktis, bermanfaat, dan mempermudah pekerjaan desain mereka.
* **Sentimen Netral (7.0%)**: Ulasan biasa atau pertanyaan seputar fitur tertentu.

## ⚙️ Cara Menjalankan Proyek
1. Buka file `UTS_BIG_DATA_TERRY.ipynb` menggunakan **Google Colab** atau **Jupyter Notebook**.
2. Jalankan *cell* pertama untuk menginstal library yang diperlukan (`pip install google-play-scraper`).
3. Jalankan *cell* berikutnya secara berurutan untuk mengumpulkan data ulasan, memuat model *Machine Learning*, dan menampilkan visualisasi hasil analisis sentimen.
