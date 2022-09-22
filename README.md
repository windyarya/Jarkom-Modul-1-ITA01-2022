# soal-shift-sisop-2-ITB11-2022

Penjelasan dan penyelesaian Soal Shift 2 Sistem Operasi 2021 Kelompok ITB11

1. Damarhafni Rahmannabel Nadim P (5027201026)
2. Achmad Aushaf Amrega Hisyam (5027201036)

# Daftar Isi

* [Daftar Isi](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#daftar-isi)
* [Soal 1](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-1)
    - [Soal 1.a.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-1a)
    - [Soal 1.b.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-1b)
    - [Soal 1.c.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-1c)
    - [Soal 1.d.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-1d)
    - [Soal 1.e.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-1e)
    - [Dokumentasi Soal 1](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#dokumentasi-soal-1)
* [Soal 2](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-2)
    - [Soal 2.a.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-2a)
    - [Soal 2.b.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-2b)
    - [Soal 2.c.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-2c)
    - [Soal 2.d.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-2d)
    - [Soal 2.e.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-2e)
    - [Dokumentasi Soal 2](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#dokumentasi-soal-2)
* [Soal 3](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-3)
    - [Soal 3.a.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-3a)
    - [Soal 3.b.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-3b)
    - [Soal 3.c.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-3c)
    - [Soal 3.d.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-3d)
    - [Soal 3.e.](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#soal-3e)
    - [Dokumentasi Soal 3](https://gitlab.com/Amrega/soal-shift-sisop-2-ITB11-2022/-/tree/main#dokumentasi-soal-3)

# Soal 1
Mas Refadi adalah seorang wibu gemink.  Dan jelas game favoritnya adalah bengshin impek. Terlebih pada game tersebut ada sistem gacha item yang membuat orang-orang selalu ketagihan untuk terus melakukan nya. Tidak terkecuali dengan mas Refadi sendiri. Karena rasa penasaran bagaimana sistem gacha bekerja, maka dia ingin membuat sebuah program untuk men-simulasi sistem history gacha item pada game tersebut. Tetapi karena dia lebih suka nge-wibu dibanding ngoding, maka dia meminta bantuanmu untuk membuatkan program nya. Sebagai seorang programmer handal, bantulah mas Refadi untuk memenuhi keinginan nya itu. 

* a. Saat program pertama kali berjalan. Program akan mendownload file characters dan file weapons dari link yang ada dibawah, lalu program akan mengekstrak kedua file tersebut. File tersebut akan digunakan sebagai database untuk melakukan gacha item characters dan weapons. Kemudian akan dibuat sebuah folder dengan nama “gacha_gacha” sebagai working directory. Seluruh hasil gacha akan berada di dalam folder tersebut. Penjelasan sistem gacha ada di poin (d).

* b. Mas Refadi ingin agar setiap kali gacha, item characters dan item weapon akan selalu bergantian diambil datanya dari database. Maka untuk setiap kali jumlah-gacha nya bernilai genap akan dilakukan gacha item weapons, jika bernilai ganjil maka item characters. Lalu untuk setiap kali jumlah-gacha nya mod 10, maka akan dibuat sebuah file baru (.txt) dan output hasil gacha selanjutnya akan berada di dalam file baru tersebut. Dan setiap kali jumlah-gacha nya mod 90, maka akan dibuat sebuah folder baru dan file (.txt) selanjutnya akan berada didalam folder baru tersebut.  Sehingga untuk setiap folder, akan terdapat 9 file (.txt) yang didalamnya berisi 10 hasil gacha. Dan karena ini simulasi gacha, maka hasil gacha di dalam file .txt adalah ACAK/RANDOM dan setiap file (.txt) isi nya akan BERBEDA.

* c. Format penamaan setiap file (.txt) nya adalah {Hh:Mm:Ss}_gacha_{jumlah-gacha}, misal 04:44:12_gacha_120.txt, dan format penamaan untuk setiap folder nya adalah total_gacha_{jumlah-gacha}, misal total_gacha_270. Dan untuk setiap file (.txt) akan memiliki perbedaan penamaan waktu output sebesar 1 second.

* d. Pada game tersebut, untuk melakukan gacha item kita harus menggunakan alat tukar yang dinamakan primogems. Satu kali gacha item akan menghabiskan primogems sebanyak 160 primogems. Karena mas Refadi ingin agar hasil simulasi gacha nya terlihat banyak, maka pada program, primogems di awal di-define sebanyak 79000 primogems. Setiap kali gacha, ada 2 properties yang akan diambil dari database, yaitu name dan rarity. Lalu Outpukan hasil gacha nya ke dalam file (.txt) dengan format hasil gacha {jumlah-gacha}_[tipe-item]_{rarity}_{name}_{sisa-primogems}. Program akan selalu melakukan gacha hingga primogems habis.
Contoh : 157_characters_5_Albedo_53880

* e. Proses untuk melakukan gacha item akan dimulai bertepatan dengan anniversary pertama kali mas Refadi bermain bengshin impek, yaitu pada 30 Maret jam 04:44.  Kemudian agar hasil gacha nya tidak dilihat oleh teman kos nya, maka 3 jam setelah anniversary tersebut semua isi di folder gacha_gacha akan di zip dengan nama not_safe_for_wibu dengan dipassword "satuduatiga", lalu semua folder akan di delete sehingga hanya menyisakan file (.zip)


Note:
    - Menggunakan fork dan exec.
    - Tidak boleh menggunakan fungsi system(), mkdir(), dan rename().
    - Tidak boleh pake cron.
    - Semua poin dijalankan oleh 1 script di latar belakang. Cukup jalankan script 1x serta ubah time dan date untuk check hasilnya.

Link
Database item characters :
https://drive.google.com/file/d/1xYYmsslb-9s8-4BDvosym7R4EmPi6BHp/view
Database item weapons :
https://drive.google.com/file/d/1XSkAqqjkNmzZ0AdIZQt_eWGOZ0eJyNlT/view

Tips :
    - Gacha adalah proses untuk mendapatkan suatu item dengan cara melakukan randomize dari seluruh item yang ada.
    - Dikarenakan file database memiliki format (.json). Silahkan gunakan library <json-c/json.h>, install dengan “apt install libjson-c-dev”, dan compile dengan “gcc [nama_file] -l json-c -o [nama_file_output]”. Silahkan gunakan dokumentasi berikut untuk membaca dan parsing file (.json).
https://progur.com/2018/12/how-to-parse-json-in-c.html

Silahkan gunakan Dynamic Memory Allocation pada C untuk menyimpan isi file (.json) jika file tersebut terlalu besar untuk disimpan saat parsing.

## Soal 1.a.

### Analisa Soal

pada soal 1.a. ini, kita diminta untuk membuat folder "gacha_gacha" dan mendownload 2 zip yang berisi database weapon dan character lalu mengekstrak kedua file zip tersebut di dalam folder "gacha_gacha".

### Cara Pengerjaan

untuk pengerjaannya, dapat menggunakan exec untuk mengerjakan perintah dari terminal. karena perintah exec menghilangkan process, maka dari itu untuk menjalankan perintah exec, harus dibuat process baru dengan cara ```fork()``` agar tidak berhenti programnya.

untuk membuat folder "gacha_gacha"
```c
child = fork();

if(child == 0){
    printf("making directory gacha_gacha.....\n");
    execlp("mkdir", "mkdir", "-p", "gacha_gacha", NULL); 
}
```
untuk mendownload database character dan weapon
```c
child = fork();

if(child == 0){
    printf("download characters database.....\n");
    execlp("wget", "wget" ,"--no-check-certificate","-q","https://drive.google.com/u/0/uc?id=1xYYmsslb-9s8-4BDvosym7R4EmPi6BHp&export=download" , "-O", "./gacha_gacha/Anggap_ini_database_characters.zip", NULL);
}

child = fork();

if(child == 0){
    printf("download weapons database.....\n");
    execlp("wget", "wget" ,"--no-check-certificate","-q","https://drive.google.com/u/0/uc?id=1XSkAqqjkNmzZ0AdIZQt_eWGOZ0eJyNlT&export=download" , "-O", "./gacha_gacha/Anggap_ini_database_weapon.zip", NULL);
}

```
untuk mengekstrak database character dan weapon
```c
child = fork();
    
if(child == 0){
    printf("extracting character database.....\n");
    chdir("gacha_gacha");
    execlp("unzip", "unzip", "-q", "Anggap_ini_database_characters.zip", NULL);
}
child = fork();
    
if(child == 0){
    printf("extracting weapons database.....\n");
    chdir("gacha_gacha");
    execlp("unzip", "unzip", "-q", "Anggap_ini_database_weapon.zip", NULL);
}
```
### Kendala

Kendala yang dialami adalah kesusahan pada memahami apa itu ```fork()``` dan memahami child process dan parent process karena pertama kali menggunakan function tersebut.

## Soal 1.b.

### Analisa Soal

Dalam soal 1B ini, kita diminta untuk membuat folder dan file, serta ketentuan untuk melakukan gacha berdasarkan jumlah gacha yang telah dilakukan. jika jumlah gacha genap, maka ambil gacha untuk weapon, jika ganjil, maka gacha untuk character, jika jumlah gachanya modulus 10, maka buat file txt baru dalam folder, jika jumlah gachanya modulus 90, maka buat folder baru.

### Cara Pengerjaan

untuk pengerajaannya, kita dapat menggunakan if sesuai dengan kondisi yang berlaku. lalu untuk membuat file, kita dapat menggunakan ```c
execlp("touch", "touch", namafile, NULL);```, untuk folder ```mkdir("touch", "mkdir", namafolder, NULL);```
```c
if(jumlah_gacha%90 == 0){
        
        
        strcpy(nam, "total_gacha_");
        sprintf(strint, "%d", jumlah_gacha);
        //itoa(jumlah_gacha, strint, 10);
        strcat(nam, strint);
        
    
        child = fork();

        if(child == 0){
            chdir("gacha_gacha");
     
            execlp("mkdir", "mkdir", "-p" ,nam, NULL); 
        }
        
    }

    while ((wait(&status)) > 0) ; 

    if(jumlah_gacha%10 == 0){
        

        strcpy(path, "gacha_gacha/");
        strcat(path, nam);
        //chdir(path);
        //chdir("gacha_gacha"); chdir(nam);
        
        //time_t rawtime;
        //struct tm * timeinfo;
        
        cekjam();
        /*time ( &rawtime );
        timeinfo = localtime ( &rawtime );
        
        strftime(temi, sizeof(temi)-1, "%H;%M;%S", timeinfo);*/
        

        sprintf(temi, "%02d", timeinfo->tm_hour);
        strcat(temi, ";");
        sprintf(temp, "%02d", timeinfo->tm_min);
        strcat(temi, temp);
        strcat(temi, ";");
        sprintf(temp, "%02d", timeinfo->tm_sec);
        strcat(temi, temp);

        strcat(temi, "_gacha_");
        sprintf(strint, "%d", jumlah_gacha);
        strcat(temi, strint);
        strcat(temi, ".txt");

        strcat(path, "/");
        strcat(path, temi);

        child = fork();
        
        if(child == 0){
            
            execlp("touch", "touch", path, NULL); 
        }
        while ((wait(&status)) > 0) ;
        sleep(1);
        timeinfo->tm_sec += 1;
    }
    
    while ((wait(&status)) > 0) ; 

    printf("gacha ke %d.....\n", jumlah_gacha+1);
    if(jumlah_gacha%2 == 1){
        read_asd('c', 50, 1, 2);
    }else if(jumlah_gacha%2 == 0){
        read_asd('w', 132, 21, 22);
    }
```
### Kendala
Kendala yang dialami adalah penggunaan library ```<time.h>``` yang masih awam.

## Soal 1.c.

### Analisa Soal

Soal 1.c. ini berisi ketentuan penamaan folder dan file. untuk file ```{Hh:Mm:Ss}_gacha_{jumlah-gacha}.txt```, untuk folder ```total_gacha_{jumlah-gacha}```.

### Cara pengerjaan

dapat menggunakan ```strcat()``` untuk menyusun stringnya, lalu string tersebut digunakan pada execlp

### Kendala

Tidak ada kendala yang dialami. 

## Soal 1.d.

### Analisa Soal

Dalam soal 1.d. ini berisi tentang ketentuan penamaan hasil gacha yang telah didapat lalu dimasukkan ke file yang telah dibuat. untuk penamaan hasil gacha ```{jumlah-gacha}_[tipe-item]_{rarity}_{name}_{sisa-primogems}``` dengan name dan rarity didapat dari database character dan weapon.

### Cara pengerjaan

Untuk pengerjaannya, dapat menggunakan ```strcat()``` untuk menyusun string hasil gacha, lalu untuk menulis pada file telah ditentukan, dapat menggunakan ```fopen()``` dan ```fwrite()```

```
fp = fopen(path,"a");
fwrite(temii, 1, strlen(temii), fp);
```

Lalu untuk mendapatkan data name dan rarity yang didapat dari database yang bertipe json, kita dapat menggunakan bantuan library ```<json-c/json.h>```. lalu kita dapat menggunakan function yang telah disediakan untuk mengambil data pada file json
```
fp = fopen(path,"r");
fread(buffer, 4096, 1, fp);
fclose(fp);

parsed_json = json_tokener_parse(buffer);

json_object_object_get_ex(parsed_json, "name", &name);
json_object_object_get_ex(parsed_json, "rarity", &rarity);
```
### Kendala

Kendala yang dialami adalah penggunaan library ```<json.h>``` yang masih awam, serta kesalahana memahami soal.

## Soal 1.e.

### Analisa Soal

Dalam soal 1.e. ini berisi tentang waktu kapan pelaksanaan gacha dan untuk melakukan zip pada folder "gacha_gacha" yang akan menjadi "not_safe_for_wibu.zip" dengan password "satuduatiga"

### Cara pengerjaan

untuk pengerjaan soal 1.e., kita dapat menggunakan ```localtime()``` pada library ```<time.h>``` untuk mendapatkan waktu pada saat itu juga.
```c
time ( &rawtime );
timeinfo = localtime ( &rawtime );
```
lalu untuk men-zip folder "gacha_gacha" dapat menggunakan
```c
execlp("zip", "zip", "-q", "-rm", "not_safe_for_wibu.zip","gacha_gacha", "--password", "satuduatiga", NULL);
```
disini saya tidak menggunakan ```fork()``` karena sudah berada pada akhir program, sehingga tidak perlu untuk men-spawning process.

### Kendala
Kendala yang dialami adalah ketidaktahuan atas ```timedatectl``` sehingga membuat kesalahan.

### Dokumentasi soal 1

- Terminal soal1.c <br>
![Terminal soal1.c](img/soal1/hasil_pada_terminal.PNG)
- Hasil pada folder "total_gacha" <br>
![Hasil "total_gacha"](img/soal1/hasil_pada_totalgacha.PNG)
- Hasil pada not_safe_for_wibu.zip <br>
![Hasil pada not_safe_for_wibu](img/soal1/hasil_pada_zip.PNG)
- Hasil pada txt <br>
![Hasil pada txt](img/soal1/hasil_pada_txt.PNG)

### Revisi
revisi terjadi pada soal :
- 1D isi dari hasil yang awalnya ```{nama}_{jenis}``` diganti menjadi ```{jumlah-gacha}_[tipe-item]_{rarity}_{name}_{sisa-primogems}
- 1E yang awalnya menguhab struct tm, sekarang menggunakan ```localtime()``` untuk mendapatkan waktu 


# Soal 2

Japrun bekerja di sebuah perusahaan dibidang review industri perfilman, karena kondisi saat ini sedang pandemi Covid-19, dia mendapatkan sebuah proyek untuk mencari drama korea yang tayang dan sedang ramai di Layanan Streaming Film untuk diberi review. Japrun sudah mendapatkan beberapa foto-foto poster serial dalam bentuk zip untuk diberikan review, tetapi didalam zip tersebut banyak sekali poster drama korea dan dia harus memisahkan poster-poster drama korea tersebut tergantung dengan kategorinya. Japrun merasa kesulitan untuk melakukan pekerjaannya secara manual, kamu sebagai programmer diminta Japrun untuk menyelesaikan pekerjaannya.
* a. Hal pertama yang perlu dilakukan oleh program adalah mengextract zip yang diberikan ke dalam folder “/home/[user]/shift2/drakor”. Karena atasan Japrun teledor, dalam zip tersebut bisa berisi folder-folder yang tidak penting, maka program harus bisa membedakan file dan folder sehingga dapat memproses file yang seharusnya dikerjakan dan menghapus folder-folder yang tidak dibutuhkan.
* b. Poster drama korea perlu dikategorikan sesuai jenisnya, maka program harus membuat folder untuk setiap jenis drama korea yang ada dalam zip. Karena kamu tidak mungkin memeriksa satu-persatu manual, maka program harus membuatkan folder-folder yang dibutuhkan sesuai dengan isi zip.
Contoh: Jenis drama korea romance akan disimpan dalam “/drakor/romance”, jenis drama korea action akan disimpan dalam “/drakor/action” , dan seterusnya.
* c. Setelah folder kategori berhasil dibuat, program akan memindahkan poster ke folder dengan kategori yang sesuai dan di rename dengan nama.
Contoh: “/drakor/romance/start-up.png”.
* d. Karena dalam satu foto bisa terdapat lebih dari satu poster maka foto harus di pindah ke masing-masing kategori yang sesuai. Contoh: foto dengan nama “start-up;2020;romance_the-k2;2016;action.png” dipindah ke folder “/drakor/romance/start-up.png” dan “/drakor/action/the-k2.png”. (note 19/03: jika dalam satu foto ada lebih dari satu poster maka foto tersebut dicopy jadi akhirnya akan jadi 2 foto)
* e. Di setiap folder kategori drama korea buatlah sebuah file "data.txt" yang berisi nama dan tahun rilis semua drama korea dalam folder tersebut, jangan lupa untuk sorting list serial di file ini berdasarkan tahun rilis (Ascending). Format harus sesuai contoh dibawah ini.
		
kategori : romance

nama : start-up
rilis  : tahun 2020

nama : twenty-one-twenty-five
rilis  : tahun 2022

Note dan Ketentuan Soal:
    - File zip berada dalam drive modul shift ini bernama drakor.zip
    - File yang penting hanyalah berbentuk .png
    - Setiap foto poster disimpan sebagai nama foto dengan format [nama]:[tahun rilis]:[kategori]. Jika terdapat lebih dari satu drama dalam poster, dipisahkan menggunakan underscore(_).
    - Tidak boleh menggunakan fungsi system(), mkdir(), dan rename() yang tersedia di bahasa C.
    - Gunakan bahasa pemrograman C (Tidak boleh yang lain).
    - Folder shift2, drakor, dan kategori dibuatkan oleh program (Tidak Manual).
    - [user] menyesuaikan nama user linux di os anda.


## Soal 2.a.

### Analisa Soal

Dalam soal 2.a. ini, kita diminta untuk membuat folder ```“/home/[user]/shift2/drakor”```. Selanjutnya kita diminta untuk meng-ekstrak file ```drakor.zip``` ke dalam folder baru yang telah kita buat tadi. lalu kita diminta untuk menghapus folder yang tidak berguna.

### Cara Pengerjaan

untuk mengerjakan soal 2.a. kita dapat menggunakan ```fork()``` untuk meng-spawn process agar program tidak terhenti saat menjalankan ```exec()``` yang digunakan untuk menjalankan perintah terminal melalui bahasa C.

untuk membuat directory ```shift2/drakor```
```c
child = fork();
if(child == 0){
    printf("create directory shift2/drakor....\n");
    execlp("mkdir", "mkdir", "/home/kali/shift2", NULL);
}
while ((wait(&status)) > 0) ; 
child = fork();
if(child == 0){
    execlp("mkdir", "mkdir", "/home/kali/shift2/drakor", NULL);
}

```
untuk meng-ekstrak ```drakor.zip```
```c
child = fork();
if(child == 0){
    execlp("unzip", "unzip", "-q", "drakor.zip", "-d", path, NULL);
}
```
Lalu untuk menghapus folder yang tidak berguna, dapat menggunakan
```c
child = fork();

if(child == 0){
    strcat(path, "/");
    strcat(path, oks);
    execlp("rm", "rm", "-r", path, NULL);
}
```
### Kendala

Kendala yang dialami adalah ada yang hal yang terlewat, yaitu untuk menghapus folder yang tidak berguna

## Soal 2.b.

### Analisa Soal

Dalam soal 2.b. ini, kita diminta untuk membuat folder baru pada ```shift2/drakor``` dengan nama folder "kategori" dari poster film drakor yang tersedia.

### Cara pengerjaan

untuk mengerjakan soal 2.b. ini, dapat menggunakan ```opendir()``` untuk membuka directory dan ```readdir()``` untuk mendapatkan nama folder dan file yang berada pada folder yang kita inginkan. Lalu untuk membuat folder menggunakan ```exec("mkdir")```

untuk mendapatkan data (kategori, nama, dan tahun) dari film drakor yang ada
```c
dp = opendir(path);
if(dp != NULL){
    while ((entry = readdir(dp))){
        strcpy(oks, entry->d_name);
        //printf("%s\n", oks);
        if(strstr(oks, ".png")){
            strcpy(okss, oks);
            token = strtok(okss, ";");
            strcpy(name1, token);
            token = strtok(NULL, ";");
            strcpy(date1, token);
            token = strtok(NULL, ";");
            if(strstr(token, "_")){
                strcpy(oksss, token);

                token = strtok(NULL, ";");
                strcpy(date2, token);

                token = strtok(NULL, ";");
                strcpy(cat2, strtok(token, "."));

                token2 = strtok(oksss, "_");
                strcpy(cat1, token2);
                token2 = strtok(NULL, "_");
                strcpy(name2, token2);

                cekdir(cat2, name2, date2, oks, 2);

            }else{
                strcpy(cat1, strtok(token, "."));                    
            }

            while ((wait(&status)) > 0) ;

            cekdir(cat1, name1, date1, oks, 1);
            
        }else if(strcmp(oks, ".") != 0 && strcmp(oks, "..") != 0){
            child = fork();

            if(child == 0){
                strcat(path, "/");
                strcat(path, oks);
                execlp("rm", "rm", "-r", path, NULL);
            }

            while ((wait(&status)) > 0) ;
        }
        memset(oks, 0, 50);
        memset(okss, 0, 50);
        memset(oksss, 0, 50);
        memset(name1, 0, 50);
        memset(date1, 0, 50);
        memset(cat1, 0, 50);
        memset(name2, 0, 50);
        memset(date2, 0, 50);
        memset(cat2, 0, 50);
    }
}
```
### Kendala
Tidak ada kendala 

## Soal 2.c.

### Analisa Soal

Dalam soal 2.c. ini, kita diminta untuk memindahkan poster film drakor pada kategori yang benar.

### Cara pengerjaan

Untuk mengerjakan soal 2.c. ini, kita dapat menggunakan ```strsrt()``` untuk mengidentifikasi mana poster dan yang bukan, karena di dalam folder ```shift2/drakor``` terdapat folder yang tidak digunakan. Lalu untuk memindahkan dan sekaligus me-rename poster film drakor dapat menggunakan ```execlp("mv", "mv", namaawal, rename, NULL);```. Lalu untuk mendapatkan data, dapat menggunakan ```strtok()``` untuk memisahkan data, untuk contohnya seperti pada "Cara pengerjaan soal 2B"

### Kendala

Tidak ada kendala 

## Soal 2.d.

### Analisa Soal

Dalam soal 2.d. ini, kita diminta berhati - hati dlaam memindahkan poster film drakor, karena ada beberapa poster film drakor yang memiliki 2 data dan diharuskan untuk memindahkan ke dalam 2 folder kategori yang benar.

### Cara pengerjaan

Untuk mengerjakan soal 2.d. ini, kita dapat menggunakan ```strstr()``` untuk mengidentifikasi mana poster film drakor yang memiliki 2 data. lalu jika poster tersebut memiliki 2 data, dapat menggunakan ```execlp("cp", "cp", namaawal, rename, NULL);``` untuk meng-copy dan me-rename poster ke dalam folder yang benar. Lalu pindahkan poster yang sama ke dalam folder kategori keduanya dengan ```execlp("mv", "mv", namaawal, rename, NULL);```

### Kendala

Tidak ada kendala 

## Soal 2.e.

### Analisa Soal

Dalam soal 2.e. ini, kita diminta untuk membuat file ```data.txt``` dalam setiap folder kategori untuk menyimpan data yang sudah kita dapat yang dikelompokkan berdasar kategori dari film tersebut, serta kita diminta juga untuk mengurutkan data secara ascending berdasar tahun rilis dari film tersebut.

### Cara pengerjaan

Untuk mengerjakan soal 2.e. ini, kita dapat menggunakan data yang telah kita dapatkan pada soal 2B tadi lalu kita urutkan berdasarkan tahunnya. Setelah itu, kita masukkan datanya ke dalam ```data.txt``` dengan cara
```c
if(cek){
    datatgl[jumlah] = tll;
    strcpy(data[jumlah++], dir);
    
    printf("%s\n", dir);
    child = fork();
    if(child == 0){
        strcat(path, "/");
        strcat(path, dir);
        //printf("%s\n", path);
        execlp("mkdir", "mkdir", path, NULL);
    }

    while ((wait(&status)) > 0) ;

    child = fork();
    if(child == 0){
        strcat(path, "/");
        strcat(path, dir);
        strcat(path, "/data.txt");
    
        execlp("touch", "touch", path, NULL);
    }

    while ((wait(&status)) > 0) ;

    strcat(path, "/");
    strcat(path, dir);
    strcat(path, "/data.txt");
    
    strcpy(tulisan, "\nnama : ");
    strcat(tulisan, nama);
    strcat(tulisan, "\nrilis  : ");
    strcat(tulisan, tgl);
    strcat(tulisan, "\n");

    fp = fopen(path, "a");
    fwrite(tulisan, 1, strlen(tulisan), fp);
    fclose(fp);

    memset(tulisan, 0, 100);
    memset(path, 0, strlen(path));
    strcpy(path, "/home/kali/shift2/drakor");
}else{
    //printf(" %s\n", nama);
    if(cekk == 1){
        strcat(path, "/");
        strcat(path, dir);
        strcat(path, "/data.txt");
        
        strcpy(tulisan, "\nnama : ");
        strcat(tulisan, nama);
        strcat(tulisan, "\nrilis  : ");
        strcat(tulisan, tgl);
        strcat(tulisan, "\n");

        fp = fopen(path, "a");
        fwrite(tulisan, 1, strlen(tulisan), fp);
        fclose(fp);

        memset(tulisan, 0, 100);
        memset(path, 0, strlen(path));
        strcpy(path, "/home/kali/shift2/drakor");
    }else{
        strcat(path, "/");
        strcat(path, dir);
        strcat(path, "/data.txt");

        fp = fopen(path, "r");
        fread(buffer, 4096, 1, fp);
        fclose(fp);

        child = fork();
        if(child == 0){
            execlp("rm", "rm", path, NULL);
        }
        while ((wait(&status)) > 0) ;

        child = fork();
        if(child == 0){
            execlp("touch", "touch", path, NULL);
        }

        while ((wait(&status)) > 0) ;

        strcpy(tulisan, "\nnama : ");
        strcat(tulisan, nama);
        strcat(tulisan, "\nrilis  : ");
        strcat(tulisan, tgl);
        strcat(tulisan, "\n");

        fp = fopen(path, "a");
        fwrite(tulisan, 1, strlen(tulisan), fp);
        fwrite(buffer, 1, strlen(buffer), fp);
        fclose(fp);

        memset(tulisan, 0, 100);
        memset(path, 0, strlen(path));
        memset(buffer, 0, strlen(buffer));
        strcpy(path, "/home/kali/shift2/drakor");

    }
}
```

### Kendala

Tidak ada kendala, tetapi ada hal kecil yang terlewat, yaitu menambahkan "tahun" pada "rilis : tahun" 

### Dokumentasi soal 2

- Hasil pada data.txt dan poster <br>
![Hasil pada data.txt dan poster](img/soal2/hasil_data_dan_poster.PNG)
- Hasil Folder <br>
![Hasil Folder](img/soal2/hasil_folder.PNG)

### Revisi

Revisi pada soal 2 adalah :
- 2A menghapus folder yang tidak berguna
- 2E menambahkan kata "tahun" pada "rilis : tahun"

# Soal 3
Conan adalah seorang detektif terkenal. Suatu hari, Conan menerima beberapa laporan tentang hewan di kebun binatang yang tiba-tiba hilang. Karena jenis-jenis hewan yang hilang banyak, maka perlu melakukan klasifikasi hewan apa saja yang hilang
* a. Untuk mempercepat klasifikasi, Conan diminta membuat program untuk membuat 2 directory di “/home/[USER]/modul2/” dengan nama “darat” lalu 3 detik kemudian membuat directory ke 2 dengan nama “air”. 
* b. Kemudian program diminta dapat melakukan extract “animal.zip” di “/home/[USER]/modul2/”.
* c. Tidak hanya itu, hasil extract dipisah menjadi hewan darat dan hewan air sesuai dengan nama filenya. Untuk hewan darat dimasukkan ke folder “/home/[USER]/modul2/darat” dan untuk hewan air dimasukkan ke folder “/home/[USER]/modul2/air”. Rentang pembuatan antara folder darat dengan folder air adalah 3 detik dimana folder darat dibuat terlebih dahulu. Untuk hewan yang tidak ada keterangan air atau darat harus dihapus.
* d. Setelah berhasil memisahkan hewan berdasarkan hewan darat atau hewan air. Dikarenakan jumlah burung yang ada di kebun binatang terlalu banyak, maka pihak kebun binatang harus merelakannya sehingga conan harus menghapus semua burung yang ada di directory “/home/[USER]/modul2/darat”. Hewan burung ditandai dengan adanya “bird” pada nama file.
* e. Terakhir, Conan harus membuat file list.txt di folder “/home/[USER]/modul2/air” dan membuat list nama semua hewan yang ada di directory “/home/[USER]/modul2/air” ke “list.txt” dengan format UID_[UID file permission]_Nama File.[jpg/png] dimana UID adalah user dari file tersebut file permission adalah permission dari file tersebut.
Contoh : conan_rwx_hewan.png

Catatan :
    - Tidak boleh memakai system().
    - Tidak boleh memakai function C mkdir() ataupun rename().
    - Gunakan exec dan fork
    - Direktori “.” dan “..” tidak termasuk

## Soal 3.a.

### Analisa Soal

Dalam soal 3.a. ini, kita diminta untuk membuat folder ```“/home/[user]/modul2/darat``` lalu 3 detik kemudian membuat folder ```“/home/[user]/modul2/air```.

### Cara pengerjaan

Untuk mengerjakan soal 3.a. ini, kita akan menggunakan fork dan exec beserta kondisi if else. Exec akan mengeksekusi perintah berupa mkdir dengan parameter -p yakni parent dan nama folder darat. Dengan menggunakan sleep kita dapat memberikan jeda 3 detik dan kemudian akan membuat folder air pada directory modul2.

```c
if (fork()==0) 
  {
    execlp("/bin/mkdir", "mkdir", "-p", "darat", NULL);
  }

  sleep(3);
  
  if (fork()==0) 
  {
    execlp("/bin/mkdir", "mkdir", "-p", "air", NULL);
  }

```

### Kendala

Tidak ada kendala yang dialami.

## Soal 3.b.

### Analisa Soal

Dalam soal 3.b. ini, kita diminta untuk meng-ekstrak file ```animal.zip``` ke dalam folder modul2 yang telah ada.

### Cara pengerjaan

Untuk mengerjakan soal 3.b. ini, kita akan melakukan hal yang serupa dengan soal 3.a. yakni dengan menggunakan fork dan exec beserta kondisi if else. Exec akan mengeksekusi perintah berupa unzip dengan parameter -o yakni overwrite dan -q yakni quiet mode.

```c
if (fork()==0)
  {
    execlp("/usr/bin/unzip", "unzip", "-oq","animal.zip", NULL);
  }
  
  sleep(2);

```

### Kendala

Tidak ada kendala yang dialami.

## Soal 3.c.

### Analisa Soal

Dalam soal 3.c., kita diminta untuk memisahkan hasil extract menjadi hewan darat dan hewan air sesuai dengan nama filenya dan dimasukkan ke dalam folder sesuai habitatnya. Kemudian setelah dipindahkan, apabila terdapat hewan yang tidak memiliki keterangan air dan darat harus dihapus.

### Cara pengerjaan

Untuk mengerjakan soal 3.b. ini, kita akan melakukan hal yang serupa dengan soal 3.b. yakni dengan menggunakan fork dan exec beserta kondisi if else. Exec akan mengeksekusi perintah berupa find untuk mencari file dengan ketentuan nama tertentu seperti *air.jpg atau *darat.jpg dan dilanjutkan dengan exec mv -t yang berarti memindahkan file tersebut ke target path tertentu. Kemudian setelah dipindahkan, apabila terdapat hewan yang tidak memiliki keterangan air dan darat harus dihapus dengan menggunakan perintah find untuk mencari file dengan tipe file tertentu yakni *jpg dan dilanjutkan dengan exec rm -r yang berarti menghapus file tersebut secara rekursif.
*
```c
while ((wait(&sts))>0);
  pindah_darat=fork();

  if(pindah_darat<0)
  {
    exit(EXIT_FAILURE);
  }

  if(pindah_darat==0)
  {
    execlp("/usr/bin/find", "find", "/home/nadim/modul2/animal", "-type", "f", "-name", "*darat.jpg", "-exec", "mv", "-t", "/home/nadim/modul2/darat", "{}", "+", (char*) NULL);
  }
  else
  {
    sleep(2);

    while ((wait(&sts))>0);
    pindah_air = fork();

    if(pindah_air<0)
    {
      exit(EXIT_FAILURE);
    }

    if(pindah_air==0)
    {
      execlp("/usr/bin/find", "find", "/home/nadim/modul2/animal", "-type", "f", "-name", "*air.jpg", "-exec", "mv", "-t", "/home/nadim/modul2/air", "{}", "+", (char*) NULL);
    }
  }

  sleep(2);

  while ((wait(&sts))>0);
  pindah_fish=fork();

  if (pindah_fish<0)
  {
    exit(EXIT_FAILURE);
  }

  if (pindah_fish==0)
  {
    execlp("/usr/bin/find", "find", "/home/nadim/modul2/animal", "-type", "f", "-name", "*air_fish.jpg", "-exec", "mv", "-t", "/home/nadim/modul2/air", "{}", "+", (char*) NULL); 
  }
  else
  {
    sleep(2);
    
    while ((wait(&sts))>0);
    pindah_bird=fork();

    if (pindah_bird<0)
    {
      exit(EXIT_FAILURE);
    }

    if (pindah_bird==0)
    {
      execlp("/usr/bin/find", "find", "/home/nadim/modul2/animal", "-type", "f", "-name", "*darat_bird.jpg", "-exec", "mv", "-t", "/home/nadim/modul2/darat", "{}", "+", (char*) NULL);
    }
  }

  sleep(2);
  
  //Hapus sisa hewan yang tidak masuk folder darat/air.
  while ((wait(&sts))>0);
  hapus_sisa=fork();

  if (hapus_sisa<0)
  {
    exit(EXIT_FAILURE);
  }

  if (hapus_sisa==0)
  {
    execlp("/usr/bin/find", "find", "/home/nadim/modul2/animal", "-type", "f", "-name", "*.jpg", "-exec", "rm", "-r", "{}", "+", (char*) NULL);
  }
    
  sleep(2);


```

### Kendala

Tidak ada kendala yang dialami.

## Soal 3.d.

### Analisa Soal

Dalam soal 3.d., kita diminta untuk memisahkan hasil extract menjadi hewan darat dan hewan air sesuai dengan nama filenya dan dimasukkan ke dalam folder sesuai habitatnya. Kemudian setelah dipindahkan, apabila terdapat hewan yang tidak memiliki keterangan air dan darat harus dihapus.

### Cara pengerjaan

Untuk mengerjakan soal 3.d. ini, kita akan melakukan hal yang serupa dengan soal 3.c. yakni dengan menggunakan fork dan exec beserta kondisi if else. Exec akan mengeksekusi perintah berupa find untuk mencari file dengan ketentuan nama tertentu seperti *bird.jpg atau *bird_darat.jpg dan dilanjutkan dengan exec rm -r yang berarti menghapus file tersebut secara rekursif.
*
```c
hapus_bird_belakang=fork();
  hapus_bird_tengah=fork();

  if (hapus_bird_belakang<0)
  {
    exit(EXIT_FAILURE);
  }

  if (hapus_bird_belakang==0)
  {
    execlp("/usr/bin/find", "find", "/home/nadim/modul2/darat", "-type", "f", "-name", "*bird.jpg", "-exec", "rm", "-r", "{}", "+", (char*) NULL);
  }

  if (hapus_bird_tengah<0)
  {
    exit(EXIT_FAILURE);
  }

  if (hapus_bird_tengah==0)
  {
    execlp("/usr/bin/find", "find", "/home/nadim/modul2/darat", "-type", "f", "-name", "*bird_darat.jpg", "-exec", "rm", "-r", "{}", "+", (char*) NULL);
  }

```

### Kendala

Tidak ada kendala yang dialami.

## Soal 3.e.

### Analisis soal 

Dalam soal 3.e. ini, kita diminta untuk membuat file ```list.txt``` pada folder ```/home/nadim/modul2/air``` yang berisi data dari file yang ada di folder tersebut dengan ketentuan ```UID_[UID file permission]_Nama File.[jpg/png]```

### Cara pengerjaan

Untuk mengerjakan soal ini, pertama buat file ```list.txt``` dengan ```execlp("/bin/touch", "touch","list.txt", NULL);```. Lalu dapat menggunakan ```opendir()``` untuk membuka directory tujuan, lalu ```readdir()``` untuk mendapatkan nama file yang ada di folder tersebut. Lalu untuk mendapatkan UID dan file permission, dapat menggunakan ```getpwuid()```. untuk programnya :

```c
while ((wait(&sts))>0);
  buat_list_file=fork();

  if(buat_list_file<0)
  {
    exit(EXIT_FAILURE);
  }

  if(buat_list_file==0)
  {
    execlp("/bin/touch", "touch","list.txt", NULL);
  }

  while ((wait(&sts))>0);
  pindah_list_air=fork();

  if(pindah_list_air<0)
  {
    exit(EXIT_FAILURE);
  }

  if(pindah_list_air==0)
  {
    execlp("/usr/bin/find", "find", "/home/nadim/modul2", "-type", "f", "-name", "*list.txt", "-exec", "mv", "-t", "/home/nadim/modul2/air", "{}", "+", (char*) NULL);
  }

  while ((wait(&sts))>0);

  masukkanlist("air");

  exit(EXIT_SUCCESS);
```

Dengan function tambahan 
```c
void masukkanlist(char di[]){
  //chdir(di);

  dp = opendir(di);
  if(dp != NULL){
    while ((entry = readdir(dp))){
      if(strcmp(entry->d_name, ".") == 0 || strcmp(entry->d_name, "..") == 0) continue;
      char tmp[50];
      char tmps[50];
      char uid[30];
     
      //strcpy(oks, entry->d_name);
      strcpy(tmp, di);
      strcat(tmp, "/");
      strcat(tmp, entry->d_name);
      r = stat(tmp, &fs);

      memset(tmp, 0, 10);
      strcpy(tmp, di);
      strcat(tmp, "/list.txt");
      // pw = getpwuid(fs.st_uid);
      sprintf(uid, "%s", getpwuid(fs.st_uid)->pw_name);
      strcpy(tmps, uid);
      strcat(tmps, "_");
      strcat(tmps, (fs.st_mode & S_IRUSR) ? "r" : "-");
      strcat(tmps, (fs.st_mode & S_IRUSR) ? "w" : "-");
      strcat(tmps, (fs.st_mode & S_IRUSR) ? "x" : "-");
      strcat(tmps, "_");
      strcat(tmps, entry->d_name);
      strcat(tmps, "\n");

      fp = fopen(tmp, "a");
      fwrite(tmps, 1, strlen(tmps), fp);
      fclose(fp);

    }
  }

}
```

### Kendala
Kendala yang terjadi adalah kami kekurangan waktu untuk mengerjakan soal 3.e. ini.

## Dokumentasi Soal 3

- Hasil Run pada Folder Air <br>
![Hasil Run pada Folder Air](img/soal3/Hasil%20Run.jpg)

- Hasil Run pada Folder Animal <br>
![Hasil Run pada Folder Animal](img/soal3/Hasil%20Run%202.jpg)

- Hasil Run pada Folder Darat <br>
![Hasil Run pada Folder Darat](img/soal3/Hasil%20Run%203.jpg)

- Hasil Revisi pada Nomor 3.e. (Memasukkan List file pada list.txt) <br>
![Hasil Revisi pada Nomor 3.e. (Memasukkan List file pada list.txt)](img/soal3/Hasil%20Revisi.jpg)
