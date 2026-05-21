# TUGAS-2 

# Survei Penggunaan ChatGPT sebagai Pendukung Pembelajaran terhadap Mahasiswa

# Latar Belakang

Kemajuan teknologi pada era digital saat ini memberikan pengaruh yang sangat besar terhadap cara mahasiswa belajar dan memperoleh informasi. Proses pembelajaran yang sebelumnya hanya bergantung pada buku dan penjelasan dosen kini mulai didukung oleh berbagai teknologi modern yang mempermudah mahasiswa dalam memahami materi pembelajaran. Salah satu teknologi yang berkembang pesat dan banyak digunakan saat ini adalah Artificial Intelligence (AI).
Artificial Intelligence atau kecerdasan buatan merupakan teknologi yang dirancang untuk membantu manusia dalam menyelesaikan berbagai pekerjaan secara lebih cepat dan efisien. Dalam bidang pendidikan, AI mulai dimanfaatkan sebagai media pendukung pembelajaran karena mampu memberikan informasi, penjelasan, dan jawaban secara instan sesuai kebutuhan pengguna. Salah satu bentuk AI yang paling populer di kalangan mahasiswa saat ini adalah ChatGPT.
ChatGPT banyak digunakan mahasiswa karena memiliki kemudahan akses dan dapat digunakan kapan saja dalam membantu aktivitas belajar. Mahasiswa memanfaatkan ChatGPT untuk mencari referensi, memahami materi perkuliahan, membuat rangkuman, menerjemahkan teks, hingga membantu menyelesaikan tugas akademik. Penggunaan ChatGPT dianggap dapat membantu mahasiswa menghemat waktu dan meningkatkan efektivitas belajar, terutama ketika mahasiswa mengalami kesulitan memahami materi tertentu.
Meskipun memberikan banyak manfaat, penggunaan ChatGPT dalam pembelajaran juga menimbulkan berbagai pendapat di kalangan mahasiswa. Sebagian mahasiswa merasa penggunaan ChatGPT sangat membantu dalam meningkatkan pemahaman materi dan produktivitas belajar, namun sebagian lainnya berpendapat bahwa penggunaan AI secara berlebihan dapat menyebabkan ketergantungan dan menurunkan kemampuan berpikir mandiri mahasiswa. Oleh karena itu, penggunaan ChatGPT dalam pembelajaran perlu dipahami secara bijak agar tetap memberikan dampak positif terhadap proses belajar mahasiswa.
Fenomena meningkatnya penggunaan ChatGPT di kalangan mahasiswa menjadi hal yang menarik untuk diteliti, terutama terkait bagaimana persepsi dan pengalaman mahasiswa dalam menggunakan teknologi tersebut sebagai media pendukung pembelajaran. Berdasarkan kondisi tersebut, peneliti tertarik untuk melakukan penelitian dengan judul **“Survei Penggunaan ChatGPT sebagai Pendukung Pembelajaran terhadap Mahasiswa”** untuk mengetahui bagaimana tanggapan mahasiswa terhadap penggunaan ChatGPT dalam kegiatan belajar sehari-hari.

# Rumusan Masalah
* Bagaimana penggunaan ChatGPT sebagai media pendukung pembelajaran mahasiswa?
* Bagaimana tanggapan mahasiswa terhadap penggunaan ChatGPT dalam proses belajar?
* Apakah penggunaan ChatGPT memberikan manfaat dalam membantu aktivitas akademik mahasiswa?
  
#  Tujuan Penelitian
* Mengetahui penggunaan ChatGPT sebagai media pendukung pembelajaran mahasiswa.
* Mengetahui respon mahasiswa terhadap penggunaan ChatGPT dalam kegiatan belajar.
* Mengetahui manfaat penggunaan ChatGPT dalam membantu aktivitas akademik mahasiswa.

# Metode Penelitian
Penelitian ini menggunakan metode kuantitatif dengan pendekatan survei. Pengumpulan data dilakukan melalui penyebaran kuesioner online menggunakan Google Form kepada mahasiswa sebagai responden penelitian. Penelitian ini menggunakan teknik penentuan sampel dengan rumus Slovin untuk menentukan jumlah responden yang digunakan dalam penelitian.
Instrumen penelitian menggunakan skala Likert dengan lima kategori jawaban, yaitu:
* Sangat Tidak Setuju
* Tidak Setuju
* Netral
* Setuju
* Sangat Setuju
Data yang telah terkumpul kemudian dianalisis menggunakan aplikasi SPSS. Analisis data yang dilakukan meliputi:
* Uji Slovin
* Uji Validitas
* Uji Reliabilitas
Jumlah responden dalam penelitian ini sebanyak 28 mahasiswa.

Hasil dan Pembahasan
Penelitian ini menggunakan variabel tunggal yaitu penggunaan ChatGPT sebagai pendukung pembelajaran mahasiswa. Variabel penelitian diukur melalui beberapa indikator yang terdapat pada item pertanyaan kuesioner.
| Kode | Indikator                 | Keterangan                                                                          |
| ---- | ------------------------- | ----------------------------------------------------------------------------------- |
| P1   | Penggunaan ChatGPT        | Mengukur penggunaan ChatGPT dalam aktivitas belajar mahasiswa.                      |
| P2   | Pemahaman Materi          | Mengukur kemampuan ChatGPT dalam membantu memahami materi pembelajaran.             |
| P3   | Penyelesaian Tugas        | Mengukur pengaruh ChatGPT dalam membantu menyelesaikan tugas akademik.              |
| P4   | Kemudahan Penggunaan      | Mengukur kemudahan mahasiswa dalam menggunakan ChatGPT.                             |
| P5   | Efektivitas Belajar       | Mengukur pengaruh ChatGPT terhadap efektivitas proses belajar.                      |
| P6   | Pencarian Informasi       | Mengukur manfaat ChatGPT dalam membantu mencari informasi akademik.                 |
| P7   | Produktivitas Belajar     | Mengukur pengaruh ChatGPT terhadap produktivitas belajar mahasiswa.                 |
| P8   | Dukungan Pembelajaran     | Mengukur dukungan ChatGPT terhadap proses pembelajaran mahasiswa.                   |
| P9   | Ketergantungan Penggunaan | Mengukur pandangan mahasiswa terhadap penggunaan ChatGPT secara berlebihan.         |
| P10  | Kepuasan Penggunaan       | Mengukur tingkat kepuasan mahasiswa terhadap penggunaan ChatGPT dalam pembelajaran. |

# Tahapan Analisis Data 
Analisis data pada penelitian ini dilakukan menggunakan aplikasi RStudio. Tahapan analisis data meliputi penentuan jumlah sampel menggunakan rumus Slovin, import data penelitian, uji validitas, dan uji reliabilitas instrumen penelitian.

1. Penentuan Jumlah Sampel Menggunakan Rumus Slovin
Syntax berikut digunakan untuk menghitung jumlah sampel penelitian berdasarkan jumlah populasi dan tingkat kesalahan (error) yang telah ditentukan. Pada penelitian ini digunakan populasi sebanyak 154 mahasiswa dengan tingkat kesalahan sebesar 15%.

```r
# Slovin
N <- 154
e <- 0.15
n <- ceiling(N / (1 + N * e^2))
cat("Jumlah sampel berdasarkan rumus Slovin =", n)

2. Import Data Penelitian
Syntax berikut digunakan untuk mengimpor data penelitian dari file Excel ke dalam RStudio. Selain itu, syntax ini juga digunakan untuk melihat nama variabel dan isi data yang telah diinput.

# Import Data
library(readxl)
library(psych)
data <- read_excel("C:/tugas/teksam p.xlsx")
View(data)
# Melihat nama variabel
names(data)
# Melihat data
View(data)

3. Uji Validitas
Syntax berikut digunakan untuk melakukan uji validitas pada item kuesioner penelitian. Uji validitas dilakukan untuk mengetahui apakah setiap item pernyataan pada kuesioner layak digunakan dalam penelitian.

# UJI VALIDITAS
# Ambil item kuesioner
item <- data[, c("P1","P2","P3","P4","P5","P6","P7","P8","P9","P10")]
# Uji validitas
corr.test(item)
# Skor total
total <- rowSums(item)
# Korelasi item-total
cor(item, total)

4. Uji Reliabilitas
Syntax berikut digunakan untuk melakukan uji reliabilitas menggunakan metode Cronbach Alpha. Uji reliabilitas dilakukan untuk mengetahui tingkat konsistensi instrumen penelitian.

# UJI RELIABILITAS
# Uji reliabilitas Cronbach Alpha
alpha(item)$total
# Menampilkan hasil Cronbach Alpha
alpha(item)$total$raw_alpha

# Hasil dan Pembahasan
Berdasarkan hasil penelitian mengenai Survei Penggunaan ChatGPT sebagai Pendukung Pembelajaran terhadap Mahasiswa, diperoleh data dari 28 responden yang telah mengisi kuesioner penelitian. Penelitian dilakukan menggunakan metode survei dengan instrumen kuesioner yang terdiri dari 10 item pernyataan (P1–P10).
Penentuan jumlah sampel dilakukan menggunakan rumus Slovin dengan jumlah populasi sebanyak 154 mahasiswa dan tingkat kesalahan sebesar 15%. Berdasarkan hasil perhitungan diperoleh jumlah sampel minimum sebanyak 35 responden. Namun, pada penelitian ini jumlah data responden yang berhasil dianalisis sebanyak 28 responden.
Hasil uji validitas menunjukkan bahwa sebagian besar item pernyataan memiliki hubungan korelasi yang cukup kuat hingga sangat kuat. Berdasarkan hasil korelasi item-total diperoleh nilai korelasi tertinggi pada item P10 sebesar 0,923 dan item P8 sebesar 0,863. Hal tersebut menunjukkan bahwa kedua item memiliki hubungan yang sangat kuat terhadap variabel penelitian. Selain itu, item P1, P2, P3, P5, P6, dan P7 juga memiliki nilai korelasi di atas 0,70 sehingga dinyatakan valid dan mampu mengukur variabel penelitian dengan baik.
Namun, terdapat satu item yaitu P9 yang memiliki nilai korelasi paling rendah sebesar 0,290. Nilai tersebut menunjukkan bahwa item P9 memiliki hubungan yang lemah dibandingkan item lainnya sehingga kurang mendukung variabel penelitian secara keseluruhan. Selain itu, pada hasil korelasi Pearson juga terlihat bahwa item P9 memiliki hubungan negatif terhadap beberapa item lain, seperti P4 sebesar -0,12. Hal ini menunjukkan bahwa respon responden pada item P9 cenderung berbeda dibandingkan item pertanyaan lainnya.
Hasil uji reliabilitas menggunakan metode Cronbach’s Alpha memperoleh nilai sebesar 0,901. Nilai tersebut menunjukkan bahwa instrumen penelitian memiliki tingkat reliabilitas yang sangat tinggi karena melebihi batas minimum reliabilitas sebesar 0,70. Dengan demikian, kuesioner penelitian dinyatakan konsisten dan layak digunakan sebagai instrumen penelitian.
Berdasarkan hasil analisis secara keseluruhan, sebagian besar responden memberikan tanggapan positif terhadap penggunaan ChatGPT sebagai media pendukung pembelajaran. Mahasiswa menilai bahwa ChatGPT membantu dalam memahami materi perkuliahan, mencari informasi akademik, menyelesaikan tugas, serta meningkatkan efektivitas belajar. Hal tersebut terlihat dari tingginya hubungan antar item pertanyaan yang berkaitan dengan manfaat penggunaan ChatGPT dalam proses pembelajaran.
Secara umum, hasil penelitian menunjukkan bahwa penggunaan ChatGPT memberikan dampak positif terhadap aktivitas belajar mahasiswa. Namun demikian, penggunaan ChatGPT tetap perlu digunakan secara bijak agar mahasiswa tidak terlalu bergantung pada teknologi AI dalam proses pembelajaran.

# Kesimpulan
Berdasarkan hasil penelitian mengenai **Survei Penggunaan ChatGPT sebagai Pendukung Pembelajaran terhadap Mahasiswa**, dapat disimpulkan bahwa penggunaan ChatGPT memberikan pengaruh positif dalam mendukung aktivitas pembelajaran mahasiswa. Hasil uji validitas menunjukkan bahwa sebagian besar item pernyataan memiliki nilai korelasi yang baik sehingga dinyatakan valid untuk digunakan dalam penelitian. Selain itu, hasil uji reliabilitas memperoleh nilai Cronbach’s Alpha sebesar 0,901 yang menunjukkan bahwa instrumen penelitian memiliki tingkat reliabilitas yang sangat tinggi dan konsisten.
Hasil analisis menunjukkan bahwa mahasiswa merasa ChatGPT membantu dalam memahami materi perkuliahan, mencari informasi akademik, menyelesaikan tugas, serta meningkatkan efektivitas belajar. Item dengan nilai korelasi tertinggi terdapat pada P10 dan P8 yang menunjukkan bahwa kedua indikator memiliki hubungan yang sangat kuat terhadap variabel penelitian. Namun, terdapat satu item yaitu P9 yang memiliki hubungan korelasi rendah dibandingkan item lainnya sehingga menunjukkan adanya perbedaan persepsi responden pada indikator tersebut.
Secara keseluruhan, penggunaan ChatGPT dapat dijadikan sebagai media pendukung pembelajaran mahasiswa karena mampu memberikan manfaat dalam proses belajar. Namun demikian, penggunaan ChatGPT tetap perlu dilakukan secara bijak agar tidak menimbulkan ketergantungan berlebihan terhadap teknologi AI dalam aktivitas akademik mahasiswa.



