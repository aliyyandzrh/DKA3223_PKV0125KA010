# Projek AI untuk Computer Vision

## 1. Pengenalan Projek

Projek ini merupakan tugasan amali bagi kursus **DKA 3223 – AI untuk Computer Vision** yang melibatkan pembangunan dan simulasi aplikasi **Computer Vision menggunakan Artificial Intelligence (AI)**.

Projek ini terdiri daripada dua amali utama:

### Amali 1 – Simulasi Deployment Model CNN Asas

Amali 1 memberi fokus kepada pembinaan dan simulasi deployment model **Convolutional Neural Network (CNN)** asas untuk melakukan klasifikasi imej.

Model CNN digunakan untuk memproses imej dan membuat ramalan berdasarkan kelas yang telah ditetapkan. Dalam amali ini, model dikonfigurasi menggunakan PyTorch dan diuji menggunakan imej input.

Antara proses yang dilaksanakan ialah:

* Penyediaan dataset imej.
* Konfigurasi persekitaran PyTorch.
* Pembetulan ralat (bugs) dalam kod yang dibekalkan.
* Penetapan `INPUT_CHANNELS = 3` untuk imej RGB.
* Penetapan `OUTPUT_CLASSES = 2`.
* Penggunaan **Cross Entropy Loss** sebagai fungsi kerugian.
* Penggunaan **Adam Optimizer** dengan learning rate `0.001`.
* Latihan model selama `10 epochs`.
* Semakan penggunaan GPU.
* Penetapan random seed `42` bagi kebolehulangan keputusan.
* Pra-pemprosesan imej kepada saiz **224 × 224 piksel**.
* Pelaksanaan inferens menggunakan `model.eval()` dan `torch.no_grad()`.
* Paparan kelas ramalan dan nilai keyakinan dalam bentuk peratus.

Spesifikasi dan proses tersebut adalah berdasarkan bahan Amali 1 yang diberikan.

### Amali 2 – Simulasi Object Detection

Amali 2 memberi fokus kepada aplikasi **Object Detection** menggunakan model **YOLO11n**. Model ini digunakan untuk mengesan objek dalam imej dan memaparkan lokasi serta kelas objek yang dikesan.

Antara proses yang dilaksanakan ialah:

* Menyediakan persekitaran Google Colab.
* Menggunakan GPU **T4 Accelerator**.
* Memasang library `ultralytics` dan `torch`.
* Menyemak ketersediaan GPU menggunakan CUDA.
* Menetapkan random seed `42` untuk reproducibility.
* Menyediakan dataset imej kawalan kualiti/pengawasan.
* Mengenal pasti dan membaiki sekurang-kurangnya tiga ralat dalam skrip.
* Memuatkan model pralatih **YOLO11n**.
* Melatih model dengan:

  * Epochs: `5 – 10`
  * Image Size: `640`
  * Batch Size: `8 atau 16`
* Menjalankan inferens pada imej ujian.
* Memaparkan bounding box, nama kelas ramalan dan skor keyakinan.

## Proses ini adalah berdasarkan arahan dan spesifikasi dalam bahan Amali 2.

## 2. Objektif Projek

Objektif projek ini adalah untuk:

1. Memahami asas penggunaan AI dalam bidang Computer Vision.
2. Membina dan menguji model CNN untuk klasifikasi imej.
3. Memahami proses pra-pemprosesan imej sebelum inferens.
4. Memahami konsep Object Detection menggunakan YOLO.
5. Menjalankan latihan dan inferens model Computer Vision.
6. Memahami kepentingan GPU dan reproducibility dalam pembangunan model AI.
7. Mengenal pasti dan membaiki ralat dalam kod yang digunakan.
8. Mengamalkan etika profesional dalam penggunaan kod, dataset dan model AI.

---

## 3. Teknologi dan Library yang Digunakan

Projek ini menggunakan beberapa teknologi dan library berikut:

| Teknologi / Library | Kegunaan                                   |
| ------------------- | ------------------------------------------ |
| Python              | Bahasa pengaturcaraan utama                |
| Google Colab        | Persekitaran pembangunan dan latihan model |
| PyTorch             | Pembinaan dan pengujian model CNN          |
| Ultralytics         | Penggunaan model YOLO                      |
| YOLO11n             | Object Detection                           |
| CUDA / GPU          | Mempercepatkan proses latihan dan inferens |
| GitHub              | Penyimpanan dan perkongsian bahan projek   |

---

## 4. Sumber Kod Rujukan

Kod dalam projek ini dibangunkan berdasarkan bahan kod yang **dibekalkan untuk tujuan amali** serta rujukan kepada library dan framework yang digunakan.

Kod tidak boleh dianggap sebagai hasil ciptaan sepenuhnya sendiri sekiranya terdapat bahagian yang diambil, diubah suai atau dirujuk daripada sumber lain.

Sebarang kod daripada sumber luar hendaklah:

* Menyatakan sumber asal.
* Menghormati lesen penggunaan kod.
* Tidak membuang maklumat hak cipta atau atribusi.
* Tidak mendakwa kod pihak lain sebagai hasil sendiri.
* Membuat pengubahsuaian dengan jelas sekiranya kod asal telah diubah.

**Sumber utama framework/library:**

* PyTorch – digunakan untuk pembangunan model CNN.
* Ultralytics – digunakan untuk model YOLO.
* Google Colab – digunakan sebagai persekitaran pelaksanaan.

> **Nota:** Pautan sumber asal perlu ditambah berdasarkan sumber sebenar yang digunakan semasa membina kod. Jangan memasukkan pautan yang tidak pernah digunakan.

---

## 5. Sumber Dataset dan Hak Harta Intelek

Dataset yang digunakan dalam projek ini adalah dataset yang **dibekalkan untuk tujuan amali**, berdasarkan bahan tugasan.

Bagi Amali 1, dataset digunakan untuk latihan dan pengujian model CNN. Bagi Amali 2, dataset imej kawalan kualiti/pengawasan digunakan untuk latihan dan proses object detection.

### Penghormatan terhadap Harta Intelek

Saya mengakui bahawa dataset, kod, model pralatih dan bahan rujukan yang bukan hasil ciptaan sendiri adalah milik pemilik atau pencipta asal.

Saya akan:

* Mengiktiraf pemilik asal dataset dan kod.
* Mematuhi syarat lesen yang ditetapkan.
* Tidak menggunakan bahan berhak cipta tanpa kebenaran.
* Tidak mendakwa hasil kerja pihak lain sebagai hasil sendiri.
* Menyatakan sumber rujukan dengan jelas.
* Menggunakan bahan yang diperoleh hanya mengikut tujuan dan syarat penggunaannya.

---

## 6. Etika Pembangunan dan Penggunaan AI

Dalam pembangunan projek ini, aspek etika AI perlu diberi perhatian bagi memastikan teknologi digunakan secara bertanggungjawab.

Antara prinsip etika yang diamalkan ialah:

### 6.1 Ketelusan

Sumber kod, dataset dan model yang digunakan perlu dinyatakan dengan jelas supaya pengguna dapat memahami asal-usul bahan yang digunakan.

### 6.2 Menghormati Harta Intelek

Kod, dataset, model dan bahan rujukan daripada pihak lain tidak boleh diakui sebagai hasil sendiri. Atribusi dan lesen yang berkaitan perlu dihormati.

### 6.3 Privasi

Sekiranya sistem Computer Vision digunakan pada imej manusia atau persekitaran sebenar, data peribadi perlu dikendalikan dengan berhati-hati dan tidak disebarkan tanpa kebenaran.

### 6.4 Keadilan

Model AI boleh menghasilkan keputusan yang tidak tepat atau berat sebelah sekiranya dataset latihan tidak mewakili keadaan sebenar dengan baik.

### 6.5 Keselamatan

Output model tidak sepatutnya digunakan sebagai satu-satunya asas untuk membuat keputusan penting tanpa pengesahan manusia.

### 6.6 Penggunaan AI Secara Bertanggungjawab

AI perlu digunakan sebagai alat bantuan dan bukan untuk menipu, meniru hasil kerja orang lain atau melanggar hak cipta.

---

## 7. Limitasi Model

Model yang dibangunkan dalam projek ini mempunyai beberapa limitasi.

### CNN

Model CNN asas mungkin mempunyai ketepatan yang terhad kerana ia bergantung kepada:

* Saiz dataset.
* Kualiti imej.
* Kepelbagaian data latihan.
* Bilangan kelas.
* Parameter dan konfigurasi model.

Model juga mungkin memberikan ramalan yang salah apabila diberikan imej yang berbeza daripada data latihan.

### YOLO11n

Model YOLO11n yang digunakan untuk object detection juga mempunyai limitasi seperti:

* Pengesanan objek boleh menjadi kurang tepat dalam keadaan pencahayaan yang berbeza.
* Objek yang terlalu kecil atau terlindung mungkin sukar dikesan.
* Model bergantung kepada kualiti dan kepelbagaian dataset.
* Skor keyakinan yang tinggi tidak semestinya bermaksud ramalan tersebut benar.
* Prestasi model boleh berubah apabila digunakan pada persekitaran sebenar yang berbeza daripada data latihan.

Dalam Amali 2, latihan hanya dilakukan dalam julat **5–10 epochs** dengan image size `640` dan batch size `8 atau 16`, maka prestasi model tidak semestinya mewakili model yang telah melalui proses pengoptimuman secara menyeluruh.

---

## 8. Tanggungjawab Pengguna

Pengguna bertanggungjawab untuk menggunakan sistem AI secara beretika dan berhati-hati.

Pengguna hendaklah:

1. Tidak bergantung sepenuhnya kepada keputusan model AI.
2. Membuat semakan manusia terhadap hasil ramalan apabila diperlukan.
3. Tidak menggunakan sistem untuk tujuan yang boleh membahayakan atau merugikan pihak lain.
4. Menghormati privasi individu dalam penggunaan imej.
5. Tidak menyebarkan data atau imej tanpa kebenaran.
6. Memahami bahawa keputusan model boleh mengandungi kesilapan.
7. Menggunakan model berdasarkan tujuan dan batasan yang telah ditetapkan.

---

## 9. Reproducibility

Bagi memastikan eksperimen boleh diulang, random seed ditetapkan kepada:

```python
torch.manual_seed(42)
```

GPU juga diperiksa sebelum proses latihan dan inferens dijalankan.

## Penggunaan random seed membantu menghasilkan keputusan yang lebih konsisten antara percubaan, walaupun keputusan mungkin masih berbeza bergantung kepada konfigurasi persekitaran dan peranti yang digunakan.

## 10. Struktur Projek

Cadangan struktur repository GitHub:

```text
DKA3223-Computer-Vision/
│
├── README.md
│
├── Amali 1/
│   ├── DKA3223_ANGKAGILIRAN_AMALI1.ipynb
│   └── dataset/
│
├── Amali 2/
│   ├── DKA3223_ANGKAGILIRAN_AMALI2.ipynb
│   └── dataset/
│
└── results/
    ├── amali1/
    └── amali2/
```

> **Nota:** Nama fail dan folder boleh diubah mengikut nama sebenar fail yang dimuat naik ke GitHub.

---

## 11. Kesimpulan

Kesimpulannya, projek ini memberikan pendedahan kepada penggunaan AI dalam bidang Computer Vision melalui dua pendekatan, iaitu **klasifikasi imej menggunakan CNN** dan **Object Detection menggunakan YOLO11n**.

Selain aspek teknikal, projek ini turut menekankan kepentingan **etika profesional AI**, termasuk menghormati harta intelek, menyatakan sumber kod dan dataset, memahami limitasi model serta menggunakan teknologi AI secara bertanggungjawab.

Model AI tidak semestinya menghasilkan keputusan yang sempurna. Oleh itu, hasil ramalan perlu digunakan dengan pertimbangan yang sewajarnya dan, bagi penggunaan dunia sebenar, pengesahan manusia perlu dipertimbangkan.

---

## 12. Pengakuan

Saya mengakui bahawa projek ini dibangunkan untuk tujuan pembelajaran bagi kursus **DKA 3223 – AI untuk Computer Vision**. Sebarang kod, dataset, library atau model yang diperoleh daripada sumber luar diiktiraf dan digunakan dengan menghormati hak cipta serta lesen yang berkaitan.

**Nama:** Nur Aliyya Nadzira Binti Abdul Rahim
**Program:** Teknologi Komputeran
**Kelas:** 2D KPD
**Pensyarah:** En. Nasrun Naim bin Tajudin
