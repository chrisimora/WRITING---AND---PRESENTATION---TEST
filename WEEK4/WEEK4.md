# Week 4

# Asynchronous - Fetch

Fetch API adalah *interface* modern yang memungkinkan kita membuat ********request******** ke server HTTP dari *web browser*, untuk membuat ********request********, diperlukan fungsi khusus yang bernama fetch()

Contoh penggunaan fungsi fetch()

```jsx
async function getMovies() {
  const response = fetch('https://api.themoviedb.org/3/discover/movie?api_key=0a03a21e889f7f720b11bba9f7532337&sort_by=popularity.desc').then((response) => response.json()).then((data) => {
    console.log(data)
  })
}

// Panggil fungsi
getMovies();
```

# Asynchronous - Async Await

Cara yang lebih baik dan lebih bersih untuk menangani *promise* adalah dengan ********keyword******** async/await. Bisa dimulai dengan menentukan fungsi pemanggil sebagai async dan kemudian menggunakan await untuk menangani promise.

```jsx
async function getMovies() {
  const response = await fetch(
    "https://api.themoviedb.org/3/discover/movie?api_key=0a03a21e889f7f720b11bba9f7532337&sort_by=popularity.desc"
  );
  const data = await response.json();
  console.log(data);
}

// Panggil fungsi
getMovies();
```

# Git

- Git adalah sebagai *Version Control System* dan dapat melacak setiap perubahan yang terjadi pada suatu folder atau *file*.
- *Version Control System* bertugas untuk mencatat setiap perubahan pada File (termasuk code yang kita buat) pada suatu proyek baik dikerjakan secara individu maupun tim.

## Perintah-perintah pada Git

- git init
    
    Perintah ini digunakan untuk membuat repositori lokal baru
    
- git status
    
    Perintah ini digunakan untuk menampilkan status *****************working directory***************** dan ************staging area************ 
    
- git add
    
    Perintah ini digunakan untuk menambahkan perubahan dari ******************working directory****************** ke ************staging area************
    
- git commit
    
    Perintah ini digunakan untuk menyimpan perubahan ke repositori lokal
    
- git log
    
    Perintah ini digunakan meninjau dan membaca riwayat segala sesuatu yang terjadi pada repositori
    
- git checkout
    
    Perintah ini digunakan untuk berpindah ******branch******
    
- git reset
    
    Perintah ini digunakan untuk membatalkan perubahan
    
- git revert
    
    Perintah ini membatalkan perubahan pada riwayat *******commit******* repositori
    
- git branch
    
    Perintah ini berguna untuk membuat, melihat, mengganti nama, dan menghapus ******branch******
    
- git merge
    
    Perintah digunakan untuk menggabungkan dua ******branch******
    

# Responsive Web Design

- Desain web responsif adalah membuat halaman web yang terlihat bagus di semua perangkat
- Desain web yang responsif akan secara otomatis menyesuaikan ukuran layar dan viewport yang berbeda
- Desain web responsif menggunakan HTML dan CSS agar secara otomatis mengubah ukuran, menyembunyikan, mengecilkan, atau memperbesar, sebuah situs web, agar terlihat bagus di semua perangkat (desktop, tablet, dan ponsel)

## Mengatur viewport

- Untuk membuat situs web yang responsif, tambahkan tag <meta> berikut ke semua halaman web
    
    ```html
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    ```
    
- *Syntax* di atas akan menetapkan viewport halaman web, yang akan memberikan instruksi browser tentang cara mengontrol dimensi dan penskalaan halaman.

## Gambar Responsif

- Gambar responsif adalah gambar yang berskala baik agar sesuai dengan ukuran browser apa pun.
- Kita dapat menggunakan properti width
    
    ```html
    <img src="img_girl.jpg" style="width:100%;">
    ```
    
- Kita juga dapat menggunakan properti max-width
    
    Jika properti max-width ditetapkan ke 100%, gambar akan diperkecil skalanya jika harus, tetapi tidak pernah diperkecil skalanya menjadi lebih besar daripada ukuran aslinya
    
    ```html
    <img src="img_girl.jpg" style="max-width:100%;height:auto;">
    ```
    

## Ukuran Teks Responsif

- Ukuran teks bisa ditetapkan dengan unit "vw", yang berarti "viewport width"
- Dengan unit tersebut ukuran teks akan mengikuti ukuran jendela browser
    
    ```html
    <h1 style="font-size:10vw">Hello World</h1>
    ```
    

# Media Queries

- Selain mengubah ukuran teks dan gambar, juga umum untuk menggunakan *media query* di halaman web responsif.
- Dengan *media query*, Kita dapat menentukan *style* yang sama sekali berbeda untuk ukuran browser yang berbeda.
- Contoh: ubah ukuran jendela browser untuk melihat bahwa tiga elemen div di bawah ini akan ditampilkan secara horizontal pada layar yang besar dan menumpuk secara vertikal pada layar yang kecil
    
    ```css
    <style>
    .left, .right {
      float: left;
      width: 20%; /* The width is 20%, by default */
    }
    
    .main {
      float: left;
      width: 60%; /* The width is 60%, by default */
    }
    
    /* Use a media query to add a breakpoint at 800px: */
    @media screen and (max-width: 800px) {
      .left, .main, .right {
        width: 100%; /* The width is 100%, when the viewport is 800px or smaller */
      }
    }
    </style>
    ```
    

# Bootstrap

- Bootstrap adalah *framework* CSS gratis dan *open-source* yang ditujukan untuk pengembangan web *front-end* yang responsif dan *mobile-first*.
- Bootstrap pertama kali dirilis pada 19 Agustus 2011 oleh Mark Otto, Jacob Thornton
- Bootstrap berisi *template* desain berbasis HTML, CSS, dan (opsional) JavaScript untuk tipografi, *form*, tombol, navigasi, dan komponen *interface* lainnya.
- Jadi, dengan Bootstrap kita tidak perlu berpikir untuk membuat web itu responsif, karena Bootstrap sudah responsif

## Layout

*Grid system* Bootstrap menggunakan serangkaian *********container*********, *row*, dan *column* untuk menata dan menyelaraskan konten. Sistem ini dibangun dengan flexbox dan sepenuhnya responsif. Di bawah ini adalah contoh dan penjelasan mendalam tentang bagaimana g*rid system* disatukan

```html
<div class="container text-center">
  <div class="row">
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
    <div class="col">
      Column
    </div>
  </div>
</div>
```

Contoh di atas membuat tiga *column* dengan lebar yang sama di semua perangkat dan *viewport* menggunakan *grid class* yang telah ditentukan sebelumnya. Kolom-kolom tersebut dipusatkan di halaman dengan *parent* .container.

## Konten

Konten pada Bootstrap terdiri atas:

- Reboot
- Typography
- Images
- Tables
- Figures

Selengkapnya kamu bisa lihat di halaman [berikut ini](https://getbootstrap.com/docs/5.2/content/)

## Komponen

Beberapa komponen pada Bootstrap adalah sebagai berikut:

- Accordion
- Alerts
- Badge
- Breadcrumb
- Buttons
- Button group
- Card
- Carousel
- Close button
- Collapse
- Dropdowns
- List group
- Modal
- Navbar
- Navs & tabs
- Offcanvas
- Pagination
- Placeholders
- Popovers
- Progress
- Scrollspy
- Spinners
- Toasts
- Tooltips
