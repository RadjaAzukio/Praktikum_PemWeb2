# PraktikumWeb2
## Langkah-langkah Praktikum
### 1. Membuat dokumen HTML
- Buatlah dokumen HTML seperti berikut
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Dasar</title>
</head>
<body>
  <header>
    <h1>CSS Internal dan <i>Inline CSS</i></h1>
  </header>
  <nav>
    <a href="lab2_css_dasar.html">CSS Dasar</a>
    <a href="lab2_css_eksternal.html">CSS Eksternal</a>
    <a href="lab1_tag_dasar.html">HTML Dasar</a>
  </nav>
  <!-- CSS ID Selector -->
  <div id="intro">
    <h1>Hello World</h1>
<p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
dan CSS.</p>
    <!-- CSS Class Selector -->
    <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
  </div>
</body>
</html>
```

- Selanjutnya buka pada brwoser untuk melihat hasilnya.

![1](https://github.com/Agussetiaa/PraktikumWeb2/assets/115542822/d161ac52-32be-4138-bf65-e0bdcb2c7a9b)


### 2. Mendeklarasikan CSS Internal
- Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen.
```
<head>
  <title>CSS Dasar</title>
  <style>
  body {
  font-family:'Open Sans', sans-serif;
  }
  header {
  min-height: 80px;
  border-bottom:1px solid #77CCEF;
  }
  h1 {
  font-size: 24px;
  color: #0F189F;
  text-align: center;
  padding: 20px 10px;
  }
  h1 i {
  color:#6d6a6b;
  }
  </style>
</head>
```

- Selanjutnya buka pada brwoser untuk melihat hasilnya.

![22](https://github.com/Agussetiaa/PraktikumWeb2/assets/115542822/c4d35cac-d4b6-45c6-9359-2adc6dc8db93)



### 3. Menambahkan Inline CSS
- Kemudian tambahkan deklarasi inline CSS pada tag ``<p>``seperti berikut.
```
<p style="color:#77CCEF">
```

- Simpan kembali dan refresh kembali browser untuk melihat perubahannya.

![3](https://github.com/Agussetiaa/PraktikumWeb2/assets/115542822/f09684e3-d62f-4b2f-8834-c61356ad1e45)


### 4. Membuat CSS Eksternal
- Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.
```
nav {
  background: #20A759;
  color:#fff;
  padding: 10px;
}
nav a {
  color: #fff;
  text-decoration: none;
  padding:10px 20px;
}
nav .active,
nav a:hover {
  background: #0B6B3A;
}
```

- Kemudian tambahkan tag ``<link>`` untuk merujuk file css yang sudah dibuat pada bagian ``<head>``
```
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- menyisipkan css eksternal -->
    <link rel="stylesheet" href="style_eksternal.css" type="text/css">
    <title>CSS Dasar</title>
</head>
```

- Selanjutnya refresh kembali browser untuk melihat perubahannya.

![44](https://github.com/Agussetiaa/PraktikumWeb2/assets/115542822/cf1e2ce2-d65b-4992-ae79-3978be11c727)


## 5. Menambahkan CSS Selector
- Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file style_eksternal.css, tambahkan kode berikut.
```
/* ID Selector */
#intro {
  background: #418fb1;
  border: 1px solid #099249;
  min-height: 100px;
  padding: 10px;
}
#intro h1 {
  text-align: left;
  border: 0;
  color: #fff;
}
/* Class Selector */
.button {
  padding: 15px 20px;
  background: #bebcbd;
  color: #fff;
  display: inline-block;
  margin: 10px;
  text-decoration: none;
}
.btn-primary {
  background: #E42A42;
}
```

-Kemudian simpan kembali dan refresh browser untuk melihat perubahannya.

![5](https://github.com/Agussetiaa/PraktikumWeb2/assets/115542822/b0921aca-bc6a-416a-bc7d-26f8e68a1eed)


# Pertanyaan dan Tugas
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
![66](https://github.com/Agussetiaa/PraktikumWeb2/assets/115542822/5f2a2c47-074b-4c95-8451-8e3296f0807a)


2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan penjelasannya!
- Kalau h1 menggunakan internal dan inline pada penggunaan style nya sedangkan intro menggunakan eksternal css style nya
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!
- Semuanya akan tampil tergantung penyebutnya contohnya pada gambar no 1
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ( p id="paragraf-1" class="text-paragraf" )
- Di praktek Hari ini keduanya tampil tapi berbeda
