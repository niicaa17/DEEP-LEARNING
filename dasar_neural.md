# Dasar-Dasar Neural Network

Pada era komputasi modern, neural network telah menjadi komponen inti dalam kecerdasan buatan. Konsep ini terinspirasi dari jaringan saraf biologis manusia dan memungkinkan komputer belajar untuk menyelesaikan tugas-tugas kompleks.

Dengan jutaan koneksi neuron buatan, neural network mampu:
- mengenali pola data,
- membuat prediksi,
- belajar dari pengalaman,
- serta digunakan dalam pengenalan gambar, NLP, robotika, dan lainnya.

Contoh penerapan sehari-hari meliputi:
- sistem rekomendasi platform streaming,
- pengenalan wajah,
- kendaraan otonom.

---

## Taksonomi AI

Taksonomi AI menggambarkan urutan evolusi konsep kecerdasan buatan:

### Artificial Intelligence (AI)
Konsep umum mesin yang mampu melakukan tugas yang membutuhkan kecerdasan manusia seperti pengambilan keputusan dan pemecahan masalah.

### Machine Learning (ML)
Cabang AI di mana komputer belajar dari data tanpa diprogram secara eksplisit.

### Neural Network (NN)
Model matematis terinspirasi jaringan saraf biologis, terdiri dari neuron buatan berlapis.

### Deep Learning (DL)
Sub-bidang ML yang menggunakan neural network berlapis banyak (deep neural network).

### Generative AI
Cabang AI yang mampu menghasilkan konten baru seperti teks, gambar, audio, dan video.

---

## Konsep Dasar Neural Network

Neural Network (NN) adalah model matematis yang meniru cara kerja otak manusia menggunakan unit pemrosesan sederhana bernama neuron.

Karakteristik:
- terdiri dari beberapa lapisan neuron
- memproses aliran informasi
- digunakan untuk klasifikasi, prediksi, dan pengenalan pola

---

## Saraf Biologis vs Saraf Tiruan

Neuron biologis terdiri dari:
- dendrit (menerima sinyal)
- badan sel

- akson (mengirim sinyal)

Pada NN:
- neuron buatan menerima input
- dikalikan bobot
- ditambah bias
- diproses fungsi aktivasi
- menghasilkan output

Bobot akan dipelajari dan disesuaikan selama proses training.

---

## Struktur Artificial Neural Network

### Single Perceptron

Komponen:
- input (x)
- bobot (w)
- bias (b)
- fungsi aktivasi f
- output (y)

Rumus dasar:
z = Σ(xi * wi) + b
y = f(z)


---

## Cara Kerja ANN

1. Input masuk ke layer pertama
2. Dikalikan bobot + bias
3. Lewat fungsi aktivasi
4. Output jadi input layer berikutnya
5. Hasil akhir = prediksi

ANN dapat memiliki jutaan neuron dalam banyak lapisan.

---

## Perceptron

Perceptron adalah unit dasar NN.

Komponen:
- input
- weights
- bias
- penjumlahan
- fungsi aktivasi
- output

Langkah kerja:
1. Input diterima
2. Dikalikan bobot
3. Ditambah bias
4. Hitung weighted sum
5. Lewat fungsi aktivasi
6. Hasilkan output

---

## Multilayer Perceptron (MLP)

MLP terdiri dari beberapa layer:

### Input Layer
Menerima fitur data.

### Hidden Layer
Memproses dan mengekstrak pola.

### Output Layer
Menghasilkan prediksi akhir.

---

## Terms pada Neural Network

### Activation Function

Menentukan apakah neuron aktif.

Jenis umum:

#### Linear
Output = input. Biasanya untuk regresi.

#### ReLU
f(x) = max(0, x)

Cepat dan populer.

#### Leaky ReLU
Versi ReLU dengan gradien kecil di sisi negatif.

#### Sigmoid
Output 0–1. Cocok klasifikasi biner. Rentan vanishing gradient.

#### Tanh
Output -1 sampai 1. Simetris terhadap nol.

#### Softmax
Menghasilkan probabilitas multiclass (total = 1).

---

## Loss Function

Mengukur kesalahan prediksi model.

Tujuan:
- mengukur error
- menjadi target minimisasi saat training

Contoh:
- Mean Squared Error (MSE)
- Cross Entropy

Semakin kecil loss → model semakin baik.

---

## Optimizer

Optimizer menyesuaikan bobot & bias agar loss turun.

Fungsi:
- hitung gradien
- update parameter
- percepat konvergensi

Contoh optimizer:
- SGD
- RMSprop
- Adam

---

## Forward Propagation

Proses menghitung prediksi.

Langkah:
1. Data masuk
2. Hitung weighted sum
3. Tambah bias
4. Aktivasi
5. Terus ke layer berikutnya
6. Hasilkan output

---

## Backpropagation

Proses belajar dari error.

Langkah:

### Hitung Error
Bandingkan output vs target → loss function.

### Backward Pass
Hitung gradien tiap bobot (chain rule).

### Update Bobot
Gunakan optimizer (gradient descent).

### Iterasi
Ulangi banyak epoch sampai konvergen.

---

Dengan kombinasi forward propagation dan backpropagation, neural network mampu belajar secara iteratif dan meningkatkan akurasi prediksi.

