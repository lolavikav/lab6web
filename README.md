# Praktikum6: Twiter Bootstrap
## Nama : Lola Seftyliani
## Nim : 312410339
## Kelas : TI.24.A.4

<img width="496" height="389" alt="Screenshot 2025-10-31 073334" src="https://github.com/user-attachments/assets/2b9f4b4c-a628-4c84-a02d-396eddc3c0ae" />

# Refactor Layout Praktikum 4

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Refactor Layout Praktikum 4</title>
  <!-- Link Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" 
        rel="stylesheet" 
        integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" 
        crossorigin="anonymous">
</head>
<body>
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark mb-4">
    <div class="container-fluid">
      <a class="navbar-brand" href="#">Praktikum 6</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item">
            <a class="nav-link active" href="#">Bootstrap</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">Portofolio</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <!-- Container Utama -->
  <div class="container">
    <!-- Baris Heading -->
    <div class="row mb-4">
      <div class="col-md-4">
        <div class="card text-center">
          <div class="card-body">
            <h5 class="card-title">Heading 1</h5>
            <p class="card-text">Deskripsi singkat heading 1.</p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card text-center">
          <div class="card-body">
            <h5 class="card-title">Heading 2</h5>
            <p class="card-text">Deskripsi singkat heading 2.</p>
          </div>
        </div>
      </div>
      <div class="col-md-4">
        <div class="card text-center">
          <div class="card-body">
            <h5 class="card-title">Heading 3</h5>
            <p class="card-text">Deskripsi singkat heading 3.</p>
          </div>
        </div>
      </div>
    </div>
    <!-- Baris Konten Utama dan Sidebar -->
    <div class="row">
      <!-- Konten Utama -->
      <div class="col-md-8">
        <div class="card mb-4">
          <div class="card-body">
            <h4 class="card-title">Konten Utama</h4>
            <p class="card-text">
              Ini adalah area untuk artikel atau isi utama website.
              Anda dapat menambahkan teks, gambar, atau elemen lain di sini.
            </p>
          </div>
        </div>
      </div>
      <!-- Sidebar -->
      <div class="col-md-4">
        <div class="card mb-4">
          <div class="card-body">
            <h5 class="card-title">Sidebar</h5>
            <p class="card-text">
              Ini adalah bagian sidebar untuk link tambahan atau informasi lainnya.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- Script Bootstrap JS -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" 
          integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" 
          crossorigin="anonymous"></script>
</body>
</html>
```

Buat folder baru dengan nama `lab6_bootstrap`. lalu tambahkan file di dalamnya dengan nama `index.html` di dalam folder tersebut. Kode HTML di atas merupakan rancangan halaman web sederhana yang menggunakan Bootstrap 5 untuk membuat tampilan lebih rapi, responsif, dan modern. Struktur halaman terdiri dari tiga bagian utama, yaitu navbar, konten utama, dan sidebar, semuanya ditempatkan di dalam container Bootstrap agar memiliki tata letak yang teratur.
Pada bagian `<body>`, terdapat navbar berwarna gelap di bagian atas dengan nama “Praktikum 6” dan dua menu navigasi yaitu Home dan Artikel. Navbar ini dibuat menggunakan komponen `navbar` Bootstrap.
Selanjutnya di dalam `<div class="container">`, terdapat dua bagian utama:
1. Baris Heading `(<div class="row">)` yang berisi tiga kolom `(col-md-4)`. Masing-masing kolom menggunakan komponen `card` yang menampilkan judul “Heading 1–3” beserta deskripsi singkatnya.
2. Baris Konten Utama dan Sidebar yang terdiri dari dua kolom: kolom kiri `(col-md-8)` untuk konten utama dan kolom kanan `(col-md-4)` untuk sidebar. Keduanya juga menggunakan komponen `card` agar tampil rapi dan seragam.
Terakhir, Bootstrap JavaScript ditambahkan di bagian bawah agar fitur interaktif seperti tombol menu di navbar dapat berfungsi dengan baik. Secara keseluruhan, kode ini menampilkan layout halaman web sederhana dengan struktur grid yang bersih tanpa menggunakan CSS manual.

Hasil di browser:

<img width="1919" height="482" alt="image" src="https://github.com/user-attachments/assets/3d27bb74-931c-4251-9f74-8196e2e3b812" />

## 2. Refactor form Praktikum 5
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Form Bootstrap</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

<div class="container mt-5">
  <h3 class="text-center mb-4">Form Kontak</h3>

  <form>
    <div class="mb-3">
      <label for="nama" class="form-label">Nama Lengkap</label>
      <input type="text" class="form-control" id="nama" placeholder="Masukkan nama Anda">
    </div>

    <div class="mb-3">
      <label for="email" class="form-label">Alamat Email</label>
      <input type="email" class="form-control" id="email" placeholder="nama@contoh.com">
    </div>

    <div class="mb-3">
      <label for="pesan" class="form-label">Pesan</label>
      <textarea class="form-control" id="pesan" rows="3" placeholder="Tulis pesan Anda di sini"></textarea>
    </div>

    <button type="submit" class="btn btn-primary">Kirim</button>
  </form>
</div>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

Kode HTML di atas merupakan pembuatan form kontak sederhana dengan tampilan modern menggunakan Bootstrap 5. Struktur utamanya dimulai dengan deklarasi `<!DOCTYPE html>` dan bahasa halaman diatur ke bahasa Indonesia `(lang="id")`. Pada bagian `<head>`, terdapat meta tag untuk mengatur karakter UTF-8 dan viewport agar tampilan halaman menyesuaikan ukuran layar perangkat, sehingga form terlihat rapi baik di komputer maupun di smartphone. Selain itu, halaman juga memuat link Bootstrap dari CDN untuk memanfaatkan gaya dan komponen siap pakai tanpa harus mengunduh file tambahan.

Di dalam `<body>, terdapat sebuah container Bootstrap dengan margin atas (mt-5) agar posisi form tidak menempel di tepi atas halaman. Judul “Form Kontak” ditampilkan di tengah menggunakan kelas text-center dan diberi jarak bawah `(mb-4)`. Setelah itu terdapat elemen `<form>` yang berisi tiga input utama, masing-masing dibungkus dalam `<div class="mb-3">` untuk memberi jarak antar elemen form.
- Input pertama adalah Nama Lengkap, menggunakan tipe teks `(type="text") dengan label dan placeholder sebagai petunjuk isi.
- Input kedua adalah Alamat Email, menggunakan `type="email"` yang otomatis memvalidasi format email saat dikirim.
- Input ketiga adalah Pesan, menggunakan elemen `<textarea>` agar pengguna bisa menulis pesan lebih panjang.
Setelah ketiga elemen input, terdapat tombol “Kirim” dengan kelas `btn btn-primary` yang memberikan tampilan tombol biru khas Bootstrap. Terakhir, di bagian bawah halaman disertakan Bootstrap JavaScript bundle agar elemen interaktif Bootstrap dapat berfungsi dengan baik. Secara keseluruhan, kode ini membuat tampilan form yang bersih, profesional, dan responsif untuk digunakan pada halaman kontak sebuah website.

Hasil di browser:
<img width="1666" height="559" alt="Screenshot 2025-10-31 074351" src="https://github.com/user-attachments/assets/baefda66-284d-48ee-a624-10531d40e8c2" />
<img width="1711" height="533" alt="Screenshot 2025-10-31 074435" src="https://github.com/user-attachments/assets/e14d51e4-9c14-4828-bfa2-ff07791afd79" />

## 3. Buat Halaman Portofolio Sederhana
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfolio - Lola Seftyliani</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-dark bg-primary">
  <div class="container">
    <a class="navbar-brand" href="#">Lola Seftyliani</a>
  </div>
</nav>

<!-- Tentang Saya -->
<div class="container my-5">
  <div class="row align-items-center">
    <div class="col-md-4">
      <img src="https://picsum.photos/300" alt="Foto Saya" class="img-fluid rounded">
    </div>
    <div class="col-md-8">
      <h2>Lola Seftyliani</h2>
      <p>Hallo saya Lola Seftyliani Mahasiswa Teknik Informatika yang memiliki ingin tahu tinggi terhadap perkembangan teknologi dan senang menciptakan web..</p>
    </div>
  </div>
</div>

<!-- Portfolio -->
<div class="container my-5">
  <h3 class="text-center mb-4">Portfolio Saya</h3>
  <div class="row">
    <div class="col-md-4 mb-3">
      <div class="card">
        <img src="https://picsum.photos/400/200" class="card-img-top" alt="Project 1">
        <div class="card-body">
          <h5 class="card-title">Proyek 1</h5>
          <p class="card-text">Website profil menggunakan HTML dan Bootstrap.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4 mb-3">
      <div class="card">
        <img src="https://picsum.photos/401/200" class="card-img-top" alt="Project 2">
        <div class="card-body">
          <h5 class="card-title">Proyek 2</h5>
          <p class="card-text">Form login interaktif dengan validasi JavaScript.</p>
        </div>
      </div>
    </div>
    <div class="col-md-4 mb-3">
      <div class="card">
        <img src="https://picsum.photos/402/200" class="card-img-top" alt="Project 3">
        <div class="card-body">
          <h5 class="card-title">Proyek 3</h5>
          <p class="card-text">Dashboard admin responsif menggunakan Bootstrap Grid.</p>
        </div>
      </div>
    </div>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

Kode HTML di atas merupakan contoh halaman portfolio pribadi milik Lola Seftyliani yang dibuat menggunakan Bootstrap 5 agar tampilannya menarik dan responsif di berbagai perangkat. Struktur halaman terdiri dari tiga bagian utama, yaitu navbar, bagian tentang saya, dan bagian portfolio.

Pada bagian atas terdapat navbar berwarna biru `(bg-primary)` dengan teks putih `(navbar-dark)` yang menampilkan nama pemilik situs. Navbar ini berfungsi sebagai identitas halaman dan tetap terlihat rapi di layar besar maupun kecil karena memanfaatkan sistem grid Bootstrap.

Selanjutnya bagian “Tentang Saya” menampilkan foto dan deskripsi singkat tentang Lola sebagai mahasiswa Teknik Informatika. Layout bagian ini menggunakan dua kolom: kolom kiri menampilkan gambar profil, dan kolom kanan berisi teks perkenalan. Penggunaan kelas `align-items-center` membuat keduanya sejajar secara vertikal sehingga tampil proporsional.

Bagian terakhir adalah “Portfolio Saya”, yang menampilkan tiga proyek dalam bentuk card Bootstrap. Masing-masing card berisi gambar, judul proyek, dan penjelasan singkat seperti website profil, form login, dan dashboard admin. Susunan tiga kolom ini otomatis menyesuaikan ukuran layar agar tetap terlihat rapi dan responsif.

Di bagian paling bawah terdapat Bootstrap JavaScript bundle yang memungkinkan fitur interaktif seperti responsivitas berjalan dengan baik.

Hasil di browser:
<img width="1894" height="900" alt="Screenshot 2025-10-31 075253" src="https://github.com/user-attachments/assets/973c43d2-fd20-4c7a-ba3b-6fc6e516cb8d" />


