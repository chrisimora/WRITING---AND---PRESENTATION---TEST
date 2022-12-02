# Day 2

# Hypertext Markup Language (HTML)

## Apa itu HTML

- Sederhananya, HTML adalah sebuah bahasa yang digunakan untuk membuat konten dan struktur dari halaman sebuah situs web
- Versi pertama HTML ditulis oleh [Tim Berners-Lee](https://en.wikipedia.org/wiki/Tim_Berners-Lee) pada tahun 1993
- Versi terbaru HTML saat ini adalah HTML5. Versi ini merupakan versi yang direkomendasikan oleh World Wide Web Consortium (W3C)
- HTML5 pertama kali dirilis dalam ke publik pada tanggal 22 Januari 2008

## *Tools* yang harus dipersiapkan untuk membuat HTML

- Peramban Web (*Web Browser*), peramban web digunakan untuk menampilkan konten HTML
    - [Chrome](https://www.google.com/chrome/)
    - [Microsoft Edge](https://www.microsoft.com/en-us/edge)
    - [Firefox](https://www.mozilla.org/en-US/firefox/new/)
    - [Opera](https://www.opera.com/browsers/opera)
    - [Brave](https://brave.com/)
- *Text Editor*, text editor digunakan untuk menulis atau mengetikkan kode HTML
    - [Visual Studio Code](https://code.visualstudio.com/download), dikembangkan oleh Microsoft
    - [Sublime Text](https://www.sublimetext.com/)
    - [Atom](https://atom.io/), dikembangkan oleh GitHub
    - [Bracket](https://brackets.io/), dikembangkan oleh Adobe
    - [Notepad++](https://notepad-plus-plus.org/downloads/)

## Struktur HTML

```html
<!DOCTYPE html>
<html>
<head>
	<title>Judu Halaman/title>
</head>
<body>
	<h1>Judul Teks</h1>
	<p>Isi Paragraf</p>
</body>
</html>
```

- <!DOCTYPE html> menyatakan bahwa kode HTML yang dibuat menggunakan versi HTML5
- < html > menyatakan elemen akar dari halaman HTML
- < head > berisi informasi meta tentang halaman HTML
- < title > digunakan untuk membuat judul halaman HTML
- < body > menyatakan badan HTML, dan merupakan wadah untuk semua konten yang terlihat, seperti judul, paragraf, gambar, *hyperlink*, tabel, *list*, dan lain-lain.
- < h1 > digunakan membuat judul besar
- < p > digunakan untuk menyatakan paragraf

## Elemen HTML

Elemen HTML terdiri dari *tag* pembuka, kontennya, dan *tag* penutup.

```html
<tagname> Isi konten </tagname>
```

Contoh Elemen HTML

```html
<h1> Judul Besar </h1>
<p> Ini adalah paragraf </p>
```

## Atribut HTML

Atribut merupakan properti dari sebuah elemen HTML

```html
<tagname attribute="value"> Isi konten </tagname>
```

- Semua elemen HTML bisa memiliki atribut
- Atribut selalu diletakkan pada *tag* pembuka sebuah elemen
- Semua atribut yang bisa dipakai untuk elemen HTML bisa dilihat melalui [tautan](https://www.w3schools.com/tags/ref_attributes.asp) berikut ini

Contoh Atribut HTML

```html
<a href="google.com">Klik di sini untuk membuka Google </a>
```

## Komentar pada HTML

- Komentar adalah sebuah teks yang tidak akan tampil pada peramban web (*web browser*).
- Komentar digunakan untuk memberikan penjelasan lebih lengkap tentang kode HTML yang ditulis
    
    ```html
    <!-- Ketikkan komentar di sini -->
    ```
    
    > Perhatikan bahwa terdapat tanda seru (!) pada *tag* pembuka, tetapi tidak ada pada *tag* penutup.
    > 
    
    Contoh 
    
    ```html
    <!-- Ini adalah komentar. Komentar tidak akan tampil di peramban web (*web browser*) -->
    ```
    

## Ekstensi Live Server pada Visual Studio Code

- Setiap kita menuliskan kode HTML, kita harus me-*refresh* halaman web tersebut di peramban web (*web browser*) untuk menampilkan kode yang telah dibuat. Hal tersebut akan sangat merepotkan karena harus berulang kali me-*refresh* halamannya
- Solusi dari permasalahan tersebut adalah dengan menginstal ekstensi yang bernama **Live Server** pada Visual Studio Code
- Ekstensi Live Server memiliki fitur *live reload* yang memungkinkan kita untuk tidak berulang kali me-*refresh* halaman web

## *Tag* HTML Populer

- < p >, digunakan untuk membuat paragraf
- < h1 > - < h6 >, digunakan untuk membuat judul besar
- < i > atau < em >, digunakan untuk membuat teks miring
- < b > atau < strong >, digunakan untuk menebalkan teks
- < a >, digunakan untuk membuat *hyperlink*
- < hr >, digunakan untuk membuat garis pemisah horizontal
- < img >, digunakan untuk memanggil gambar
- < video >, digunakan untuk memanggil video
- < table >, digunakan untuk membuat tabel
- < form >, digunakan untuk membuat form

## Elemen Semantik pada HTML

- Elemen semantik adalah elemen yang memiliki arti.
- Terdapat beberapa *tag* semantik yang dapat digunakan untuk mendefinisikan bagian yang berbeda dari halaman web
    - < article >
    - < aside >
    - < details >
    - < figcaption >
    - < figure >
    - < footer >
    - < header >
    - < main >
    - < mark >
    - < nav >
    - < section >
    - < summary >
    - < time >
- Kegunaan menggunakan elemen semantik adalah meningkatkan aksesibilitas, meningkatkan SEO, serta lebih mudah di-*maintain*

## Deploy HTML

- Deploy adalah sebuah proses untuk menyebarkan atau mengunggah kode ke web server agak bisa di akses oleh banyak orang
- Kode HTML bisa disebarkan atau diunggah melalui layanan berikut
    - Netlify
    - GitHub Pages
    - Firebase
    - Microsoft Azure

## Sekian dan Terima kasih

Medan, 28 September 2022

Christian Galileo Simamora
