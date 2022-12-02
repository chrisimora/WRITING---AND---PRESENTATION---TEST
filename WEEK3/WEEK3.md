# Week 3

# Array

- *Array* adalah tipe data yang bisa menampung lebih dari satu nilai
- *Array* dapat menyimpan tipe data String, Number, Boolean, dan lainnya

## Membuat *array*

```jsx
const array_name = [item1, item2, ...];
```

## Mengakses elemen *array*

Anda mengakses elemen *array* dengan merujuk ke nomor indeks. Indeks dimulai dari angka 0. *Syntax* di bawah ini akan menampilkan elemen pertama dari *array* **animals**

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];
let animal= animals [0];
```

*Syntax* di bawah ini akan menampilkan elemen terakhir dari *array* **animals**

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];
let animal= animals [animals.length - 1];
```

## Mengubah elemen *array*

*Syntax* di bawah ini mengubah nilai elemen pertama pada *array* **animals**

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];
animals[0] = "Ayam";
```

## Menambah elemen pada *array*

*Syntax* di bawah ini akan menambahkan elemen baru ke dalam *array* (di akhir)

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];
animals.push("Singa")
```

*Syntax* di bawah ini akan menambahkan elemen baru ke dalam *array* (di awal)

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];
animals.unshift("Singa")
```

## Menghapus elemen pada *array*

*Syntax* di bawah ini akan menghapus elemen terakhir dari sebuah *array*

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];
animals.pop()
```

*Syntax* di bawah ini akan menghapus elemen pertama dari sebuah *array*

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];
animals.shift()
```

## Mengetahui panjang *array*

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];
let array_length = animals.length
```

## Menggabungkan *array*

*Syntax* di bawah ini akan menggabungkan array **animals1** dan **animals2** dan akan membentuk *array* baru yang bernama **allAnimals**

```jsx
const animals1= ["Kucing", "Bebek"];
const animals2= ["Anjing", "Harimau"];

const allAnimals= animals1.concat(animals2);
```

## Mengurutkan *array*

*Syntax* di bawah ini akan mengurutkan secara alfabetis

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];
animals.sort()
```

## Perulangan pada *array*

### forEach

forEach adalah salah satu cara untuk melakukan perulangan (*looping*) pada sebuah *array*

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];

animals.forEach(function(animals) {
    console.log(animals)
});
```

### Map

Map melakukan perulangan (*looping*) dengan membuat *array* baru

```jsx
const animals = ["Kucing", "Kelinci", "Kambing"];

 animals.map(function(animals){
   console.log(animals)
});
```

# Object

- Objek adalah tipe data yang dapat mengambil koleksi pasangan *key-value*

## Membuat objek

```jsx
const kucing = {warna:"Orange", ekor:"Panjang", jenis:"Persia"};
```

## Mengakses elemen objek

### Cara 1

```jsx
const kucing = {warna:"Orange", ekor:"Panjang", jenis:"Persia"};
console.log(kucing.warna);
```

### Cara 2

```jsx
const kucing = {warna:"Orange", ekor:"Panjang", jenis:"Persia"};
console.log(kucing["warna"]);
```

## Menambah properti pada objek

```jsx
const kucing = {warna:"Orange", ekor:"Panjang", jenis:"Persia"};
kucing.mata = "Biru"
```

## Menghapus properti

```jsx
const kucing = {warna:"Orange", ekor:"Panjang", jenis:"Persia"};
delete kucing.warna
```

# ****Recursive****

- *Recursive* adalah fungsi yang memanggil dirinya sendiri sampai kondisi tertentu.
- *Recursive* kebanyakan digunakan untuk *case* matematika, fisika, kimia, dan yang berhubungan dengan kalkulasi
    
    .
    
    Contoh penerapan *recursive*
    
    ```jsx
    
    function countDown(angka) {
    
        // tampilkan angka
        console.log(angka);
    
        // angka dikurangkan
        const angkaBaru = angka- 1;
    
        // base case
        if (angkaBaru > 0) {
            countDown(angkaBaru );
        }
    }
    
    countDown(4);
    // Hasil:
    //4
    //3
    //2
    //1
    ```
    

# Asynchronous JavaScript

- Fungsi yang berjalan secara paralel (bersamaan) dengan fungsi lain disebut *asynchronous*
    
    ```jsx
    console.log('A');
    console.log('B');
    
    setTimeout(()=>{
        console.log('C');
    },2000);
    
    console.log('D');
    ```
    

## Promises dalam JavaScript

Promises adalah sesuatu yang akan memakan waktu untuk dilakukan. Ada dua kemungkinan hasil dari sebuah promises 

- Kita bisa menjalankan dan menyelesaikan promises itu, atau
- Beberapa kesalahan terjadi dan promises ditolak
    
    ```jsx
    const getData = (dataEndpoint) => {
       return new Promise ((resolve, reject) => {
         //some request to the endpoint;
         
         if(request is successful){
           //do something;
           resolve();
         }
         else if(there is an error){
           reject();
         }
       
       });
    };
    ```
    

# Web Storage

- Dengan web storage, aplikasi web dapat menyimpan data secara lokal di dalam browser pengguna.
- Sebelum HTML5, data aplikasi harus disimpan dalam cookie, termasuk dalam setiap *server request.* Web storage lebih aman, dan data dalam jumlah besar dapat disimpan secara lokal, tanpa mempengaruhi performa situs web.
- Tidak seperti cookie, batas penyimpanan web storage jauh lebih besar (setidaknya 5MB) dan informasi tidak pernah ditransfer ke server.
- Web storage terdiri dari:
    - `localStorage`, menyimpan data tanpa kedaluwarsa
    - `sessionStorage`, menyimpan data untuk satu sesi (data hilang ketika tab browser ditutup)

## localStorage

localStorage menyimpan data tanpa tanggal kedaluwarsa. Data tidak akan dihapus ketika browser ditutup, dan akan tersedia pada hari, minggu, atau tahun berikutnya.

```jsx
localStorage.setItem("nama", "Andrian Putra Ramadan");
```

## sessionStorage

sessionStorage sama dengan localStorage, namun sessionStorage menyimpan data hanya untuk satu sesi. Data dihapus ketika pengguna menutup tab browser tertentu.

```jsx
sessionStorage.setItem("nama", "Mariana Evelin");
```
