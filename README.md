# soal-shift-jarkom-1-ITA01-2022

Penjelasan dan penyelesaian Soal Shift 1 Jaringan Komputer 2022 Kelompok ITA01

1. Damarhafni Rahmannabel Nadim P (5027201026)
2. Salman Al Farisi Sudirlan (5027201056)
3. I Putu Windy Arya Sagita (5027201071)

# Daftar Isi

* [Daftar Isi](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/-/tree/main#daftar-isi)
* [Soal 1](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/#soal-1)
* [Soal 2](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/#soal-2)
* [Soal 3](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/soal-3)
* [Soal 4](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/#soal-4)
* [Soal 5](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/#soal-5)
* [Soal 6](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/#soal-6)
* [Soal 7](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/#soal-7)
* [Soal 8](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/#soal-8)
* [Soal 9](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/#soal-9)
* [Soal 10](https://github.com/windyarya/Jarkom-Modul-1-ITA01-2022/#soal-10)

# Soal 1

Sebutkan web server yang digunakan pada `monta.if.its.ac.id`!

## Analisa Soal

Pada soal 1 ini, kita diminta untuk mencari web server yang digunakan oleh host `monta.if.its.ac.id`.

## Cara Pengerjaan

Dengan menggunakan Display Filter http, maka kita dapat menyaring seluruh paket yang terkoneksi dengan HTTP, salah satunya yakni website `monta.if.its.ac.id`. Hal ini dapat kita cek dengan melakukan ping `monta.if.its.ac.id` dan kedua nya menunjukkan IP Address yang sama yakni `103.94.189.5`.

Dengan melihat isi dari salah satu response dari host `103.94.189.5`, maka terlihat bahwa server yang digunakan adalah `nginx/1.10.3`.

## Kendala

Tidak ada kendala

## Dokumentasi Soal 1
- Hasil display filter `http`  <br>
![Hasil Display Filter http](images/1-1.png)

- Hasil ping web Monta  <br>
![Hasil Ping Web Monta](images/1-2.png)

- Hasil response dari web Monta  <br>
![Hasil Filter soal 3](images/1-3.png)

# Soal 2

Ishaq sedang bingung mencari topik TA untuk semester ini, lalu ia datang ke website monta dan menemukan **detail topik** pada website `monta.if.its.ac.id`, judul TA apa yang dibuka oleh ishaq?

## Analisa Soal

Pada soal 2 ini, kita diminta untuk mencari request dan response yang mengarah ke host `monta.if.its.ac.id`. Dengan mencari response tersebut, kita bisa mendapatkan judul TA yang dibuka oleh Ishaq.

## Cara Pengerjaan

Dengan display filter http, command `http.request.uri contains "detail"` kita mendapatkan packet request ke website monta yaitu ke path `index.php/topik/detailTopik/194` sebagai berikut.

Dengan mengetahui packet requestnya di packet 576, kita bisa mencari request dan response nya dengan command display filter berikut `http.request.uri contains "detail" or http.request_in eq 576`. Kemudian, pada request kita cari judulnya dan mendapatkan topik TA yaitu ???Evaluasi unjuk kerja User Space Filesystem FUSE???.

## Kendala

Tidak ada kendala

## Dokumentasi Soal 2
- Hasil display dilter `http.request.uri contains "detail"`  <br>
![Hasil Display Filter](images/2-1.png)

- Hasil display filter `http.request.uri contains "detail" or http.request_in eq 576`  <br>
![Hasil Ping Web Monta](images/2-2.png)


# Soal 3
Filter sehingga wireshark hanya menampilkan paket yang menuju ```port 80```.

## Analisa Soal

Dalam soal 3 ini, kita diminta untuk menampilkan seluruh paket yang menuju port 80.

## Cara pengerjaan

Untuk mengerjakan soal 3 ini, kita akan menggunakan syntax tcp.dstport dan udp.dstport. Dengan tcp.dstport == 80 || udp.dstport == 80, kita dapat menyaring seluruh paket TCP yang menuju port (dstport) 80 dan paket UDP yang menuju port (dstport) 80.

## Kendala

Tidak ada kendala yang dialami.

## Dokumentasi Soal 3
- Hasil Filter soal 3 <br>
![Hasil Filter soal 3](images/3.png)

# Soal 4
Filter sehingga wireshark hanya mengambil paket yang berasal dari ```port 21```.

## Analisa Soal

Dalam soal 4 ini, kita diminta untuk menggunakan filter dalam wireshark sehingga hanya menampilkan paket yang berasal dari port 21.
.

## Cara pengerjaan

Untuk mengerjakan soal 4 ini, kita akan melakukan hal yang mirip dengan soal 3 yakni dengan menggunakan syntax tcp dan udp, hanya saja yang membedakannya yakni port asal dibanding port tujuan sehingga kita akan menggunakan tcp.srcport dan udp.srcport. Dengan tcp.srcport == 21 || udp.srcport == 21, kita dapat menyaring seluruh paket TCP yang berasal dari port (srcport) 21 dan paket UDP yang berasal dari port (srcport) 21.
.

## Kendala

Tidak ada kendala yang dialami.

## Dokumentasi Soal 4
- Hasil Filter soal 4 <br>
![Hasil Filter soal 4](images/4.png)

# Soal 5
Filter sehingga wireshark hanya mengambil paket yang berasal dari ```port 443```.

## Analisa Soal

Dalam soal 5 ini, kita diminta untuk menggunakan filter dalam wireshark sehingga hanya menampilkan paket yang berasal dari port 21.

## Cara pengerjaan

Dalam soal 5, kita akan melakukan hal yang sama dengan soal 4 yakni dengan menggunakan syntax tcp.srcport dan udp.srcport. Dengan tcp.srcport == 443 || udp.srcport == 443, kita dapat menyaring seluruh paket TCP yang berasal dari port (srcport) 443dan paket UDP yang berasal dari port (srcport) 443.

## Kendala

Tidak ada kendala yang dialami.

## Dokumentasi Soal 5
- Hasil Filter soal 5 <br>
![Hasil Filter soal 5](images/5.png)

# Soal 6
Filter sehingga wireshark hanya menampilkan paket yang menuju ke lipi.go.id!

## Analisa Soal

Dalam soal 6, kita diminta untuk menampilkan seluruh paket yang menuju ```lipi.go.id```.
.

## Cara pengerjaan

Untuk mengerjakan soal 6 ini, kita akan mencari ip website lipi.go.id dengan perintah ping pada cmd/terminal.

Kemudian kita dapat melakukan filter dengan syntax ip.dst dan mencari ip destinasi yang sama sesuai hasil IP yang didapat dari ping sebelumnya yakni ```ip.dst == 203.160.128.158``` dan dari deskripsi Request ``GET``` dapat dilihat tertulis ???FULL REQUEST URI: http://lipi.go.id???. Berikut ini hasil screenshot dari paket yang menuju ke lipi.go.id.

## Kendala

Tidak ada kendala yang dialami.

## Dokumentasi Soal 6
- Hasil ping lipi.go.id <br>
![Hasil ping lipi.go.id](images/6-1.png)

- Hasil Filter soal 6 <br>
![Hasil Filter soal 6](images/6-2.png)

# Soal 7
Filter sehingga wireshark hanya mengambil paket yang berasal dari ip kalian!

## Analisis soal 

Pada soal ini, kita diminta untuk melakukan filter sehingga yang tampil hanyalah paket yang berasal dari IP miliki kita.

## Cara pengerjaan

Pertama kita dapat mengetahui ip address melalui cmd/terminal dengan syntax `ipconfig (cmd)` atau `ifconfig -a (terminal)` disini terlihat ip kami pada bagian IPv4 Address.

Lalu saat mendapatkan IP-nya, kita melakukan filter package dengan syntax `ip.src == 192.168.1.7` agar dapat terlihat paket yang berasal dari kita.


## Kendala
Tidak ada kendala

## Dokumentasi Soal 6
- Hasil cek IP Address <br>
![Hasil cek IP](images/7-1.png)

- Hasil Filter soal 7 <br>
![Hasil Filter soal 7](images/7-2.png)

# Untuk soal 8-10, silahkan baca cerita di bawah ini!

Di sebuah planet bernama Viltrumite, terdapat Kementerian Komunikasi dan Informatika yang baru saja menetapkan kebijakan baru. Dalam kebijakan baru tersebut, pemerintah dapat mengakses data pribadi masyarakat secara bebas jika memang dibutuhkan, baik dengan maupun tanpa persetujuan pihak yang bersangkutan. Sebagai mahasiswa yang sedang melaksanakan program magang di kementerian tersebut, kalian mendapat tugas berupa penyadapan percakapan mahasiswa yang diduga melakukan tindak kecurangan dalam kegiatan Praktikum Komunikasi Data dan Jaringan Komputer 2022. Selain itu, terdapat sebuah password rahasia (flag) yang diduga merupakan milik sebuah organisasi bawah tanah yang selama ini tidak sejalan dengan pemerintahan Planet Viltrumite. Tunggu apa lagi, segera kerjakan tugas magang tersebut agar kalian bisa mendapatkan pujian serta kenaikan jabatan di kementerian tersebut!

# Soal 8
Telusuri aliran paket dalam file .pcap yang diberikan, cari informasi berguna berupa percakapan antara dua mahasiswa terkait tindakan kecurangan pada kegiatan praktikum. Percakapan tersebut dilaporkan menggunakan protokol jaringan dengan tingkat keandalan yang tinggi dalam pertukaran datanya sehingga kalian perlu menerapkan filter dengan protokol yang tersebut.

## Analisa  Soal
Pada soal ini kami diperintahkan untuk menelusuri percakapan tersembunyi antar-mahasiswa yang sedang membicarakan kunci jawaban.

## Pengerjaan Soal
Pada percakapan ini kami menemukan peserta menanyakan clue untuk mendapatkan jawaban soal shift dari kode mencurigakan dan bagaimana cara memecahkan kodenya. Kami menelusurinya dengan metode syntax `tcp.stream eq [angka]` dan follow dari setiap paket yang ada dan menemukan beberapa percakapan dalam screenshot berikut:

## Kendala
Tidak ada, hanya perlu waktu saja.

## Dokumentasi Soal 8
- Hasil pencarian paket soal no 8 <br>
![Hasil pencarian paket soal no 8](images/8.png)

# Soal 9
Terdapat laporan adanya pertukaran file yang dilakukan oleh kedua mahasiswa dalam percakapan yang diperoleh, carilah file yang dimaksud! Untuk memudahkan laporan kepada atasan, beri nama file yang ditemukan dengan format [nama_kelompok].des3 dan simpan output file dengan nama ???flag.txt???.

## Analisa Soal
Pada soal ini kami diperintahkan mencari file yang mencurigakan yang dikirim. Setelah mendapatkan soalnya kami disuruh untuk mensavenya dengaan format des3 dan hasil output dekripsi des3nya disave dengan nama flag.txt

## Pengerjaan Soal
Dengan petunjuk yang diberikan dalam percakapan dari soal sebelumnya (8) dapat
diketahui port yang digunakan yakni ``port 9002``. Maka dari itu kita akan menggunakan
Display Filter `tcp.dstport == 9002`. Kami menemukan kode rahasia yang kemungkinan
berisi jawaban saat kodenya di decrypt sesuai petunjuk pelaku.

Kemudian hasil deskripsi ini diubah menjadi Raw dan didapatkan hasil string yang terenkripsi dengan OpenSSL dan DES3. Dari percakapan tadi juga dapat diketahui kata sandi atau password berupa lima karakter anime yang kembar 5. Ketika dilakukan penelusuran di Google didapatkan 5 nama karakter berupa Ichika, Nino, Miku, Yotsuba, dan Itsuki Nakano. Untuk mendekripsinya kami menggunakan fungsi terminal `openssl enc -d -des3 -in encrypted.txt -out decrypted.txt` dengan password `nakano` dan mendapatkan hasil berikut:

## Kendala
Kami Salah syntax file sebelumnya untuk mendekripsi hasil file des3nya

## Revisi
Disini kami salah syntax untuk mendekrip filenya karena kami malah mensave file saltnya dengan format `.txt` bukan `.des3` sehingga terjadi error. Untuk syntaxnya yang benar menjadi `openssl enc -d -des3 -in ITA.des3 -out flag.txt` lalu masukkan keynya, yaitu nakano.

## Dokumentasi Soal 9
- Hasil penemuan isi file des3 dalam bentuk ASCII <br>
![Hasil penemuan isi file des3 dalam bentuk ASCII](images/9-2.png)

- Hasil penemuan isi file des3 dalam bentuk raw <br>
![Hasil penemuan isi file des3 dalam bentuk raw](images/9-3.png)

### Sebelum Revisi
- Syntax dekripsi yang salah <br>
![Hasil penemuan isi file des3 dalam bentuk raw](images/9-1.png)

### Sesudah Revisi
- Syntax dekripsi yang benar <br>
![Syntax dekripsi yang benar](images/9-4.png)

- Memasukkan keynya <br>
![Memasukkan keynya](images/9-5.png)

# Soal 10 (Revisi)
Temukan password rahasia (flag) dari organisasi bawah tanah yang disebutkan di atas!

## Analisa Soal
Kami harus menemukan flag pada dari output file des3 yang telah didekripsi sesuai petunjuk yang pelaku jelaskan.

## Pengerjaan Soal
Disini kami hanya menampilkan hasil dekripsi dari file des3 pada soal 9

## Kendala
Kami terkendala waktu sehingga belum sempat menuntaskan soal.

## Revisi
Sebenarnya jika nomor 9 selesai maka otomatis nomor 10 selesai karena nomor 10 hanya merupakan hasil dari nomor 9.

## Dokumentasi Soal 10
- Hasil dekripsi file des3 <br>
![Hasil dekripsi file des3](images/10.png)




