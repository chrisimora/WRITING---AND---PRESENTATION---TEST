# Week 2

# Scope in JavaScript

- Scope adalah konsep dalam flow data variabel. Menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.
- Blocks adalah code yang berada di dalam curly braces {}
- Conditional, function, dan looping menggunakan blocks.
- Global scope berarti variabel yang kita buat dapat diakses di mana pun dalam suatu file.
    
    ```jsx
    let umur = 15;
    
    function cetakUmur()
    {
    	return "Umur saya adalah " + umur;
    }
    
    console.log(cetakUmur());
    ```
    
- Local scope berarti kita mendeklarasikan variabel di dalam blocks seperti function, conditional, dan looping.
    
    ```jsx
    function cetakUmur()
    {
    	let umur = 15;
    	return "Umur saya adalah" +  umur;
    }
    console.log(umur) // Uncaught ReferenceError: umur is not definedFunction in JavaScript
    ```
    

## Function in JavaScript

- Function adalah blok kode yang dirancang untuk melakukan tugas tertentu.
- Function akan dieksekusi ketika dipanggil.
- Function dibuat dengan *keyword* function, diikuti dengan nama *function*-nya, diikuti dengan tanda kurung ().
- Nama function bisa berisi huruf, angka, garis bawah, dan tanda dolar (aturan yang sama seperti variabel).
    
    ```jsx
    function nama(parameter1, parameter2, parameter3) {
      // kode yang akan dieksekusi
    }
    ```
    
- Parameter function  dicantumkan di dalam tanda kurung () saat membuat function.
- Argumen function adalah nilai yang diterima oleh function ketika dipanggil.
- Kode di dalam function akan dieksekusi ketika "sesuatu" memanggil function tersebut:
    - Ketika suatu *event* terjadi (ketika pengguna mengklik tombol)
    - Ketika dipanggil dari kode JavaScript
    - Secara otomatis (dipanggil sendiri)

```jsx
//deklarasi function pada JavaScript
function cetakSelamat()
{
	console.log("Selamat Siang, Andrian Putra Ramadan")
}
```

- Cara memanggil function cukuplah mudah, kita tinggal tulis saja nama *function*-nya dengan tanda kurung ()
    
    ```jsx
    //deklarasi function pada JavaScript
    function cetakSelamat()
    {
    	console.log("Selamat Siang, Andrian Putra Ramadan")
    }
    
    cetakSelamat(); // memanggil function
    ```
    
- Function juga bisa mengembalikan sebuah nilai yang telah diproses oleh function tersebut
    
    ```jsx
    // function untuk menghitung luas persegi
    function luasPersegi(sisi)
    {
    	return s * s;
    }
    
    // panggil fungsi dengan mengisi argumen luas perseginya
    console.log(luarPersegi(4))
    ```
    
- Parameter default adalah parameter yang dipakai ketika function tidak diberikan argumen
    
    ```jsx
    // function untuk menghitung luas persegi dengan parameter default sisi = 0;
    function luasPersegi(s = 0)
    {
    	return s * s;
    }
    
    // kode tidak akan error ketika function tidak diberikan argumen
    console.log(luasPersegi())
    ```
    
- Function Helper adalah kita memanggil *function* yang sudah dibuat pada function lain.
    
    ```jsx
    function luasPersegi(s = 0)
    {
    	return s * s;
    }
    
    function volumeKubus(s)
    {
    return luasPersegi() * s;
    }
    
    console.log(volumeKubus(2))
    ```
    
- Arrow function diperkenalkan pada ES6. Arrow function membuat deklarasi function menjadi lebih cepat
    
    ```jsx
    // function di bawah ini mengembalikan string selamat siang
    hello = () => {
      return "Selamat Siang";
    }
    ```
    
- Jika hanya memiliki satu *statement,* dan *statement* mengembalikan nilai, kita bisa menghapus tanda kurung () dan keyword return
    
    ```jsx
    hello = () => "Hai, Nama saya Andrian";
    ```
    

.

- Jika function memiliki parameter, kita bisa meletakkan parameter tersebut di dalam tanda kurung
    
    ```jsx
    LuasPersegi = (sisi) => sisi * sisi;
    ```
    
- Bahkan, jika hanya memiliki satu parameter, kita bisa menghapus tanda kurung juga
    
    ```jsx
    CetakUmur = umur=> "Umur kamu adalah " + umur;
    ```
    

# Tipe Data pada JavaScript

- Tipe Data Primitif adalah semua tipe data kecuali objek yang menyatakan nilai immutable (nilai yang tidak bisa diubah). Tipe data immutable adalah tipe data yang tidak dapat dimodifikasi dan diubah (misalnya menambahkan elemen baru, menghapus elemen, mengganti elemen). Berikut yang merupakan tipe data primitif
    - **Boolean**
        
        Boolean adalah tipe data yang hanya dapat memiliki dua nilai: true dan false
        
    - **Null**
        
        Dalam JavaScript, null artinya "tidak ada".
        
    - **Undefined**
        
        Variabel yang belum diberi nilai memiliki nilai undefined (tidak terdefinisi)
        
    - **Number**
        
        ECMAScript memiliki dua tipe numerik bawaan: Number dan BigInt
        
        - Numbers
            
            Tipe data dapat menyimpan bilangan bulat dan desimal. Tipe data ini mampu menyimpan angka floating-point positif antara 2^-1074 dan 2^1024 serta angka floating-point negatif antara -(2^-1074) dan -(2^1024), tetapi hanya dapat menyimpan bilangan bulat dengan aman dalam rentang -(2^53 - 1)  hingga 2^53 - 1.
            
        - BigInt
            
            BigInt adalah tipe data numerik dalam JavaScript yang dapat merepresentasikan bilangan bulat dengan presisi bebas. Dengan BigInt, kita dapat menyimpan dan mengoperasikan bilangan bulat besar dengan aman bahkan melebihi batas bilangan bulat yang aman untuk Numbers.
            
    - **String**
        
        String digunakan untuk menampung rangkaian karakter
        
    - **Symbol**
        
        Symbol adalah tipe data primitif yang unik dan tidak dapat diubah dan dapat digunakan sebagai kunci dari properti Objek
        
- Tipe Data Non Primitif
    - Object
    - Array
    - Function

# String pada JavaScript

String digunakan untuk menyimpan dan memanipulasi teks.

- Menampilkan panjang string
    
    ```jsx
    let nama = "Andrian Putra Ramadan";
    let length = text.nama;
    ```
    
- Mengekstrak Bagian String
    
    slice() mengekstrak bagian dari string dan mengembalikan bagian yang diekstrak dalam string baru.
    
    ```jsx
    let makanan = "Nasi Padang, Sate, Ketoprak";
    let part = makanan.slice(13);
    console.log(part)
    ```
    
- Mengganti Konten String
    
    ```jsx
    let ucapan = "Selamat Malam";
    let ucapanBaru = ucapan.replace("Malam", "Siang");
    
    console.log(ucapanBaru);
    ```
    
- Mengonversi ke Huruf Besar dan Kecil
    - Konversi ke Huruf Besar
        
        ```jsx
        let teks1= "Selamat Datang";
        let teks2= teks1.toUpperCase();
        
        console.log(teks2)
        ```
        
    - Konversi ke Huruf Kecil
        
        ```jsx
        let teks1= "Selamat Datang";
        let teks2= teks1.toLowerCase();
        
        console.log(teks2)
        ```
        
- Menggabungkan string
    
    ```jsx
    let ucapan= "Selamat";
    let waktu= "Malam";
    let ucapanBaru= ucapan.concat(" ", waktu);
    
    console.log(ucapanBaru)
    ```
    

- Mengekstrak Karakter String
    
    ```jsx
    let teks = "INDONESIA";
    let char = teks.charAt(0);
    
    // mengekstrak karakter string dengan index 0
    console.log(char )
    ```
    
- Mengonversi String ke Array
    
    ```jsx
    let teks = "a,b,c,d,e,f";
    let arraybaru= teks.split(",");
    
    console.log(arraybaru)
    
    ```
    

# Numbers pada JavaScript

- Konversi angka menjadi string
    
    ```jsx
    let angka = 123;
    console.log(angka.toString());
    
    ```
    
- Mengonversi Variabel menjadi Angka
    
    ```jsx
    let umur = "12";
    console.log(Number(umur));
    ```
    

# JavaScript Math

JavaScript Math memungkinkan kita untuk melakukan tugas matematika pada angka.

## Math Properties

```jsx
Math.E // mengembalikan bilangan Euler
Math.PI // mengembalikan PI
Math.SQRT2 // mengembalikan akar kuadrat dari 2
Math.SQRT1_2 // mengembalikan akar kuadrat dari 1/2
Math.LN2 // mengembalikan logaritma natural dari 2
Math.LN10 // mengembalikan logaritma natural dari 10
Math.LOG2E // mengembalikan logaritma basis 2 dari E
Math.LOG10E // mengembalikan logaritma basis 10 dari E
```

## Math Method

```jsx
Math.round(x) // Mengembalikan x dibulatkan ke bilangan bulat terdekatnya
Math.ceil(x) // Mengembalikan x dibulatkan ke bilangan bulat terdekatnya
Math.floor(x) // Mengembalikan x dibulatkan ke bawah ke bilangan bulat terdekatnya
Math.trunc(x) // Mengembalikan bagian integer dari x (baru di ES6)
Math.pow(x, y) // mengembalikan nilai x ke pangkat y
Math.sqrt(x) // mengembalikan akar kuadrat dari x
Math.abs(x) // mengembalikan nilai absolut (positif) dari x
Math.sin(x) // mengembalikan sinus (nilai antara -1 dan 1) dari sudut x (dalam radian)
Math.cos(x) // mengembalikan kosinus (nilai antara -1 dan 1) dari sudut x (dalam radian)
Math.min() Math.max() //dapat digunakan untuk menemukan nilai terendah atau tertinggi dalam daftar argumen
Math.random() // mengembalikan angka acak antara 0 (inklusif), dan 1 (eksklusif);
```

# DOM

- Dengan DOM HTML, JavaScript dapat mengakses dan mengubah semua elemen dokumen HTML
- Ketika halaman web dimuat, browser menciptakan Document Object Model dari halaman tersebut.
- Dengan Object Model, JavaScript mendapatkan semua kekuatan yang dibutuhkan untuk membuat HTML dinamis
- Berikut yang bisa dilakukan oleh DOM
    - JavaScript dapat mengubah semua elemen HTML dalam halaman
    - JavaScript dapat mengubah semua atribut HTML dalam halaman
    - JavaScript dapat mengubah semua styling CSS di halaman
    - JavaScript dapat menghapus elemen dan atribut HTML yang ada
    - JavaScript dapat menambahkan elemen dan atribut HTML baru
    - JavaScript dapat bereaksi terhadap semua *event* HTML yang ada di halaman
    - JavaScript dapat membuat *event* HTML baru di halaman

## Sintaks pada DOM

Contoh sederhana implementasi DOM pada HTML

```html
<html>
<body>

<p id="nama"></p>

<script>
	document.getElementById("demo").innerHTML = "Andrian Putra Ramadan";
</script>

</body>
</html>
```

### Menemukan Elemen HTML

| Metode | Deskripsi |
| --- | --- |
| document.getElementById(id) | Menemukan elemen berdasarkan id-nya |
| document.getElementsByTagName(name) | Menemukan elemenen berdasarkan nama tag-nya |
| document.getElementsByClassName(name) | Menemukan elemen berdasarkan nama kelasnya |

### Mengubah Elemen HTML

| Properti | Deskripsi |
| --- | --- |
| element.innerHTML =  new html content | Mengubah inner HTML dari sebuah elemen |
| element.attribute = new value | Mengubah nilai atribut dari sebuah elemen HTML |
| element.style.property = new style | Mengubah style dari sebuah elemen HTML |
| Metode | Deskripsi |
| element.setAttribute(attribute, value) | Mengubah nilai atribut dari sebuah elemen HTML |

### Menambah dan Menghapus Elemen

| Metode | Deskripsi |
| --- | --- |
| document.createElement(element) | Membuat elemen HTML |
| document.removeChild(element) | Menghapus elemen HTML |
| document.appendChild(element) | Menambahkan elemen HTML |
| document.replaceChild(new, old) | Mengganti elemen HTML |
| document.write(text) | Menulis ke dalam output stream HTML |

### Menambahkan event handler

| Metode | Deskripsi |
| --- | --- |
| document.getElementById(id).onclick = function(){code} | Menambahkan kode event handler kepada event onclick |
|  |  |
