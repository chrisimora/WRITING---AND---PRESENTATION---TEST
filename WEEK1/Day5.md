# Day 5

# JavaScript Dasar

## Apa itu JavaScript

- JavaScript adalah bahasa pemrograman yang sangat powerful yang digunakan untuk logic pada sebuah website
- JavaScript juga dapat membuat website menjadi interaktif dan dinamis
- JavaScript berjalan di setiap peramban web (*web browser*) **karena setiap peramban web sudah memiliki JavaScript di dalamnya

## Console log pada JavaScript

Console log mencetak pesan ke web console. Pesan dapat berupa string, atau dapat berupa satu atau lebih objek JavaScript

```jsx
console.log("Hello world!");
```

## Komentar pada JavaScript

- Komentar adalah teks yang tidak akan dieksekusi oleh JavaScript. Komentar sangat berguna untuk memberikan penjelasan terkait kode JavaScript yang ditulis.
- Komentar pada JavaScript terdiri dari 2 yaitu single line dan multi-line
    
    ### Komentar Single Line
    
    - Komentar single line dimulai dengan //.
    - Teks apa pun antara // dan akhir baris akan diabaikan oleh JavaScript (tidak akan dieksekusi).
        
        ```jsx
        // Perintah untuk menampilkan teks Hello World ke konsol
        console.log("Hello world!");
        ```
        
    
    ### Komentar Multi-line
    
    - Komentar multi-line dimulai dengan /* dan diakhiri dengan */.
    - Teks apa pun di antara /* dan */ akan diabaikan oleh JavaScript.
        
        ```jsx
        /*
        Perintah di bawah ini
        untuk menampilkan teks Selamat Malam ke konsol
        */
        console.log("Selamat Malam")
        ```
        
    

## Tipe Data pada JavaScript

Ada 6 tipe data fundamental pada JavaScript

- Numbers
    - JavaScript hanya memiliki satu jenis angka.
    - Numbers bisa ditulis dengan, atau tanpa desimal
        
        ```jsx
        let phi= 3.14;     // Ditulis dengan desimal
        let diameter= 31;  // Ditulis tanpa desimal
        ```
        

- String
    - String adalah serangkaian karakter seperti "Hello World.
    - String ditulis dengan tanda kutip, bisa menggunakan tanda kutip tunggal atau ganda
        
        ```jsx
        let ucapan = "Selamat Malam";   // Menggunakan tanda kutip ganda
        let ucapan2 = 'Selamat Sore;   // Menggunakan tanda kutip tunggal
        ```
        

- Boolean
    - Boolean adalah jenis tipe data yang hanya memiliki 2 nilai yaitu true atau false
        
        ```jsx
        let benar = true;
        let salah = false;
        ```
        

- Null
    - Tipe data null adalah tipe data yang diartikan bahwa sebuah variable/data tidak memiliki nilai
    - Null berbeda dengan string kosong. String kosong masih memiliki tipe data string
        
        ```jsx
        let ini_null = null;
        ```
        
    
- Undefined
    - Dalam JavaScript, variabel tanpa nilai, memiliki nilai undefined. Jenisnya juga tidak terdefinisi.
        
        ```jsx
        let halo;    // Nilainya tidak ada, jenisnya pasti undefined
        ```
        

- Object
    - Objek JavaScript ditulis dengan tanda kurung kurawal {}.
    - Properti objek ditulis sebagai pasangan nama:nilai, dipisahkan dengan koma.
        
        ```jsx
        const orang= {namaPertama:"Andrian", namaAkhir:"Ramadan", umur:19, jenisKelamin:"Laki-Laki"};
        ```
        

## Variabel pada JavaScript

- Variabel adalah tempat menampung data
- Terdapat 4 cara untuk membuat variabel
    - Menggunakan var
        
        ```jsx
        var x = 1;
        var y = 5;
        var z = x + y;
        ```
        
    - Menggunakan let
        
        ```jsx
        let nama = "Andrian Ramadan";
        ```
        
    - Menggunakan const
        
        ```jsx
        const phi = 3.14;
        ```
        
    
    ### Kapan menggunakan var?
    
    - var digunakan pada JavaScript dari tahun 1995 sampai 2015
    - let dan const ditambahkan ke JavaScript pada tahun 2015
    - Jika ingin kodenya berjalan di *browser* lama, harus menggunakan var.
    
    ### Kapan menggunakan let?
    
    - Penggunaan var sudah tidak direkomendasikan dan juga sudah lawas oleh karena itu para disarankan menggunakan let
    
    ### Kapan menggunakan const?
    
    - Jika ingin menampung nilai variabel yang tidak berubah atau konstan, seperti phi, kamu bisa gunakan const

## Jenis Operator pada JavaScript

- Ada berbagai jenis operator JavaScript:
    - Operator Aritmetika
    - Operator Penugasan
    - Operator Perbandingan
    - Operator Logika
    - Operator Kondisional
    - Operator Tipe

### Operator Aritmatika JavaScript

| Operator | Deskripsi |
| --- | --- |
| + | Penjumlahan |
| - | Pengurangan |
| * | Perkalian |
| ** | Eksponensiasi (ES2016) |
| / | Pembagian |
| % | Modulus (Sisa Bagi) |
| ++ | Increment |
| -- | Decrement |

### Operator Penugasan JavaScript

| Operator | Contoh | Sama Seperti |
| --- | --- | --- |
| = | x = y | x = y |
| += | x += y | x = x + y |
| -= | x -= y | x = x - y |
| *= | x *= y | x = x * y |
| /= | x /= y | x = x / y |
| %= | x %= y | x = x % y |
| **= | x **= y | x = x ** y |

### Operator Perbandingan JavaScript

| Operator | Deskripsi |
| --- | --- |
| == | sama dengan |
| === | nilai yang sama dan tipe yang sama |
| != | tidak sama |
| !== | tidak sama nilainya atau tidak sama jenisnya |
| > | lebih besar dari |
| < | kurang dari |
| >= | lebih besar dari atau sama dengan |
| <= | kurang dari atau sama dengan |
| ? | operator terner |

### Operator Perbandingan JavaScript

| Operator | Deskripsi |
| --- | --- |
| && | logika dan |
| || | logika or |
| ! | logika not |
|  |  |

### Operator Tipe JavaScript

| Operator | Deksripsi |
| --- | --- |
| typeof | Mengembalikan tipe variabel |
| instanceof | Mengembalikan nilai true jika sebuah objek adalah instance dari sebuah tipe objek |

## Kondisional

- Kondisional merupakan statement percabangan yang menggambarkan suatu kondisi
- Statement kondisional akan mengecek kondisi spesifik dan menjalankan perintah berdasarkan kondisi tersebut
- Dalam JavaScript ada beberapa statement kondisional yaitu sebagai berikut:
    - if, untuk menentukan blok kode JavaScript yang akan dieksekusi jika suatu kondisi benar.
        
        ```jsx
        if (umur > 18) {
          console.log("Memasukan kedewasaan");
        }
        ```
        
    - else, untuk menentukan blok kode yang akan dieksekusi, jika kondisi yang sama salah
        
        ```jsx
        if (umur > 18) {
          console.log("Memasuki fase kedewasaan");
        }else
        {
        	console.log("Memasuki fase anak-anak");
        }
        ```
        
    - else if, untuk menentukan kondisi baru untuk diuji, jika kondisi pertama salah
        
        ```jsx
        if (umur > 18) {
          console.log("Memasuki fase kedewasaan");
        }else if(umur > 50){
        	console.log("Memasuki fase lansia");
        }else
        {
        	console.log("Memasuki fase anak-anak");
        }
        ```
        
    - switch, untuk menentukan banyak blok kode alternatif yang akan dieksekusi
        
        ```jsx
        let nilai = "A"
        switch(expression) {
          case "A":
            console.log("Sangat Baik")
            break;
          case "B":
            console.log("Baik")
            break;
        	case "C":
        	  console.log("Cukup")
        	  break;
        	case "D":
        		 console.log("Buruk")
        		 break;
          default:
            console.log("Tidak ada")
        }
        ```
        

## Perulangan (Looping)

- Looping adalah statement yang mengulang sebuah instruksi hingga kondisi terpenuhi atau jika kondisi stop/berhenti tercapai.
- Ada beberapa cara untuk melakukan looping
    - FOR LOOP
        
        ```jsx
        // Kode dibawah ini akan menampilkan angka 1 - 5
        for (let i = 1; i <= 5; i++) {
          console.log(i)
        }
        ```
        
    - WHILE LOOP
        
        ```jsx
        // Kode dibawah ini akan menampilkan angka 1 - 10
        let i = 1;
        while (i <= 10) {
         console.log(i)
          i++;
        }
        ```
        
    - DO WHILE
        
        ```jsx
        // Kode dibawah ini akan menampilkan angka 1 - 10
        let i = 1;
        do {
        console.log(i)
          i++;
        }
        while (i <= 10);
        ```
        
    

## Sekian dan Terima Kasih

Christian Galileo Simamora

Medan, 28 November 2022
