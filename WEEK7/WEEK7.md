# Week 2

# Database Introduction

- Database adalah kumpulan informasi yang disimpan di dalam komputer secara sistematik dan saling berelasi.
- Database merupakan sekumpulan tabel yang berisikan informasi untuk diolah yang kemudian data tersebut bisa digunakan di dalam sebuah sistem.

# Database Management System (DBMS)

- DBMS adalah software yang dapat digunakan oleh user untuk berkomunikasi dengan data yang ada dalam media penyimpanan.
- Tipe utama pada Database management System antara lain, Hierarchical, Network, Relational, Non-Relational, and Object Oriented.

# Istilah pada database

- Tabel
    
    Tabel adalah  kumpulan value yang dibangun oleh baris dan kolom, yang di dalamnya berisikan atribut dari sebuah data.
    
- Field
    
    Field adalah kolom dari sebuah tabel di mana masing-masing field memiliki tipe data masing-masing.
    
- Record
    
    Record merupakan kumpulan nilai yang saling terkait. Record merupakan isi dari sebuah tabel.
    

# SQL

- SQL atau Structured Query Language merupakan suatu bahasa (Language) yang digunakan untuk mengakses database.
- SQL adalah Bahasa Query yang digunakan untuk melakukan interaksi di RDMS (Relational Database Management System)
- SQL digunakan untuk:
    - Membuat, menampilkan dan menghapus data di dalam database.
    - Mengatur “permission” (siapa saja yang bisa mengakses data).
    - Membuat dan menghapus database

# Data Definition Language

- DDL (Data Definition Language) merupakan kumpulan perintah SQL yang digunakan untuk membuat, mengubah dan menghapus struktur dan definisi metadata dari objek-objek Database.
- Beberapa contoh perintah DDL
    - ALTER
    - DROP
    - CREATE
    - RENAME
    - TRUNCATE

# Data Definition Language

- DDL (Data Definition Language) adalah perintah yang digunakan untuk memanipulasi tabel
- Beberapa contoh perintah DDL
    - SELECT
    - INSERT
    - UPDATE
    - DELETE

# Data Control Language

- DCL (Data Control Language) adalah perintah yang digunakan untuk mengontrol akses ke data yang disimpan dalam database (otorisasi).
- DCL hanya memiliki 2 perintah yaitu:
    - GRANT
    - REVOKE

# Klausa WHERE

Klausa ini digunakan untuk memfilter *records,* jadi hanya records yang memenuhi kondisi tertentu saja yang akan tampil

# Operator AND, OR, NOT

- Klausa WHERE bisa dikombinasikan dengan operator AND, OR, dan NOT.
- Operator AND menampilkan record jika semua kondisi yang dipisahkan oleh AND adalah TRUE.
- Operator OR menampilkan record jika salah satu kondisi yang dipisahkan oleh OR adalah TRUE.

# Database Relationship

- Sederhananya, *database relationship* adalah relasi atau hubungan antara beberapa tabel dalam bahasa yang kita miliki.
- Beberapa jenis relasi pada database adalah
    - one-to-one
    - one-to-many
    - many-to-one
    - many-to-many

# Database Normalization

- Database Normalization adalah merupakan teknik analisis data yang mengorganisasikan atribut-atribut data dengan cara mengelompokkan sehingga terbentuk entitas yang non-redundant, stabil, dan fleksibel.
- Tujuan dari database normalization adalah:
    - Menghilangkan redundan data pada database.
    - Memudahkan jika ada perubahan struktur table database.
    - Memperkecil pengaruh jika ada perubahan dari struktur table database
- Bentuk database normalization
    - First Normal Form (1NF)
    - Second Normal Form (2NF)
    - Third Normal Form (3NF)

# Keys in SQL

- Super key
    
    Super key adalah kumpulan dari satu atau lebih dari satu key yang dapat digunakan untuk mengidentifikasi record secara unik dalam sebuah tabel.
    
- Candidate Key
    
    Candidate Key adalah kumpulan satu atau lebih fields/columns yang dapat mengidentifikasi record secara unik dalam tabel.
    
- Primary Key
    
    Primary key adalah kumpulan satu atau lebih fields/columns dari sebuah tabel yang secara unik mengidentifikasi sebuah record dalam tabel database
    
- Alternate Key
    
    Alternate key adalah key yang bisa digunakan menjadi primary key.
    
- Unique Key
    
    Unique Key adalah kumpulan dari satu atau lebih fields/columns di sebuah table database yang secara unik mengidentifikasi sebuah record dalam table database tersebut.
    
- Foreign Key
    
    Foreign key adalah field di sebuah table database yang menjadi Primary Key di table database lain.
    

# Joining multiple tables in SQL

- INNER JOIN
    
    Semua baris akan diambil dari kedua table yang akan di JOIN, selama columns cocok dengan kondisi yang sudah di tentukan.
    
- LEFT JOIN
    
    Semua records dari table di sisi kiri JOIN statement akan di pilih. Jika record yang di pilih dari table kiri tidak memiliki record yang cocok pada table JOIN yang kanan, maka record tersebut masih dipilih, dan kolom pada table yang kanan akan bernilai NULL.
    
- RIGHT JOIN
    
    Pada JOIN ini, semua records dari table di sisi kiri JOIN statement akan di pilih, bahkan jika table di sebelah kiri tidak memiliki record yang cocok.
    

# Aggregate Function

- SUM
    
    SUM adalah fungsi untuk mengembalikan  jumlah total kolom numerik.
    
- COUT
    
    COUT adalah fungsi untuk mengembalikan jumlah baris yang cocok dengan kriteria yang ditentukan.
    
- AVG
    
    AVG adalah fungsi untuk mengembalikan rata-rata dari sebuah kolom
    

# GROUP BY dan HAVING

- GROUP BY adalah *statement* yang mengelompokkan baris yang memiliki nilai yang sama ke dalam baris ringkasan
- *Statement* GROUP BY sering digunakan dengan *aggregate function* (COUNT(), MAX(), MIN(), SUM(), AVG()) untuk mengelompokkan hasil-hasil yang ditetapkan oleh satu atau lebih kolom.
- Klausa HAVING ditambahkan ke SQL karena *keyword* WHERE tidak dapat digunakan dengan *aggregate function*.

# Autentikasi pada JavaScript

- Authentication adalah proses di mana seorang user (melalui berbagai macam akses fisik berupa komputer, dan lain-lain) mendapatkan hak akses kepada suatu entity.
- Seorang user melakukan login ke dalam suatu infrastruktur jaringan dan sistem mengenali user ID dan menerimanya untuk kemudian diberikan akses, sesuai dengan otorisasi yang dia terima.

# Otorisasi pada JavaScript

- Authorization adalah proses penentuan apakah user tersebut diizinkan / ditolak untuk melakukan satu atau beberapa action akses terhadap resources tertentu dalam sistem.
- User login terhadap sistem dengan menggunakan user-ID dan password, kemudian sistem mengenalinya dan user mendapatkan akses atau ditolak terhadap suatu resource sistem tertentu.

# JSON Web Token

- JSON Web Token adalah sebuah JSON Object yang didefinisikan dalam RFC 7519 sebagai cara aman untuk mewakili sekumpulan informasi antara dua pihak.
- Token terdiri dari Header, Content, dan Signature
- Instalasi JSON Web Token dengan npm
    
    ```jsx
    npm install jsonwebtoken
    ```
    

# Sequelize

- Sequelize adalah ORM (Object Relational Mapping) Node JS yang berbasis promise. Sequelize mendukung sebagian besar relational Database seperti MySQL, PostgresQL, MariaDB, SQLite dan Microsoft SQL Server.
- Dengan fitur-fitur di Sequelize, kita bisa mengelola dan mengatur data di database kita dengan cepat, dan efisien
- ORM adalah suatu metode/teknik pemrograman yang digunakan untuk mengkonversi data dari lingkungan bahasa pemrograman berorientasi objek (OOP) dengan lingkungan database relational.
- Instalasi Sequelize dengan npm
    
    ```jsx
    npm install -g sequelize-cli
    ```
