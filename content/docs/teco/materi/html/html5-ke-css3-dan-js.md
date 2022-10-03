---
title: "HTML5 ke CSS3 dan JS"
weight: 2
---

## Pengertian
HTML, CSS dan JS merupakan satu kesatuan yang saling melengkapi dan menjadi sumber utama untuk membuat situs atau _website_.

Situs masih dapat berfungsi apabila tidak memiliki salah satu dari mereka, akan tetapi situs tersebut menjadi tidak optimal baik dari segi fungsi maupun tampilan.

## Struktur

### External CSS

| Tag | Atribut |
| :-: | - |
| `link` | <table> <tr> <th>Nama</th> <th>Nilai</th> </tr><tr align="center"> <td>href</td><td>*.css</td></tr><tr align="center"> <td>rel</td><td>stylesheet</td></tr><tr align="center"> <td>type</td><td>text/css</td></tr></table> |

### External JS

| Tag | Atribut |
| :-: | - |
| script | <table> <tr> <th>Nama</th> <th>Nilai</th> </tr><tr align="center"> <td>src</td><td>*.js</td></tr></table> |

## Metode
Agar menjadi situs yang utuh, maka perlu untuk menghubungkan antara file HTML, CSS dan JS yang bertujuan untuk saling berkomunikasi satu sama lain.

Ada tiga dan dua metode untuk menghubungkan atau memanggil CSS dan JS ke dalam HTML.

### Cascading Style Sheets

#### Inline
Metode ini menggunakan atribut `style` pada elemen HTML. Berikut contohnya :

```html
<h1 style="color:red; border: 5px solid #000">Ini bukan judul!</h1>
```

#### Internal
Metode ini menggunakan tag `style` di dalam elemen `head`. Berikut contohnya :

```html
<head>
  ...
  <style>
    h1 { color:red }
  </style>
</head>
<body>
  <h1>Ini bukan judul!</h1>
</body>
```

#### External
Metode ini menggunakan tag `link` di dalam elemen `head`. Berikut contohnya :

```html
<head>
  <link href="style.css" rel="stylesheet" type="text/css">
</head>
```

### JavaScript

#### Internal
Metode ini menggunakan tag `script` di dalam elemen `head` atau `body`. Berikut contohnya :

```html
<head>
  ...
  <script src="script.js"></script>
</head>
```

#### External
Metode ini menggunakan tag `script` di dalam elemen `head` atau `body`. Berikut contohnya :

```html
<body>
  <script>
    (function() {
      alert("Halo dunia!")
    })()
  </script>
</body>
```

## File Paths
Ada dua metode ketika ingin memanggil file ke dalam HTML.

### Absolute
Metode ini menggunakan URL lengkap dari sumber file. Sebagai contoh :

```html
<img alt="Mountain" src="https://www.w3schools.com/images/picture.jpg">
```

### Relative
Metode ini memanggil sumber file berdasarkan lokasi halaman yang sedang diakses. Sebagai contoh :

```html
<!-- index.html -->
<img src="images/picture.jpg" alt="Colorfull Background" width="250px" height="auto">
```

```html
<!-- spesial.html -->
<img src="../images/picture.jpg" alt="Colorfull Background" width="250px" height="auto">

<br>

<img src="./../images/picture.jpg" alt="Colorfull Background" width="250px" height="auto">
```