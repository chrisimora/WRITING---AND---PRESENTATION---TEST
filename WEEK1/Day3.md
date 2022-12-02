# Day 3

# Cascading Style Sheet (CSS)

## Apa itu CSS?

- CSS adalah sebuah bahasa yang digunakan untuk mempercantik dan memberi gaya (*styling*) halaman HTML
- Dengan CSS, kita bisa mengubah warna, menggunakan *font custom*, mengedit format teks, mengatur tata letak, dan lainnya
- CSS pertama kali diperkenalkan pada tahun 1996

## Struktur CSS

```css
.selector{
  properti: nilai;
}
```

- *Selector* menunjuk ke elemen HTML apa yang ingin dipercantik atau diberi gaya
- Nama properti CSS dan nilai, dipisahkan dengan titik dua

## Komentar pada CSS

```css
/* Ini adalah komentar*/
p {
  font-size: 15px;
}
```

- Komentar CSS tidak ditampilkan di peramban web, tetapi dapat membantu memberi penjelasan mengenai kode CSS yang dibuat.

## Cara Memanggil file CSS ke dalam file HTML

### External CSS

- Dengan CSS eksternal, Kita bisa mengubah tampilan seluruh situs web hanya dengan mengubah satu *file*
- Setiap halaman HTML harus menyertakan referensi ke CSS eksternal di dalam elemen < link >, di dalam elemen < head >
- CSS eksternal dapat ditulis dalam *text editor* apa pun, dan harus disimpan dengan ekstensi .css
    
    ```html
    <!DOCTYPE html>
    <html>
    	<head>
    		<link rel="stylesheet" href="mystyle.css">
    	</head>
    	<body>
    		<h1>This is a heading</h1>
    		<p>This is a paragraph.</p>
    	</body>
    </html>
    ```
    

### **Internal CSS**

- CSS internal dapat digunakan jika satu halaman HTML tunggal memiliki gaya yang unik.
- CSS internal dibuat di dalam elemen < style >, di dalam elemen < head >
    
    ```html
    <!DOCTYPE html>
    <html>
    	<head>
    		<style>
    		body {
    		  background-color: linen;
    		}
    		
    		h1 {
    		  color: maroon;
    		  margin-left: 40px;
    		}
    		</style>
    	</head>
    	<body>
    	
    	<h1>KKN di Desa Penari/h1>
    	<p>KKN di Desa Penari adalah film horor dari Indonesia</p>
    	
    	</body>
    </html>
    ```
    

### Inline CSS

- CSS Inline dapat digunakan untuk memberikan gaya unik untuk satu elemen.
- Untuk menggunakan CSS Inline tambahkan atribut style ke elemen yang relevan. Atribut gaya dapat berisi properti CSS apa pun.
    
    ```html
    <!DOCTYPE html>
    <html>
    	<body>
    		<h1 style="color:blue;text-align:center;">Indonesia/h1>
    		<p style="color:red;">Indonesia adalah negara kepulauan/p>
    	</body>
    </html>
    ```
    

## Selector pada CSS

- Selector CSS digunakan untuk menemukan atau memilih elemen HTML yang ingin diberi gaya atau dipercantik.
- Selector CSS dapat dibagi ke dalam lima kategori:
    - Simple Selector (memilih elemen berdasarkan nama elemen, id, class)
    - Combinator Selector (memilih elemen berdasarkan hubungan spesifik antar elemen)
    - Pseudo-class Selector (memilih elemen berdasarkan keadaan tertentu)
    - Pseudo-elements Selector (memilih dan memberi gaya pada bagian dari sebuah elemen)
    - Attribute Selector (memilih elemen berdasarkan atribut atau nilai atribut)

### Selector berdasarkan nama elemen

```css
h1 {
  text-align: center;
  color: blue;
}
```

### Selector berdasarkan id

- Selector id menggunakan atribut id dari elemen HTML untuk memilih suatu elemen
- Id dari sebuah elemen adalah unik di dalam sebuah halaman, jadi selector id digunakan untuk memilih satu elemen yang unik
- Untuk memilih elemen dengan id tertentu, ketikkan karakter hash (#), diikuti dengan id elemen.
    
    ```css
    #judul_pertama{
     font-size:20px;
    	background-color:red;
    }
    ```
    

### Selector berdasarkan nama

- Selector class memilih elemen HTML dengan atribut class tertentu.
- Untuk memilih elemen dengan class tertentu, tulis karakter titik (.), diikuti dengan nama class.
    
    ```css
    .foto_profil{
      width:100px;
    }
    ```
    

### Universal Selector

Selector universal (*) memilih semua elemen HTML pada halaman.

```css
* {
 background-color : red;
}
```

### Chaining Selectors

Chaining selector dapat kita gunakan pada case/kasus berikut. Jika kita memiliki 3 tag elemen HTML pada CSS namun kita ingin ada 1 elemen HTML yang memiliki styling berbeda

```css
h1 {
color : green;
}

h1.judul_pertama {
color : blue;
}
```

**Grouping Selector**

- Grouping selector memilih semua elemen HTML dengan *styling* yang sama.
- Untuk membuat grouping selector, pisahkan setiap selector dengan koma.
    
    ```css
    h1, h2, p {
      font-weight: bold;
      color: blue;
    }
    ```
    

## CSS !important

- !important CSS berada di level paling atas dari ID dan Class.
- Jika pada *styling* CSS kita menggunakan !important, maka *styling* sebelumnya baik itu id, nama elemen atau nama kelas akan di-*override*

## Sekian dan Terima Kasih

Christian Galileo Simamora

Medan, 28 November 2022
