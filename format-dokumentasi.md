# Submission 1: Nama Proyek Anda
Nama:

Username dicoding:

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Dataset Komentar Instagram Cyberbullying](https://github.com/rizalespe/Dataset-Sentimen-Analisis-Bahasa-Indonesia/blob/master/dataset_komentar_instagram_cyberbullying.csv) |
| Masalah | Dataset ini berisi komentar-komentar di Instagram yang berhubungan dengan cyberbullying. Setiap komentar telah diberi label dengan sentimen, yang bisa berupa "positive" atau "negative". Komentar ini digunakan untuk mengidentifikasi apakah suatu komentar mengandung cyberbullying atau tidak berdasarkan teks yang diberikan.Tujuan utama dari proyek ini adalah untuk membangun sebuah model yang dapat memprediksi apakah suatu komentar Instagram mengandung cyberbullying atau tidak. Model ini perlu mengklasifikasikan komentar ke dalam dua kategori sentimen: negatif (cyberbullying) atau positif (tidak mengandung cyberbullying).|
| Solusi machine learning | Deskripsi Solusi Machine Learning: Model machine learning yang akan dibangun menggunakan metode Text Classification dengan menggunakan neural network berbasis deep learning. Model akan menggunakan arsitektur yang terdiri dari layer TextVectorization untuk mengubah teks komentar menjadi vektor angka, kemudian diteruskan ke layer embedding dan beberapa layer dense untuk mengklasifikasikan sentimen komentar. |
| Metode pengolahan | Deskripsi Metode Pengolahan Data:
Preprocessing: Teks komentar akan diproses dengan menghilangkan tanda baca dan mengubahnya menjadi huruf kecil menggunakan TextVectorization.
Feature Engineering: Setelah data diproses, model akan menggunakan teknik embedding untuk mewakili setiap kata dalam komentar sebagai vektor numerik. Kemudian, model akan memanfaatkan pooling dan dense layers untuk menghasilkan prediksi sentimen.
Data Split: Dataset dibagi menjadi dua bagian, yaitu data pelatihan (train) dan data evaluasi (eval) dengan rasio 3:1. |
| Arsitektur model | Deskripsi Arsitektur Model: Model yang digunakan adalah model deep neural network (DNN) dengan struktur berikut:
Input Layer: Komentar Instagram yang diubah menjadi representasi numerik menggunakan TextVectorization.
Embedding Layer: Untuk mengubah kata-kata dalam komentar menjadi vektor berdimensi lebih rendah.
Global Average Pooling: Untuk merangkum representasi kata-kata menjadi satu vektor yang mewakili seluruh komentar.
Dense Layers: Dua lapisan dense untuk menangkap fitur-fitur non-linear dari data.
Output Layer: Menggunakan sigmoid activation untuk menghasilkan output antara 0 (negatif) dan 1 (positif), yang akan digunakan untuk klasifikasi sentimen. |
| Metrik evaluasi | Binary Cross-Entropy Loss: Digunakan sebagai fungsi loss untuk klasifikasi biner (positif atau negatif).
Binary Accuracy: Metrik ini digunakan untuk mengevaluasi akurasi model dalam mengklasifikasikan komentar sebagai positif atau negatif.
AUC (Area Under Curve): Digunakan untuk mengevaluasi kinerja model secara keseluruhan dengan mengukur area di bawah kurva ROC. |
| Performa model | Deskripsi Performa Model: Performa model diukur dengan menggunakan metrik akurasi, binary cross-entropy, dan AUC. Model ini diharapkan dapat mengklasifikasikan komentar Instagram dengan cukup akurat, membedakan komentar yang mengandung cyberbullying dan yang tidak, berdasarkan fitur yang diekstraksi dari teks komentar. Model akan diuji menggunakan data evaluasi yang sebelumnya dipisahkan dari data pelatihan |
