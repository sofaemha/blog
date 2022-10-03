---
title: "Pengenalan CSS3"
weight: 1
---

## Pengertian
CSS singkatan dari _Cascading Style Sheets_, merupakan bahasa pemrograman yang menjelaskan bagaimana sebuah elemen ditampilkan pada layar, kertas, atau media lainnya agar terlihat menarik dan indah.

Selain itu bahasa ini dapat mengontrol berbagai halaman situs sekaligus mulai dari pewarnaan, tata letak, _font_ yang digunakan, bahkan animasi. 

## Struktur
CSS sendiri memiliki empat bagian yaitu `selector`, `declaration`, `property` dan `value`.

```css
selector {
  property: value;
}
```

Ketika ingin mendekorasi _heading 1_, maka :

```css
h1 {
  color: #fe2020;
  background-color: #060057;
}
```

Jika dipresentasikan dalam bentuk tabel, maka :

| Selektor | Deklarasi |
| :-: | :-: |
| `h1` | <table> <tr> <th>Properti</th> <th>Nilai</th> </tr><tr align="center"> <td>color</td><td>#fe2020</td></tr><tr align="center"> <td>background-color</td><td>#060057</td></tr></table> |

### Selector
Selektor merupakan bagian yang digunakan untuk memanggil elemen HTML yang ingin didekorasi. Ada tiga selektor yang sering dipakai, yaknik `Simple`, `Combinators` dan `Pseudo`.

#### Simple
Bagian ini digunakan untuk memilih elemen yang akan didekorasi. Secara keseluruhan ada enam metode untuk memilih elemen, yakni dengan `id`, `tag`, `class` dan `universal`.

##### ID
Selektor `id` disebut juga _ID Selector_, memiliki simbol khusus yakni `#` (U+0023). Selektor ini akan memilih elemen secara spesifik berdasarkan nilai identitas yang bersifat unik.

```css
#punyaku { ... } #panjang { ... }
#sekali {...} #bagaikan { ... }
#sosis { ... } #jumbo { ... }
```

##### Tag
Selektor `tag` disbut juga _Type Selector_. Selektor ini akan memilih semua elemen berdasarkan nama tag. Sebagai contoh ketika ingin memilih semua elemen paragraf atau div, maka cukup memanggil nama dari tag tersebut.

```css
p { ... } ul { ... } ol {...}
div { ... } li { ... } span { ... }
```

##### Class
Selektor `class` disbut juga _Class Selector_. Selektor ini akan memilih semua elemen berdasarkan identitas dari elemen tersebut.

```css
.batik { ... } .smk { ... }
.warepack { ... } .ups { ... }
```

##### Universal
Selektor `universal` disebut juga _Universal Selector_, memiliki simbol khusus yakni `*` (U+002A). Selektor ini akan memilih semua elemen pada suatu dokumen baik umum atau spesifik.

```css
* { ... }
*.batik { ... } /* === */ .batik { ... }
*#ganteng /* === */ #ganteng { ... }
```

#### Combinators
Penggabungan merupakan salah satu metode yang menggabungkan dua selektor berdasarkan kategori. Terdapat empat kategori, diantaranya :

##### Descendant
Kategori ini memilih semua elemen turunan dari elemen yang spesifik. Adapun simbol yang digunakan berupa `spasi`.

```css
div p { ... } p a { ... }
a span { ... } span i { ... }
```

##### Child
Kategori ini memilih semua anak elemen dari elemen yang spesifik. Adapun simbol yang digunakan berupa `>` (U+003E).

```css
div > p { ... } p > a { ... }
a > span { ... } span > i { ... }
```

##### Adjacent Sibling
Kategori ini memilih elemen yang berada tepat setelah elemen yang spesifik. Adapun simbol yang digunakan berupa `+` (U+002B).

```css
div + p { ... } p + a { ... }
a + span { ... } span + i { ... }
```

##### General Sibling
Kategori ini memilih semua elemen yang bersaudara dari elemen yang spesifik. Adapun simbol yang digunakan berupa `~` (U+007E).

```css
div ~ p { ... } p ~ a { ... }
a ~ span { ... } span ~ i { ... }
```

### Declaration
Deklarasi merupakan bagian yang digunakan untuk mendeklarasikan style atau dekorasi yang dipisahkan dengan titik koma.

### Property and Value
Properti merupakan pilihan dekorasi yang diinginkan. Sedangkan nilai merupakan nilai dari properti tersebut.