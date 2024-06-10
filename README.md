Books Recommendation Systems
<<<<---------------------------+++++++++++++++++++++++++++++------------------------------->>>> <<------>> Capstone Project MSIB Skilvul Batch 7 IBM Skillsbuild for AI & Cybersecurity <<--------->> <<<<------------+++++------------->>>> Created by : Team 23 <<<<------------+++++------------>>>> <<<<---------------------------+++++++++++++++++++++++++++++------------------------------->>>>

Description
Sistem rekomendasi buku berbasis machine learning dengan rating adalah aplikasi yang dirancang untuk memberikan saran buku kepada pengguna berdasarkan preferensi dan riwayat pembacaan mereka. Sistem ini memanfaatkan algoritma machine learning untuk menganalisis data pengguna, termasuk buku yang telah mereka baca dan nilai yang mereka berikan. Dengan menggunakan data ini, sistem dapat memprediksi buku yang mungkin disukai oleh pengguna di masa depan. Pendekatan ini meningkatkan pengalaman pengguna dengan menyediakan rekomendasi yang lebih akurat dan personal, sehingga membantu mereka menemukan buku baru yang sesuai dengan minat mereka. Sistem rekomendasi ini biasanya memanfaatkan teknik seperti collaborative filtering, content-based filtering, dan hybrid methods untuk menghasilkan rekomendasi yang efektif dan relevan.

Data yang Akan Dipakai
goodbooks-10k (Book Recomendation System with Rating)

Metadata, Ratings, Popular Title Attributes, Ratings and User Engagement Metric (https://www.kaggle.com/datasets/zygmunt/goodbooks-10k)

=> Kumpulan data ini berisi peringkat untuk sepuluh ribu buku populer. Mengenai sumbernya, katakanlah rating ini ditemukan di internet. Umumnya, ada 100 ulasan untuk setiap buku, meskipun beberapa memiliki peringkat yang lebih sedikit. Peringkatnya berkisar dari satu hingga lima. Ada kumpulan data yang bagus untuk rekomendasi film (Netflix, Movielens) dan musik (Jutaan Lagu), tetapi tidak untuk buku. Begitulah, sampai sekarang. ID buku dan ID pengguna keduanya bersebelahan. Untuk buku 1-10.000, untuk pengguna 1-53424. Semua pengguna telah membuat setidaknya dua peringkat. Jumlah rata-rata peringkat per pengguna adalah 8. Ada juga buku yang ditandai untuk dibaca oleh pengguna, metadata buku (penulis, tahun, dll.) dan tag.

Model yang Digunakan
Cosine Similarity
=> Cosine Similarity cocok digunakan untuk membandingkan kesamaan antara buku berdasarkan fitur teks seperti judul atau deskripsi dan juga ketika tidak ada informasi rating yang tersedia, tetapi ingin merekomendasikan buku berdasarkan kesamaan fitur.

Singular Value Decomposition (SVD)
=> SVD dipilih karena efektif dalam mengatasi masalah cold start (ketika ada user atau buku baru) dan menangani data yang jarang (sparse), dengan cara mengekstrak fitur-fitur utama dari data, dan keunggulannya menghasilkan representasi latensi dari user dan item, memungkinkan model untuk menangkap preferensi latent user dan karakteristik buku.

Non-Negative Matrix Factorization (NMF)
=> NMF adalah NMF menghasilkan faktor tersembunyi yang dapat diinterpretasikan secara langsung, dan juga ecara efektif melakukan reduksi dimensi pada data rating, sehingga dapat mengatasi masalah sparsity (kekosongan) dari dataset rating. NMF dapat digunakan untuk menghasilkan rekomendasi yang personalisasi, dengan menghasilkan matriks faktorisasi yang disesuaikan dengan preferensi masing-masing pengguna.

K-Nearest Neighbors (KNN)
=> KNN itu adalah sebuah algoritma yang sederhana dan mudah dimengerti, cocok untuk dataset kecil hingga sedang, cepat dan mudah diimplementasikan, cocok untuk digunakan sebagai baseline atau untuk kasus sederhana rekomendasi berbasis user.

