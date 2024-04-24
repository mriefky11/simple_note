Nama: Mochamad Riefky Rafliana Suwandy

Username dicoding: riefky_rafliana

|                         | Deskripsi                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Dataset                 | [Toxic Comments](https://www.kaggle.com/datasets/chaitanya99/toxic-comment-classification)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Masalah                 | Toxic Comments merupakan komentar-komentar yang mengandung konten yang merendahkan, mengancam, atau menyebarkan kebencian dapat membahayakan atau mengganggu individu atau kelompok tertentu. Identifikasi komentar-komentar semacam ini penting dalam menjaga keamanan dan kenyamanan lingkungan online, serta mencegah penyebaran pesan-pesan yang                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Solusi machine learning | Dengan menggunakan machine learning kita dapat mengetahui komentar-komentar yang bersifat negatif sehingga dapat menjaga kenyamanan di lingkungan                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Metode pengolahan | Pada dataset terdapat 2 feature kemudian dilakukan split data training dan eval menjadi rasio 80:20, dan mengubah data feature menjadi lowercase                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| Arsitektur model        | Dalam arsitektur model yang digunakan, dimulai dengan penggunaan layer vectorize untuk mengubah teks menjadi representasi numerik. Selanjutnya, ada layer embedding dengan dimensi embedding sebesar 16, yang membantu model mempelajari representasi yang lebih kaya dari teks. Karena data berupa teks, digunakan juga layer AveragePooling1D untuk mengambil rata-rata dari representasi kata-kata dalam teks. Setelah itu, terdapat dua layer dense dengan masing-masing memiliki 64 dan 32 unit, yang menggunakan aktivasi relu untuk mempelajari pola-pola yang kompleks dalam data. Akhirnya, digunakan layer dense dengan aktivasi sigmoid karena tujuan utamanya adalah klasifikasi biner antara dua label. Untuk pelatihan model, loss function yang digunakan adalah binary_crossentropy, yang sesuai untuk masalah klasifikasi biner, serta optimizer Adam untuk mengoptimalkan proses pelatihan. Metrik evaluasi yang digunakan adalah BinaryAccuracy, yang mengukur akurasi dari klasifikasi biner yang dilakukan oleh model. |

| Metrik evaluasi         | Metrik evaluasi yang digunakan ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, dan BinaryAccuracy. 

|

| Performa model | hasil metrik evaluasi menunjukkan bahwa model klasifikasi teks memiliki kinerja yang sangat baik dalam mengidentifikasi dan membedakan antara komentar-komentar beracun dan tidak beracun. Dengan nilai AUC yang tinggi (0.99014) dan akurasi biner sebesar 0.96562, model mampu dengan baik dalam memprediksi kelas-kelas yang benar |
