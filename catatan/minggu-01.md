# Catatan Minggu 01.md : Paradigma Pemrograman dan Setup
## Yang saya kerjakan
Pada minggu pertama, saya mempelajari tiga paradigma pemrograman, yaitu prosedural, berorientasi objek (OOP), dan fungsional. Saya membuat program sederhana yang berisi nama  dan NIM menggunakan ketiga paradigma  tersebut. 
## Keputusan desain
Saya  menggunakan paradigma prosedural dengan membuat method sapa () untuk meghasilkan teks sapaan. pada paradigma OOP, saya menggunakan class HelloOOP dengan atribut nama dan nim yang bersifat private agardata terlindungi.
## Kendala
saya juga masih mengalami kesulitan saat menjalankan pengujian karena masih terdapat kode TODO pada constructur class HelloOOP.Untuk mengatasi saya mengatur java versi 21 memasang maven, memperbaiki kode constructur dan method, kemudian menjalanakan ulang pengujian menggunakan perintah . \scripts\uji.ps1.
## Penggunaan AI
- Alat yang dipakai: chatgpt
- Bagian yang dibantu AI:
    *code
    *instalasi dan pemasangan Java dan Maven 
    *membuat dan memperbaiki kode pada tiga class java yaitu : Helloprosedural.java, HelloOOP, HelloFungsional.java
- Prompt utama:
    1. "Bantu saya memperbaiki kode java yang masih terdapat TODO pada class HelloOOP
    2. "Bantu saya memperbaiki error dan menjalnakan pengujian menggunakan PowerShell
- Yang saya ubah atau tolak dari saran AI, dan alasannya:
    Saya memperbaiki  bagian kode yang masih terdapat TODO dan menyesuaikan dengan intruksi tugas agar program dapat berjalan dengan benar.
- Satu hal yang saya pahami lebih baik sekarang:
    Saya lebih memahami perbedaan  tiga paradigma pemrograman , yaitu prosedural yang fokus pada fungsi,OOP yang menggunakan class dan objek, serta fungsional yang menggunakn fungsional lamda.
## Hasil Pengujian
    PS C:\Users\ismat\Documents\OOP\oop-202601-250202912\oop-202601-250202912> .\scripts\uji.ps1
Menjalankan tes minggu 1 sampai 1  (groups: week1)
[INFO] Scanning for projects...
[INFO] Loaded 24571 auto-discovered prefixes for remote repository central (prefixes-central.txt)
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Build Order:
[INFO] 
[INFO] Aset-Pinjam (OOP 202601)                                           [pom]
[INFO] Aset-Pinjam Core (minggu 1-11)                                     [jar]
[INFO] Aset-Pinjam API (minggu 12-15)                                     [jar]
[INFO] 
[INFO] --------------------< id.ac.upb:asetpinjam-parent >---------------------
[INFO] Building Aset-Pinjam (OOP 202601) 0.1.0                            [1/3]
[INFO]   from pom.xml
[INFO] --------------------------------[ pom ]---------------------------------
[INFO] 
[INFO] ---------------------< id.ac.upb:asetpinjam-core >----------------------
[INFO] Building Aset-Pinjam Core (minggu 1-11) 0.1.0                      [2/3]
[INFO]   from core\pom.xml
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- resources:3.3.1:resources (default-resources) @ asetpinjam-core ---
[INFO] Copying 0 resource from src\main\resources to target\classes
[INFO] Copying 1 resource from src\main\resources to target\classes
[INFO] 
[INFO] --- compiler:3.14.1:compile (default-compile) @ asetpinjam-core ---
[INFO] Recompiling the module because of changed source code.
[INFO] Compiling 33 source files with javac [debug parameters release 21] to target\classes
[INFO] 
[INFO] --- resources:3.3.1:testResources (default-testResources) @ asetpinjam-core ---
[INFO] skip non existing resourceDirectory C:\Users\ismat\Documents\OOP\oop-202601-250202912\oop-202601-250202912\core\src\test\resources
[INFO] 
[INFO] --- compiler:3.14.1:testCompile (default-testCompile) @ asetpinjam-core ---
[INFO] Recompiling the module because of changed dependency.
[INFO] Compiling 12 source files with javac [debug parameters release 21] to target\test-classes
[INFO] 
[INFO] --- surefire:3.5.6:test (default-test) @ asetpinjam-core ---
[INFO] Using auto detected provider org.apache.maven.surefire.junitplatform.JUnitPlatformProvider
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running id.ac.upb.asetpinjam.Minggu01Test
[INFO] Tests run: 5, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.098 s -- in id.ac.upb.asetpinjam.Minggu01Test
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 5, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] 
[INFO] ----------------------< id.ac.upb:asetpinjam-api >----------------------
[INFO] Building Aset-Pinjam API (minggu 12-15) 0.1.0                      [3/3]
[INFO]   from api\pom.xml
[INFO] --------------------------------[ jar ]---------------------------------
[INFO] 
[INFO] --- resources:3.3.1:resources (default-resources) @ asetpinjam-api ---
[INFO] Copying 1 resource from src\main\resources to target\classes
[INFO] Copying 0 resource from src\main\resources to target\classes
[INFO] 
[INFO] --- compiler:3.14.1:compile (default-compile) @ asetpinjam-api ---
[INFO] Recompiling the module because of changed dependency.
[INFO] Compiling 12 source files with javac [debug parameters release 21] to target\classes
[INFO] 
[INFO] --- resources:3.3.1:testResources (default-testResources) @ asetpinjam-api ---
[INFO] skip non existing resourceDirectory C:\Users\ismat\Documents\OOP\oop-202601-250202912\oop-202601-250202912\api\src\test\resources
[INFO] 
[INFO] --- compiler:3.14.1:testCompile (default-testCompile) @ asetpinjam-api ---
[INFO] Recompiling the module because of changed dependency.
[INFO] Compiling 2 source files with javac [debug parameters release 21] to target\test-classes
[INFO] 
[INFO] --- surefire:3.5.6:test (default-test) @ asetpinjam-api ---
[INFO] Using auto detected provider org.apache.maven.surefire.junitplatform.JUnitPlatformProvider
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 0, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] Reactor Summary for Aset-Pinjam (OOP 202601) 0.1.0:
[INFO] 
[INFO] Aset-Pinjam (OOP 202601) ........................... SUCCESS [  0.006 s]
[INFO] Aset-Pinjam Core (minggu 1-11) ..................... SUCCESS [  3.567 s]
[INFO] Aset-Pinjam API (minggu 12-15) ..................... SUCCESS [  4.988 s]
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  9.213 s
[INFO] Finished at: 2026-11-22T12:23:46+07:00
[INFO] ------------------------------------------------------------------------
