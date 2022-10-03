---
title: "HTML5 Dasar"
weight: 1
---

# Pendahuluan

Artikel ini berisi penilaian tugas biodata yang dibuat dalam waktu 10-15 menit menggunakan html, berdasarkan sudut pandang **Sofa Machabba Haeta**. Penilaian dilakukan oleh 2 orang, saya dan **Koordinator Divisi Website**.

Akan tetapi, penilaian yang dipublikasi tidak berupa nilai atau angka, melainkan sebatas komentar berupa kelebihan dan kekurangan dari *syntax*, *semantic*, atau tampilan.

# Kriteria Penilaian
1. Sesuai dengan perintah yang diberikan atau kreativitas pribadi.
2. Tidak menyalahi aturan penulisan dan penggunaan.
3. Tertata rapi dan terbaca jelas. 

# Daftar Penilaian

## Sabdayagra Ahessa

{{< details "Dokumentasi">}}
{{< figure align=center src="/assets/praktik-teco/html5-dasar/Sabdayagra-Ahessa.png" width="100%">}}
{{< /details >}}

<br>

{{< details "Sumber Data">}}

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width,initial 
 scale=1.0">
  <link rel="stylesheet" href="style.css">
  <title> </title>
</head>

<body>
  
  <div class="caption">
    <p>Nama : Sabdayagra Ahessa</p>
    <p>Kelas : X PPLG</p>
    <P>No Absen : 30 </P>
  </div>


  <div class="caption">
    <h2>Hobby</h2>
    <ul>
      <li>bersepeda</li>
      <li>Main Game</li>
    </ul>
  </div>
  <div class="caption">
    <h2>Keinginan</h2><br>
    <p>Menjadi Back End Website Developer</p>
  </div>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/prettier/2.7.1/standalone.js"></script>
</body>

</html>
```

<br>

```css
* {
    margin: 0;
    padding: 0;
    font-family: sans-serif;
    color: #d1d1d1;
}

body{
    margin: auto;
    background-color: #0f172a;
}

.header{
    text-align: center;
    margin: 32px 0;
}

.profiles{
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    margin: 0 auto;
    max-width: 768px;
}

.caption{
    padding: 24px;
}

.caption p{
    color: #b9b9b9;
}
```
{{< /details >}}

<br>

{{< details "Fitur dan Kelebihan">}}
1. Memakai tag *heading*, *paragraph* dan *lists*.
2. Memakai tag blok, *link* dan *script*.
3. Menggunakan *Cascading Style Sheets*.
{{< /details >}}

<br>

{{< details "Saran dan Masukan">}}
1. Kalau bisa, kedepannya jangan sampai tidak mengisi tag `<title>` pada bagian *header*.
```html
  <title> </title>
```

2. Apa tujuan memasukan library *prettier v2.7.1*? Kalau tidak ada fungsinya, mending dihapus saja. Untuk projek berskala kecil, bukan menjadi masalah jika tidak menggunakan *code formating*. Kalau mau "pamer", pilih library yang dapat dilihat jelas, seperti *bootstrap* atau *font-awesome*.
```html
  <script src="https://cdnjs.cloudflare.com/ajax/libs/prettier/2.7.1/standalone.js"></script>
```

3. Selain itu, diharap dapat melihat perbedaan antara baris baru dan baris yang menyambung. Seperti contoh berikut :

**Baris baru**
```html {linenos=table,hl_lines=[4]}
...
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width,initial 
 scale=1.0">
<link rel="stylesheet" href="style.css">
...
```

**Baris yang menyambung**
```html {linenos=table,hl_lines=[3]}
...
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width,initial scale=1.0">
<link rel="stylesheet" href="style.css">
...
```

4. Pada proyek berskala kecil, ketika ada 3 tag menggunakan *style* yang sama. Alangkah baiknya tidak memakai atribut *class*, melainkan langsung memanggil tag tersebut. Jika ingin "pamer", saran saya digunakan pada judul. Sebagai contoh :


```html {linenos=table,hl_lines=[2,"6-7",13]}
  ...
  <div>
    <p>...</p>
  </div>

  <div>
    <h2 class="punyaku12cm">...</h2>
    <ul>
      <li>...</li>
    </ul>
  </div>

  <div>
    <h2>...</h2>
    <p>...</p>
  </div>
  ...
```

```css {linenos=table,hl_lines=["2-4",6,10]}
...
.punyaku12cm {
    color: #ff0;
}

div {
    padding: 24px;
}

div p {
    color: #b9b9b9;
}
...
```
{{< /details >}}

## Fadlan Abduh Erman Nawa

{{< details "Dokumentasi">}}
  {{< figure align=center src="/assets/praktik-teco/html5-dasar/Fadlan-Abduh-Erman-Nawa.png" width="100%">}}
{{< /details >}}

<br>

{{< details "Sumber Data">}}
```html
<!DOCTYPE html>
<html>

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Teco</title>
</head>

<body>
  <table>
    <tr>
      <td width="72">Nama</td>
      <td>Fadlan Abduh Erman Nawa</td>
    </tr>
    <tr bgcolor="#eaeaea">
      <td>Kelas</td>
      <td>X PPLG 1</td>
    </tr>
    <tr>
      <td>No Absen</td>
      <td>11</td>
    </tr>
    <tr bgcolor="#eaeaea">
      <td>Deskripsi Diri</td>
      <td>Hi! Saya Fadlan Abduh, dan ini adalah bagian deskripsi pribadi saya. Apa yang harus ditulis pada bagian deskripsi pribadi ? Apakah menyebutkan nama saja cukup untuk mendeskripsikan diri saya ? Sepertinya tidak... <br> Anyway, saya rasa rentetan pertanyaan saya tadi sudah cukup untuk mendeskripsikan diri saya. Ya, saya punya banyak pertanyaan yang terpendam di dalam otak saya.</td>
    </tr>
    <tr>
      <td>Hobi</td>
      <td>Mendengarkan Musik</td>
    </tr>
  </table>

  
</body>

</html>
```
{{< /details >}}

<br>

{{< details "Fitur dan Kelebihan">}}
1. Memakai tag tabel
2. Mendekorasi tabel dengan CSS
{{< /details >}}

<br>

{{< details "Saran dan Masukan">}}
1. Sangat tidak disarankan menulis atribut *width* pada tag `<tr>`, karena efek visual yang dihasilkan tidak maksimal. Lebih jelasnya berikut adalah [daftar tag yang bisa dikasih atribut *width* (***W3School | English***)](https://www.w3schools.com/tags/att_width.asp).

Kesalahan :
```html
<td width="72">...</td>
```

Perbaikan alternatif :
```html
<td>...</td>
```

2. Apabila ingin mendekorasi tag, gunakan metode ***Inline CSS*** yaitu menambahkan atribut ***style*** yang diisi kode CSS. Hal ini berkaitan pada fitur terbaru dari HTML5.

Kesalahan :
```html {linenos=table,hl_lines=[5,11]}
...
  <tr> 
    <td>...</td>
  </tr>
  <tr bgcolor="#eaeaea">
    <td>...</td>
  </tr>
  <tr> 
    <td>...</td>
  </tr>
  <tr bgcolor="#eaeaea">
    <td>...</td>
  </tr>
...
```

Perbaikan alternatif :
```html {linenos=table,hl_lines=[5,11]}
...
  <tr> 
    <td>...</td>
  </tr>
  <tr style="background-color: #eaeaea">
    <td>...</td>
  </tr>
  <tr> 
    <td>...</td>
  </tr>
  <tr style="background-color: #eaeaea">
    <td>...</td>
  </tr>
...
```

3. Jika ingin mendekorasi *table-row* atau `<tr>` hanya pada kolom genap (kolom ke-2, kolom ke-4, dst), gunakan metode CSS internal atau eksternal. Hal ini sangat berguna apabila memiliki puluhan atau ratusan *table-row*.

Kesalahan :
```html {linenos=table,hl_lines=[5,11]}
...
  <tr> 
    <td>...</td>
  </tr>
  <tr bgcolor="#eaeaea">
    <td>...</td>
  </tr>
  <tr> 
    <td>...</td>
  </tr>
  <tr bgcolor="#eaeaea">
    <td>...</td>
  </tr>
...
```

Perbaikan alternatif :

```css {linenos=false}
table tr:nth-child(odd|even) { /* odd: ganjil, even: genap*/
  background-color: #eaeaea;
}
```

Contoh CSS internal :

```html {linenos=table,hl_lines=["5-9",16,22]}
<!-- index.html -->
...
<head>
  ...
  <style>
    table tr:nth-child(even) {
      background-color: #eaeaea;
    }
  </style>
</head>
<body>
  <table>
    <tr> <!-- Tidak ada Background -->
      <td>...</td>
    </tr>
    <tr> <!-- Background #eaeaea -->
      <td>...</td>
    </tr>
    <tr> <!-- Tidak ada Background -->
      <td>...</td>
    </tr>
    <tr> <!-- Background #eaeaea -->
      <td>...</td>
    </tr>
  </table>
</body>
...
```

Contoh CSS eksternal :

```html {linenos=table,hl_lines=[5,12,18]}
<!-- index.html -->
...
<head>
  ...
  <link rel="stylesheet" href="index.css">
</head>
<body>
  <table>
    <tr> <!-- Tidak ada Background -->
      <td>...</td>
    </tr>
    <tr> <!-- Background #eaeaea -->
      <td>...</td>
    </tr>
    <tr> <!-- Tidak ada Background -->
      <td>...</td>
    </tr>
    <tr> <!-- Background #eaeaea -->
      <td>...</td>
    </tr>
  </table>
  ...
<body>
...
```

```css {linenos=table,hl_lines=["2-4"]}
/* index.css */
table tr:nth-child(even) {
  background-color: #eaeaea;
}
```
{{< /details >}}

## Muhammad Aji Mauliddinar

{{< details "Dokumentasi">}}
{{< figure align=center src="/assets/praktik-teco/html5-dasar/Muhammad-Aji-Mauliddinar.png" width="100%">}}
{{< /details >}}

<br>

{{< details "Sumber Data">}}
```html
<!DOCTYPE html>
<html>

<head>
  <title>Biodata Teco</title>

</head>

<body>
  <p>NAMA: Muhammad Aji Mauliddinar</p>
  <p>TTL : PEMALANG 31-03-2007</p>
  <p>NO ABSEN : 23</p>
  <p>Kelas : X PPLG</p>
  <p>
    Deskripsi Pribadi : Saya murid dari SMKN 01 Pemalang, saya berasal dari
    jurusan PPLG, dan saya suka menonton anime dan membaca komik.
  <h3>Hobby:</h3>
  <ul type="disc">
    <li>Membaca komik</li>
    <li>Nonton anime</li>
    <li>Makan</li>
    <li>Main Genshin</li>
    <li>Mendengarkan musik</li>
    <li>Tidur</li>
  </ul>
  </p>
</body>

</html>
```
{{< /details >}}

<br>

{{< details "Fitur dan Kelebihan">}}
1. Menggunakan *heading*, *paragraph* dan *lists*
2. Mendekorasi *lists* dengan CSS *inline*.
{{< /details >}}

<br>

{{< details "Saran dan Masukan">}}
1. Kedepannya diharap dapat membedakan tag berdasarkan kategori. Tidak semua elemen bisa berisi tag, seperti `<ul>` atau `<ol>` dimana mereka mampu menampung `<li>` didalamnya. Sedangkan tag `<p>` memiliki sifat "*Phrasing Content*" , dimana tidak boleh ada tag apapun di dalam tag `<p>`. Lebih lengkapnya silahkan [lihat dokumentasi berikut ***(MDN | English)***](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/Content_categories).

Kesalahan :
```html {linenos=table,hl_lines=["3-13"]}
...
  <p>
    Deskripsi Pribadi : Saya murid dari SMKN 01 Pemalang, saya berasal dari
    jurusan PPLG, dan saya suka menonton anime dan membaca komik.
  <h3>Hobby:</h3>
  <ul type="disc">
    <li>Membaca komik</li>
    <li>Nonton anime</li>
    <li>Makan</li>
    <li>Main Genshin</li>
    <li>Mendengarkan musik</li>
    <li>Tidur</li>
  </ul>
  </p>
...
```

Perbaikan alternatif :
```html {linenos=table,hl_lines=["3-4","7-15"]}
...
  <p>
    Deskripsi Pribadi : Saya murid dari SMKN 01 Pemalang, saya berasal dari
    jurusan PPLG, dan saya suka menonton anime dan membaca komik.
  </p>

  <h3>Hobby:</h3>
  <ul type="disc">
    <li>Membaca komik</li>
    <li>Nonton anime</li>
    <li>Makan</li>
    <li>Main Genshin</li>
    <li>Mendengarkan musik</li>
    <li>Tidur</li>
  </ul>
...
```

2. Untuk apa menulis *default style type* pada tag `<ul>`? Lebih baik dihapus, atau menggunakan tipe lainnya. Berikut merupakan [daftar lengkap tipe tag `<ul>` atau `<ol>` ***(W3School | English)***](https://www.w3schools.com/cssref/pr_list-style-type.asp).

Kesalahan :
```html {linenos=table,hl_lines=2}
...
  <ul type="disc">
    ...
  </ul>
...
```

Perbaikan alternatif :
```html {linenos=table,hl_lines=[3,8]}
...
  <!-- Default Style -->
  <ul>
    ...
  </ul>

  <!-- Square Style -->
  <ul type="square">
    ...
  </ul>
...
```
{{< /details >}}

## Kania Ariskum Mahesti

{{< details "Dokumentasi">}}
{{< figure align=center src="/assets/praktik-teco/html5-dasar/Kania-Ariskum-Mahesti.png" width="100%">}}
{{< /details >}}

<br>

{{< details "Sumber Data">}}
```html
<!DOCTYPE html>
<html>
  <head>
    <title>BIODATA></title>
  </head>
  <body>
    <h1>BIODATA</h1>
   Nama: KANIA ARSIKUM MAHESTI<br>
    Kelas: X TJKT 1<br>
    Umur: 15thn<br>
    Hobi: Baca komik<br>
    <p>
      Deskripsi:<br>
      Manusia yang betah di dikamar,padahal kalo di rumah yaa dimarahin ortu :v
    </p>
    
  </body>
</html>
```
{{< /details >}}

<br>

{{< details "Fitur dan Kelebihan">}}
1. Menggunakan *heading*, *paragraph* dan *Line Breaks*.
{{< /details >}}

<br>

{{< details "Saran dan Masukan">}}
1. Sebisa mungkin mengkategorikan suatu bagian menggunakan tag. Jangan sampai ada bagian yang tidak terkategori, hal ini sangat merugikan ketika bekerja dengan JavaScript.

Kesalahan :
```html {linenos=table,hl_lines=["2-5"]}
...
   Nama: KANIA ARSIKUM MAHESTI<br>
    Kelas: X TJKT 1<br>
    Umur: 15thn<br>
    Hobi: Baca komik<br>
...
```
Bagian nama, kelas, umur dan hobi tidak berada di dalam tag apapun, sehingga sulit dijangkau ketika bekerja dengan JavaScript.

Perbaikan alternatif :
```html {linenos=table,hl_lines=["3-6",9,14]}
...
  <!-- Memakai tag P -->
  <p>Nama: KANIA ARSIKUM MAHESTI</p>
  <p>Kelas: X TJKT 1</p>
  <p>Umur: 15thn</p>
  <p>Hobi: Baca komik</p>

  <!-- Memakai tag DIV -->
  <div>
    Nama: KANIA ARSIKUM MAHESTI<br>
    Kelas: X TJKT 1<br>
    Umur: 15thn<br>
    Hobi: Baca komik<br>
  </div>
...
```
{{< /details >}}
## Satria Nur Alfata Panca

{{< details "Dokumentasi">}}
{{< figure align=center src="/assets/praktik-teco/html5-dasar/Satria-Nur-Alfata-Panca.png" width="100%">}}
{{< /details >}}

<br>

{{< details "Sumber Data">}}
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>data diri</title>
</head>

<body>
  <p>Nama: Satria Nur Alfata Panca</p>
  <p>Kelas : X PPLG</p>
  <p> Asal : Petarukan, Pemalang</p>
  <p>Hobi : sedang di cari</p>
  <p>Bakat : Terpendam</p>
  <h3>FOLLOW IG @satrialfata</h3>
</body>

</html>
```
{{< /details >}}

<br>

{{< details "Fitur dan Kelebihan">}}
1. Menggunakan tag *heading* dan *paragraph*
{{< /details >}}

<br>

{{< details "Saran dan Masukan">}}
1. Jika ingin **memperbesar** dan **menebalkan** teks/tulisan, **JANGAN** memakai *heading*. Gunakan fitur bahasa CSS sebagai dekorasi.

Kesalahan :
```html
<h3>FOLLOW IG @satrialfata</h3>
```
Perbaikan alternatif :
```html
<!-- Default H3 stylesheet -->
<p style="font-size: 1.17em; font-weight: bolder">FOLLOW IG @satrialfata</p>
```
{{< /details >}}

## Nadia Febriana

{{< details "Dokumentasi">}}
{{< figure align=center src="/assets/praktik-teco/html5-dasar/Nadia-Febriana.png" width="100%">}}
{{< /details >}}

<br>

{{< details "Sumber Data">}}
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Biodata Diri</title>
  </head>
  <body>
    <p>Nama:Nadia Febriana</p>
    <p>Kelas:X PPLG</p>
    <P>Deskripsi hobby:Nama saya nadia febriana dari kelas 10 PPLG biasa dipanggil nadia </P>
  </body>
</html>
```
{{< /details >}}

<br>

{{< details "Fitur dan Kelebihan">}}
1. Menggunakan tag *paragraph*
{{< /details >}}

<br>

{{< details "Saran dan Masukan">}}
1. Sebisa mungkin **JANGAN** menggunakan huruf besar pada nama tag.

Kesalahan :
```html
<P>Deskripsi hobby:Nama saya nadia febriana dari kelas 10 PPLG biasa dipanggil nadia </P>
```

Perbaikan alternatif :
```html
<!-- Default H3 stylesheet -->
<p>Deskripsi hobby:Nama saya nadia febriana dari kelas 10 PPLG biasa dipanggil nadia</p>
```
{{< /details >}}

## Hanif Maulana S.

{{< details "Dokumentasi">}}
{{< figure align=center src="/assets/praktik-teco/html5-dasar/Hanif-Maulana-S.png" width="100%">}}
{{< /details >}}

<br>

{{< details "Sumber Data">}}
```html
<!DOCTYPE html>
<html>
  <head>
    <title>BIODATA DIRI</title>
  </head>
  <body>
    <h1 align="center">BIODATA</h1>
    <p>Nama     : Hanif Maulana S</p>
    <p>Kelas    : X PPLG</p>
    <p>No Absen : 14</p>
    <p>Hobi     : Mabar</p>
    <p>Alamat : Tentunya Di Pemalang</p>
    <p>Deskripsi: </p>
    <p>Halo Gais , Saya Hanif Maulana S ,tentunya saya baik hati dan tidak sombong,saya hobinya mabar tapi cupu sih hehehe ,sekian terimakasih.</p>
  </body>
</html>
```
{{< /details >}}

<br>

{{< details "Fitur dan Kelebihan">}}
1. Menggunakan *heading* dan *paragraph*
2. Mendekorasi *heading* dengan CSS *inline*
{{< /details >}}

<br>

{{< details "Saran dan Masukan">}}
1. Apabila ingin merubah posisi teks agar *center* (rata tengah), gunakan CSS inline berdasarkan fitur CSS terbaru.

Kesalahan :
```html
<h1 align="center">BIODATA</h1>
```

Perbaikan alternatif :
```html
<h1 style="text-align: center">BIODATA</h1>
```
{{< /details >}}

## Bayu Suryo Nur Cahyo

{{< details "Dokumentasi">}}
{{< figure align=center src="/assets/praktik-teco/html5-dasar/Bayu-Suryo-NurCahyo.png" width="100%">}}
{{< /details >}}

<br>

{{< details "Sumber Data">}}
```html
<!DOCTYPE html>
<html lang="en">
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<head>
  <title>kaizel</title>
  <style>
    .para {
      text-align: justify;
      margin-right: auto;
      margin-left: auto;
      font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    }
  </style>
</head>

<body>
  <p class="para">
    Nama : Bayu Suryo NurCahyo<br>
    Kelas : X PPLG<br>
    Asal : Sewaka,Pemalang<br>
    Hobi : Suka Membaca,Bermain Game <br>
    Bakat : Belum ketemu
  </p>
</body>

</html>
```
{{< /details >}}

<br>

{{< details "Fitur dan Kelebihan">}}
1. Menggunakan *paragraph* dan *Line Breaks*
2. Mendekorasi *paragraph* dengan CSS internal
{{< /details >}}

<br>

{{< details "Saran dan Masukan">}}
1. Tag `<meta>` seharusnya berada di dalam tag `<head>` 

Kesalahan :
```html {linenos=table,hl_lines=["3-5"]}
<!DOCTYPE html>
<html lang="en">
<meta charset="UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<head>
  ...
</head>
```

Perbaikan alternatif :
```html {linenos=table,hl_lines=["5-7"]}
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  ...
</head>
```

2. Alangkah lebih baik untuk tidak menggunakan rata kanan-kiri (*justify align*) pada paragraf yang singkat. Dan tidak mengatur *margin* kanan dan kiri dengan nilai otomatis, karena secara *default* nilainya adalah 0. Apabila ingin mengatur *margin* secara otomatis, maka harus ada faktor pendukung, seperti salah satu sisinya harus memiliki nilai, atau berada pada kontainer khusus. Akan tetapi, ketika ingin membuat posisi *paragraph* berada di tengah tanpa mengubah *align* menjadi rata tengah, bisa menggunakan contoh berikut :

```html {linenos=table,hl_lines=["7-9"]}
...
<head>
  ...
  <style>
    p {
      text-align: justify;
      margin: auto;
      width: 50%;
      max-width: fit-content;
      font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    }
  </style>
</head>
<body>
  <p>
    Nama : Bayu Suryo NurCahyo<br>
    Kelas : X PPLG<br>
    Asal : Sewaka,Pemalang<br>
    Hobi : Suka Membaca,Bermain Game <br>
    Bakat : Belum ketemu
  </p>
</body>
...
```

3. Jangan sembarangan memilih huruf (*font*), karena setiap *font* memiliki keunikan tersendiri. Selalu memilih *font* berdasarkan kebutuhan agar dapat memperindah dan tidak merusak tampilan. Berikut [visualisasi untuk melihat perbedaan antara *Lucida Sans*, *Lucida Sans Regular*, *Lucida Grande*, *Lucida Sans Unicode*, *Geneva*, *Verdana*, *sans-serif*. (***CSS Font Stack | English***)](https://www.cssfontstack.com/Lucida-Grande)

{{< figure align=center src="/assets/praktik-teco/html5-dasar/other/cssfontstack.png" width="100%">}}
{{< /details >}}

## Ridwan Fahmi Aldiansyah

{{< details "Dokumentasi">}}
{{< figure align=center src="/assets/praktik-teco/html5-dasar/Ridwan-Fahmi-Aldiansyah.png" width="100%">}}
{{< /details >}}

<br>

{{< details "Sumber Data">}}
```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>data diri</title>
</head>

<body>
  <h1 align="center">BIODATA DIRI</h1>
  <table border="1" cellspacing="0" callpadding="5" align="center" width="800">
    <tr align="center" bgcalor="#95F586">
      <td width="200">DATA DIRI</td>
      <td width="400">KETERANGAN</td>
    </tr>
    <tr>
      <td align="center">NAMA</td>
      <td align="center">Ridwan Fahmi Aldiansyah</td </tr>
    <tr>
      <td align="center">TEMPAT/TANGGAL LAHIR</td>
      <td align="center">Pemalang,30 oktober 2006</td>
    </tr>
    <tr>
      <td align="center">ALAMAT</td>
      <td align="center">JL.urip sumoharjo rt 05 rw 09</td>
    </tr>
    <tr>
      <td align="center">AGAMA</td>
      <td align="center">Islam</td>
    </tr>
    <tr>
      <td align="center">JENIS KELAMIN</td>
      <td align="center">Laki-Laki</td>
    </tr>
    <tr>
      <td align="center">SEKOLAH</td>
      <td align="center">SMKN 1 pemalang</td>
    </tr>
    <tr>
      <td align="center">HOBI</td>
      <td align="center">Jalan-Jalan</td>
    </tr>
  </table>
</body>

</html>

```
{{< /details >}}

<br>

{{< details "Fitur dan Kelebihan">}}
1. Menggunakan tag `<table>` beserta jajarannya.
2. Mendekorasi tabel dengan CSS inline.
{{< /details >}}

<br>

{{< details "Saran dan Masukan">}}
> Karena ada banyak *typo* pada **Sumber Data** di atas, dengan ini saya mencoba untuk membuat ulang dengan desain yang sama persis. Hanya saja menggunakan metode CSS internal, agar mudah dibaca dan dipahami.

{{< details "Tutorial">}}

1. Mengetik ulang semua tag tanpa adanya *inline style*.
```html {linenos=table,hl_lines=["2","5","8-42"]}
<!DOCTYPE html>
<html lang="id">
  <head>
    ...
    <style></style>
  </head>
  <body>
    <h1>BIODATA DIRI</h1>
    <table>
      <tr>
        <th>DATA DIRI</th>
        <th>KETERANGAN</th>
      </tr>
      <tr>
        <td>NAMA</td>
        <td>Sofa Machabba Haeta</td>
      </tr>
      <tr>
        <td>TEMPAT, TANGGAL LAHIR</td>
        <td>Pemalang, XX Desember 2003</td>
      </tr>
      <tr>
        <td>ALAMAT</td>
        <td>Bojongbata, Kec. Pemalang, Kab. Pemalang</td>
      </tr>
      <tr>
        <td>AGAMA</td>
        <td>Islam</td>
      </tr>
      <tr>
        <td>JENIS KELAMIN</td>
        <td>Laki-Laki</td>
      </tr>
      <tr>
        <td>SEKOLAH</td>
        <td>SMKN 1 pemalang</td>
      </tr>
      <tr>
        <td>HOBI</td>
        <td></td>
      </tr>
    </table>
  </body>
</html>
```

2. Menambahkan dekorasi CSS secara berkala, dimulai dari tag *heading*.
```html {linenos=table,hl_lines=["4-7","11"]}
...
<head>
  ...
  <style>
    h1 {
      /* Membuat tulisan rata tengah */
      text-align: center
    }
  </style>
</head>
<body>
  <h1>BIODATA DIRI</h1>
  ...
</body>
...
```

3. Menambahkan dekorasi CSS khusus untuk tabel.
```html {linenos=table,hl_lines=["5-15", "20"]}
...
<head>
  ...
  <style>
    ...
    table {
      /* Mengatur panjang tag tabel */
      width: 800px;

      /* Mengatur lebar spasi bingkai */
      border-spacing: 0;

      /* Mengatur margin tabel agar rata tengah */
      margin-left: auto;
      margin-right: auto;
    }
  </style>
</head>
<body>
  ...
    <table>
      ...
    </table>
</body>
...
```

4. Menambahkan dekorasi CSS khusus untuk *table-row* pertama dan *table-head*.
```html {linenos=table,hl_lines=["5-28","34-37"]}
...
<head>
  ...
  <style>
    ...
    /* Menyeleksi table-row pertama */
    /* Memberi warna latar #95F586 pada table-row */
    tr:first-child {
      background-color: #95F586
    }

    /* Menyeleksi table-head pertama */
    /* Mengatur panjang table-head pertama */
    th:first-child {
      width: 200px
    }

    /* Menyeleksi table-head terakhir */
    /* Mengatur panjang table-head terakhir */
    th:last-child {
      width: 400px
    }

    /* 
     * Catatan:
     * Saya mengunakan first dan last child pada tag <th>,
     * karena memang hanya ada 2 tag. Apabila terdapat lebih
     * dari 2 tag, saran saya gunakan `tag:nth-child({number})`.
     */
  </style>
</head>
<body>
  ...
    <table>
      <tr>
        <th>DATA DIRI</th>
        <th>KETERANGAN</th>
      </tr>
      <tr>
        <td>...</td>
        <td>...</td>
      </tr>
      ...
    </table>
</body>
...
```

5. Menambahkan dekorasi CSS untuk *table*, *table-head* dan *table-data*.
```html {linenos=table,hl_lines=["5-18","22-32"]}
...
<head>
  ...
  <style>
    ...
    /* Menyeleksi semua table-head dan semua table-data */
    /* Mengatur padding pada semua tag th dan td */
    th, td {
      padding: 5px;
    }

    /* Menyeleksi table, semua table-head dan semua table-data */
    table, th, td {
      /* Memberi bingkai solid sebesar 1px */
      border: 1px solid;

      /* Membuat tulisan rata tengah */
      text-align: center;
    }
  </style>
</head>
<body>
    <table>
      <tr>
        <th>...</th>
        <th>...</th>
      </tr>
      <tr>
        <td>...</td>
        <td>...</td>
      </tr>
      ...
    </table>
</body>
...
```
{{< /details >}}

<br>

{{< details "Dokumentasi Tutorial">}}
{{< figure align=center src="/assets/praktik-teco/html5-dasar/Sofa-Machabba-Haeta.png" width="100%">}}
{{< /details >}}

<br>

{{< details "Sumber Data Tutorial">}}
```html
<!DOCTYPE html>
<html lang="id">

<head>
  <meta http-equiv="Content-Type" content="text/html;charset=UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="author" content="Sofa Machabba Haeta">
  <meta name="email" content="mail@sofa.my.id">
  <meta name="website" content="https://sofa.my.id/">
  <meta name="description" content="Sebuah perbaikan kode dari tugas praktik HTML5 milik Ridwan Fahmi Aldiansyah oleh Sofa Machabba Haeta.">
  <meta name="language" content="Indonesia">
  <title>Biodata Diri</title>
  <style>
    h1 {
      text-align: center;
    }
    table {
      width: 800px;
      border-spacing: 0;
      margin-left: auto;
      margin-right: auto;
    }
    tr:first-child {
      background-color: #95F586;
    }
    th:first-child {
      width: 200px;
    }
    th:last-child {
      width: 400px;
    }
    th, td {
      padding: 5px;
    }
    table, th, td {
      border: 1px solid;
      text-align: center;
    }
  </style>
</head>

<body>
  <h1>BIODATA DIRI</h1>
  <table>
    <tr>
      <th>DATA DIRI</th>
      <th>KETERANGAN</th>
    </tr>
    <tr>
      <td>NAMA</td>
      <td>Sofa Machabba Haeta</td>
    </tr>
    <tr>
      <td>TEMPAT, TANGGAL LAHIR</td>
      <td>Pemalang, XX Desember 2003</td>
    </tr>
    <tr>
      <td>ALAMAT</td>
      <td>Bojongbata, Kec. Pemalang, Kab. Pemalang</td>
    </tr>
    <tr>
      <td>AGAMA</td>
      <td>Islam</td>
    </tr>
    <tr>
      <td>JENIS KELAMIN</td>
      <td>Laki-Laki</td>
    </tr>
    <tr>
      <td>SEKOLAH</td>
      <td>SMKN 1 pemalang</td>
    </tr>
    <tr>
      <td>HOBI</td>
      <td></td>
    </tr>
  </table>
</body>

</html>
```
{{< /details >}}

{{< /details >}}

# Penutup

Demikian penilaian dari saya, mungkin ada banyak nama yang tidak tercantum pada daftar di atas. Beberapa alasan diantaranya, karena :

- Tidak ada kesalahan, baik penulisan maupun tampilan.
- Ada kesalahan, akan tetapi tidak terlalu fatal dan sudah dibahas pada salah satu siswa yang terpilih.
- Kurang menarik untuk dibahas, entah karena *copy-paste* kode milik orang lain, atau tidak adanya kreativitas.

Adapun alasan siswa yang terpilih untuk saya nilai pada situs ini, diantaranya :
- Menarik untuk dibahas, entah karena kreativitas dalam mencoba hal baru atau sekedar "pamer".
- Sangat banyak kesalahan baik yang sering terjadi hingga yang dapat berakibat fatal.

Apabila ada yang ingin ditanyakan lebih lanjut, dapat melalui grup WhatsApp, atau *Direct Message*.