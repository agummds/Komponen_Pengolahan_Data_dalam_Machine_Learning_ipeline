# Komponen Pengolahan Data dalam Machine Learning Pipeline
Pengolahan Data dalam Machine Learning Pipeline

Tujuan dari latihan ini adalah membuat tahapan pengolahan data sederhana dengan memanfaatkan berbagai tool yang disediakan oleh TFX. Tahapan pengolahan data ini terdiri dari beberapa proses seperti berikut.

<li>Proses data ingestion.</li> Pada proses ini kita menggunakan komponen ExampleGen.
<li>Proses data validation.</li>  Proses ini akan dibuat menggunakan beberapa komponen yang disediakan oleh TFX, seperti StatisticGen, SchemaGen, dan ExampleValidator
<li>Proses data preprocessing.</li>  Pada proses ini, kita akan memanfaatkan komponen Transform.


## Repository Resource:
``git clone https://github.com/dicodingacademy/a443-MLOps-ML-Pipeline.git``

## Link Google Colab:
ttps://colab.research.google.com/drive/1kySyaIQZ_FAADRwTDjtoY8JvVNaIn5N5?usp=sharing (tambahkan h diawal ya)

#  Membuat Model Serving Menggunakan Flask
Flask merupakan sebuah micro web framework yang ditulis dalam bahasa Python. Ia menyediakan berbagai tools dan library yang dapat digunakan untuk membuat web application (web app).

Model serving merupakan sebuah proses untuk menjalankan model machine learning di sebuah server (cloud atau on premises) yang dapat diakses melalui API endpoint.
Berdasarkan workload pada server, model serving dapat dibagi menjadi dua, yaitu **streaming (real-time)** dan **batch prediction**.


## Repository Resource: 
``git clone https://github.com/dicodingacademy/a443-MLOps.git``

## Link Google Collab:
ttps://colab.research.google.com/drive/1GaJKY1eSgekWUek9HUqvFahVaq3FBScX?usp=sharing (tambahkan h diawal ya)

# Submission 1: Machine Learning Pipeline - Sentiment Tweet Review
Nama: Agum Medisa

Username dicoding: agum_medisa


| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Sentiment Tweet Review](https://drive.google.com/drive/folders/1pCLO0hLiMceqae1vSEVbOXZFAGe1xFE1?usp=drive_link)|
| Masalah | Di media sosial terutama tweeter, banyaks ekali cuitan orang-orang di sana, terutama hal yang mengandung sentiment, Namun, menganalisis tweet ini secara manual dapat memakan waktu dan rentan terhadap bias. Tantangannya adalah mengotomatiskan proses mengklasifikasikan tweet ini sebagai positif atau negatif, yang dapat membantu para pencari data untuk memudahkan mereka dalam menganalisis |
| Solusi machine learning | Melalui masalah yang ada, pendekatan _machine learning_ akan sangat membantu untuk mengklasifikasikan sentiment yang berbasis teks. _Machine learning_, terutama _deep learning_ memiliki kemampuan yang baik dalam memproses data teks dan memberikan tingkat akurasi yang tinggi. Sehingga cocok digunakan untuk kasus ini. |
| Metode pengolahan | Data awal sentiment tweet akan dipisah menjadi data pelatihan dan data evaluasi dengan rasio 80:20, kemudian data akan melalui tahapan validasi untuk analisa dan menemukan anomali pada data. Tahap selanjutnya data akan diproses agar siap untuk masuk kedalam pelatihan. Setelah pelatihan maka akan dimasukkan juga ke dalam pelatihan komponen tuner selesai model akan di evaluasi dan di dikirim pada _endpoint_ dimana model siap dipakai. |
| Arsitektur model | Arsitektur yang digunakan cukup sederhana terdiri dari _layer Embedding_ dan satu _layer Dense_ sebagai _hidden layer_, kemudian fungsi aktivasi pada _output layer_ dan dalam kasus ini saya adalah _binary classification_.|
| Metrik evaluasi | Metrik evaluasi yang digunakan yaitu metrik klasifikasi seperti ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, dan BinaryAccuracy. |
| Performa model | Evaluasi model diperoleh yaitu AUC sebesar 0.481, true_negatives besar 31320, true_positives sebesar 0. Kemudian example_count 201,  dan loss: 0.2141 - binary_accuracy: 0.9406 - val_loss: 0.2023 - val_binary_accuracy: 0.9359 serta Best val_binary_accuracy So Far: 0.9468749761581421. Performa model dapat ditingkatkan lebih baik lagi, bisa dari segi data ataupun pemrosesan data yang lebih baik lagi. |


# Submission Final: Proyek Pengembangan dan Pengoperasian Sistem Machine Learning
Nama: Agum Medisa

Username dicoding: agum_medisa


| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Sentiment Tweet Review](https://drive.google.com/drive/folders/12z0RuXDpmh8zluoWtU_Va6U8jULOFXc5?usp=drive_link)|
| Masalah | Di media sosial terutama tweeter, banyaks ekali cuitan orang-orang di sana, terutama hal yang mengandung sentiment, Namun, menganalisis tweet ini secara manual dapat memakan waktu dan rentan terhadap bias. Tantangannya adalah mengotomatiskan proses mengklasifikasikan tweet ini sebagai positif atau negatif, yang dapat membantu para pencari data untuk memudahkan mereka dalam menganalisis |
| Solusi machine learning | Melalui masalah yang ada, pendekatan _machine learning_ akan sangat membantu untuk mengklasifikasikan sentiment yang berbasis teks. _Machine learning_, terutama _deep learning_ memiliki kemampuan yang baik dalam memproses data teks dan memberikan tingkat akurasi yang tinggi. Sehingga cocok digunakan untuk kasus ini. |
| Metode pengolahan | Data awal sentiment tweet akan dipisah menjadi data pelatihan dan data evaluasi dengan rasio 80:20, kemudian data akan melalui tahapan validasi untuk analisa dan menemukan anomali pada data. Tahap selanjutnya data akan diproses agar siap untuk masuk kedalam pelatihan. Setelah pelatihan maka akan dimasukkan juga ke dalam pelatihan komponen tuner selesai model akan di evaluasi dan di dikirim pada _endpoint_ dimana model siap dipakai. |
| Arsitektur model | Arsitektur yang digunakan cukup sederhana terdiri dari _layer Embedding_ dan satu _layer Dense_ sebagai _hidden layer_, kemudian fungsi aktivasi pada _output layer_ dan dalam kasus ini saya adalah _binary classification_.|
| Metrik evaluasi | Metrik evaluasi yang digunakan yaitu metrik klasifikasi seperti ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, dan BinaryAccuracy. |
| Performa model | Evaluasi model diperoleh yaitu AUC sebesar 0.481, true_negatives besar 31320, true_positives sebesar 0. Kemudian example_count 201,  dan loss: 0.2141 - binary_accuracy: 0.9406 - val_loss: 0.2023 - val_binary_accuracy: 0.9359 serta Best val_binary_accuracy So Far: 0.9468749761581421. Performa model dapat ditingkatkan lebih baik lagi, bisa dari segi data ataupun pemrosesan data yang lebih baik lagi. |
| Opsi Deployment | Di sini saya menggunakan cloudeka untuk mendeploy modelnya |
| Web App | [Tweer Sentiment](http://103.190.215.83:8501/v1/models/sentiment-review/metadata) |
| Monitoring | Di sini saya menggunakan prometherus dan grafana yang sudah terintegrasi dengan grafana dashboard|
