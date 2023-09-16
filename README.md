# php-dasar
* [Tipe data dalam PHP](#1-tipe-data-dalam-php)
  + [Tipe data String](#1-tipe-data-string)
  + [Tipe data Integer](#2-tipe-data-integer)
  + [Tipe data Float](#3-tipe-data-float)
  + [Tipe data Boolean](#4-tipe-data-boolean)
  + [Tipe data Null](#5-tipe-data-null)
* [Struktur Kendali](#2-struktur-kendali)
  + [Pernyataan if](#1-if)
  + [Pernyataan else](#2-else)
  + [Pernyataan else-if](#3-else-if)
  + [Pernyataan operator ternary](#4-operator-ternary)
  + [Pernyataan switch case](#5-switch-case)
  + [Pernyataan for](#6-for)
  + [Pernyataan while](#7-while)
  + [Pernyataan do while](#8-do-while)
  + [Pernyataan foreach](#9-foreach)
  + [Pernyataan nested loop](#10-nested-loop)
* [Pengolahan Form](#3-pengolahan-form)
  + [Mengirim dan menerima data dari formulir HTML](#1-mengirim-dan-menerima-data-dari-formulir-html)
  + [Validasi input pengguna](#2-validasi-input-pengguna)
  + [Menggunakan metode GET dan POST](#3-menggunakan-metode-get-dan-post)
    + [Metode GET](#metode-get)
    + [Metode POST](#metode-post)
    
  
  
# 1. Tipe Data dalam PHP

Tipe data dalam pemrograman PHP adalah cara untuk mengklasifikasikan dan mengelompokkan nilai-nilai berdasarkan jenis atau karakteristik tertentu. Pemahaman yang baik tentang tipe data sangat penting karena mereka memengaruhi bagaimana Anda memanipulasi dan memproses data dalam aplikasi PHP Anda. Dalam PHP, ada beberapa tipe data dasar yang umum digunakan.

## 1. Tipe Data String

Tipe data string digunakan untuk merepresentasikan teks atau karakter. String dalam PHP didefinisikan dengan tanda kutip ganda (" ") atau tanda kutip tunggal (' ').

```php
$nama = "Efika";
$alamat = 'Lampung Barat';
```

## 2. Tipe Data Integer

Tipe data integer digunakan untuk merepresentasikan bilangan bulat positif atau negatif.

```php
$nilaiMtk = 90;
$nilaiKimia = -10;
$nilaiFisika = 0;
```

## 3. Tipe Data Float

Tipe data float (atau double) digunakan untuk merepresentasikan bilangan pecahan..

```php
$harga = 12.99;
$nilaiPi = 3.14159265359;
```

## 4. Tipe Data Boolean

Tipe data boolean digunakan untuk merepresentasikan nilai kebenaran (true atau false). Tipe data ini sering digunakan dalam kondisi dan pernyataan kontrol aliran program.

```php
$benar = true;
$salah = false;
```


## 5. Tipe Data NULL

Tipe data null digunakan untuk menunjukkan bahwa suatu variabel tidak memiliki nilai atau tidak terdefinisi.

```php
$nilai = null;
```

## Coba Kode dibawah ini :

PHP

```php
 <?php
    $namaFaisal = "Faisal";
    $nilaiKimiaFaisal = 85;
    $nilaiFisikaFaisal = 78.5;
    $nilaiBiologiFaisal = 92;
    $nilaiMatematikaFaisal = 88;

    $namaHevi = "Hevi";
    $nilaiKimiaHevi = 90.5;
    $nilaiFisikaHevi = 85;
    $nilaiBiologiHevi = 88;
    $nilaiMatematikaHevi = 76;

    $namaChania = "Chania";
    $nilaiKimiaChania = 75;
    $nilaiFisikaChania = 82.5;
    $nilaiBiologiChania = 95;
    $nilaiMatematikaChania = 91;
    ?>
```

HTML

```html
<!DOCTYPE html>
<html>
<head>
    <title>Daftar Nilai</title>
</head>
<body>
    <h1>Daftar Nilai Siswa</h1>

    <table border="1">
        <tr>
            <th>Nama</th>
            <th>Kimia</th>
            <th>Fisika</th>
            <th>Biologi</th>
            <th>Matematika</th>
        </tr>
        <tr>
            <td><?php echo $namaFaisal; ?></td>
            <td><?php echo $nilaiKimiaFaisal; ?></td>
            <td><?php echo $nilaiFisikaFaisal; ?></td>
            <td><?php echo $nilaiBiologiFaisal; ?></td>
            <td><?php echo $nilaiMatematikaFaisal; ?></td>
        </tr>
        <tr>
            <td><?php echo $namaHevi; ?></td>
            <td><?php echo $nilaiKimiaHevi; ?></td>
            <td><?php echo $nilaiFisikaHevi; ?></td>
            <td><?php echo $nilaiBiologiHevi; ?></td>
            <td><?php echo $nilaiMatematikaHevi; ?></td>
        </tr>
        <tr>
            <td><?php echo $namaChania; ?></td>
            <td><?php echo $nilaiKimiaChania; ?></td>
            <td><?php echo $nilaiFisikaChania; ?></td>
            <td><?php echo $nilaiBiologiChania; ?></td>
            <td><?php echo $nilaiMatematikaChania; ?></td>
        </tr>
    </table>
</body>
</html>

```


## Buatlah Tampilan berikut ini (1)

<img width="1296" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/1799596b-739c-41fb-847d-b7a948cc08d1">

  dengan ketentuan :
- Kolom Produk dan Harga, disimpan pada variable
- Kolom	Diskon (10%)	dihitung menggunakan operator dan disimpan menggunakan variable
- Kolom Harga Setelah Diskon dihitung menggunakan operator dan disimpan menggunakan variable



## Revisi Tugas sebelumnya menjadi seperti ini (1)

<img width="1449" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/2e5d461f-e56f-43d4-b153-4b21a90d2d64">

dengan ketentuan :
- Kolom Stok disimpan kedalam variable
- Baris total menghitung jumlah Stok
- Total harga menghitung jumlah harga

## Buatlah Tampilan berikut ini (2)

<img width="590" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/bcc8db76-3e21-4189-88a9-65c1016e8f31">

dengan ketentuan :
- Kolom Bulan, total Penjualan, Biaya Operasional dan Laba Bersih disimpan pada variable
- Kaba bersih diperoleh dari total penjualan - biaya operasional

## Revisi Tugas sebelumnya menjadi seperti ini (2)

<img width="568" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/5dc9e50f-622d-4c0c-8ce8-9e6a5ad74af3">

dengan ketentuan :
- baris total  terdapat kolom yang mehitung total semua bulan
- gunaknan operasi matematika untuk menghitung total yang ada

## Membuat Kaklulator HTML sederhana

![code](https://github.com/irfanltf/php-dasar/assets/48278734/b88d26fe-8891-425a-aa09-ef37608e501b)


## Menggunakan variable di file lain
Scenario
- Buatlah 2 file php dengan nama __variable.php__ dan __index.php__
- pada file __variable.php__ isi dengan variable yang menyimpan nama dan umur
- pada file __index.php__ gunakan fungsi include ke __variable.php__ untuk menggunakan variable yang sudah dibuat di __variable.php__ lalu tuliskan kode seperti berikut ini, disini kita ingin menampilkan umur saat ini, umur 1 tahun kedepan, dan umur setahun yang lalu
  
  ![variable](https://github.com/irfanltf/php-dasar/assets/48278734/41eb8aad-a32f-4f9f-9c5c-0626a4e8562e)


Nilai Kelompok 1 : 7
Nilai Kelompok 2 : 5
Nilai Kelompok 3 : 10
Nilai Kelompok 4 : 
Nilai Kelompok 5 : 10
Nilai Kelompok 6 :


# 2. Struktur Kendali
Struktur kendali adalah bagian dari bahasa pemrograman yang memungkinkan Anda mengontrol alur eksekusi program berdasarkan kondisi atau keputusan tertentu. Ini memungkinkan program Anda untuk membuat keputusan tentang tindakan yang akan diambil berdasarkan berbagai situasi yang mungkin terjadi selama eksekusi. Dalam bahasa pemrograman PHP, ada beberapa jenis struktur kendali utama:

## 1. if
Pernyataan if digunakan untuk menguji suatu kondisi. Jika kondisi tersebut benar (true), maka blok kode di dalamnya akan dieksekusi. Jika kondisi salah (false), blok kode tersebut dilewati. lihatlah kode dibawah ini :

```php
$nilai = 75;
if ($nilai >= 70) {
    echo "Selamat, Anda lulus!";
}
```

## 2. else

Pernyataan else digunakan bersama dengan if untuk memberikan alternatif ketika kondisi dalam if tidak benar.
Ini memungkinkan untuk menjalankan blok kode alternatif.

```php
$nilai = 60;
if ($nilai >= 70) {
    echo "Selamat, Anda lulus!";
} else {
    echo "Maaf, Anda belum lulus.";
}
```

## 3. else if
Pernyataan elseif digunakan untuk menambahkan kondisi tambahan setelah if. Jika kondisi dalam if tidak benar, maka kondisi dalam elseif akan cek. Ini memungkinkan untuk menguji beberapa kondisi secara berurutan.

```php
$nilai = 60;
if ($nilai >= 70) {
    echo "Selamat, Anda lulus!";
} elseif ($nilai >= 60) {
    echo "Anda hampir lulus.";
} else {
    echo "Maaf, Anda belum lulus.";
}
```


## Contoh Kasus (1) Pengkondisian If
identifikasikan menjadi sebuah penjelasan tentang kode dibawah ini :

![1](https://github.com/irfanltf/php-dasar/assets/48278734/f6b6db43-c8c3-44e6-8791-02d576ac8bbf)

## 4. Operator Ternary
(If Else dalam 1 baris)
Operator Ternary (juga dikenal sebagai ternary conditional operator atau conditional expression) adalah operator khusus dalam banyak bahasa pemrograman, termasuk PHP, yang digunakan untuk mengevaluasi ekspresi berdasarkan kondisi tertentu dan mengembalikan satu dari dua nilai berdasarkan kondisi tersebut. Operator ternary biasanya digunakan sebagai alternatif singkat untuk pernyataan if-else. Format umum dari operator ternary adalah:

```php
(condition) ? value_if_true : value_if_false;
```
__condition:__ Kondisi yang akan dievaluasi. Jika kondisi ini benar (true), maka value_if_true akan digunakan; jika kondisi salah (false), maka value_if_false yang akan digunakan.

__value_if_true:__ Nilai yang akan dikembalikan jika kondisi benar.

__value_if_false:__ Nilai yang akan dikembalikan jika kondisi salah.

__Contoh penggunaan :__

```php
$umur = 18;
$status = ($umur >= 18) ? "Dewasa" : "Anak-anak";
echo "Status: " . $status;
```
Pada contoh di atas, operator ternary digunakan untuk mengevaluasi apakah $umur lebih besar atau sama dengan 18. Jika benar, variabel $status akan diisi dengan "Dewasa"; jika salah, variabel $status akan diisi dengan "Anak-anak". Hasil akhirnya adalah "Status: Dewasa" karena nilai $umur adalah 18, yang memenuhi kondisi.

__contoh lain :__

```php
$total_belanja = 120;
$diskon = ($total_belanja > 100) ? ($total_belanja * 0.10) : 0;
echo "Diskon: $" . $diskon;
```
__kalau dalam bentuk if else biasa :__

```php
$total_belanja = 120;
if ($total_belanja > 100) {
    $diskon = $total_belanja * 0.10;
} else {
    $diskon = 0;
}
echo "Diskon: $" . $diskon;
```

## 5. Switch Case
Pernyataan switch digunakan untuk membuat percabangan berdasarkan nilai ekspresi tertentu. Ini memungkinkan Anda untuk menjalankan kode berbeda berdasarkan nilai ekspresi yang sesuai dengan salah satu dari beberapa "kunci" yang didefinisikan. Berikut adalah format umum dari pernyataan switch dalam PHP:
```php

variable ekspresi;

switch (ekspresi) {
    case nilai_1:
        // Blok kode yang akan dieksekusi jika ekspresi sama dengan nilai_1
        break;
    case nilai_2:
        // Blok kode yang akan dieksekusi jika ekspresi sama dengan nilai_2
        break;
    // case lainnya jika diperlukan
    default:
        // Blok kode yang akan dieksekusi jika tidak ada kasus yang cocok
}
```

__contoh kasusnya__

```php
//misalnya terdapat variable $day yang isinya Monday
$day = "Monday";


//variable $day akan dicek dimasukan ke dadlam switch
switch ($day) {
//apakah nilainya Monday? jika iya eksekusi perintah didalamnya
    case "Monday":
        echo "It's Monday!";
//break dgunakan untuk keluar dari kondisi
        break;
//apakah nilainya Tuesday? jika iya eksekusi perintah didalamnya
    case "Tuesday":
        echo "It's Tuesday!";
        break;
//apakah nilainya Wednesday, jika iya eksekusi perintah didalamnya
    case "Wednesday":
        echo "It's Wednesday!";
        break;
//jika tidak ada yang cocok dengan case diatas maka eksekusi bagian default
    default:
        echo "It's another day.";
}
```

## Contoh Kasus (2) Membuat Halaman Login 

__Kode html :__

![halaman login](https://github.com/irfanltf/php-dasar/assets/48278734/f98d8837-975c-437e-b5d9-c353a070f503)

__Kode php :__

![php kondisi](https://github.com/irfanltf/php-dasar/assets/48278734/5dc57133-bddd-4a7f-8d29-2c97373c392e)


## 6. for
Perulangan for adalah salah satu struktur kendali yang digunakan dalam pemrograman untuk mengulangi serangkaian pernyataan dengan jumlah iterasi tertentu. __Perulangan for umumnya digunakan ketika Anda tahu berapa kali perlu menjalankan pernyataan tersebut__.
```php
for (inisialisasi; kondisi; peningkatan) {
    // Blok kode yang akan diulang
}
```


__contohnya :__

```php
<!DOCTYPE html>
<html>

<head>
    <title>Contoh Perulangan For dalam HTML</title>
</head>

<body>
    <h1>Daftar Angka 1 hingga 10</h1>
    <ul>
        <?php
        for ($i = 1; $i <= 10; $i++) {
            echo "<li>Item ke-$i</li>";
        }
        ?>
    </ul>
</body>

</html>
```

## 7. while
Perulangan while  adalah struktur kendali yang digunakan dalam pemrograman untuk mengulangi serangkaian pernyataan selama kondisi tertentu terpenuhi. 
Perulangan while menguji kondisi sebelum menjalankan blok kode

```php
while (kondisi) {
    // Blok kode yang akan diulang
}
```

__contohnya :__

```php
$angka = 1;
while ($angka <= 5) {
    echo "Angka: $angka<br>";
    $angka++;
}
```


## 8. Do While
Perulangan while  adalah struktur kendali yang digunakan dalam pemrograman untuk mengulangi serangkaian pernyataan selama kondisi tertentu terpenuhi. do-while menjalankan blok kode setidaknya satu kali, dan kemudian menguji kondisi setelahnya.

```php
do {
    // Blok kode yang akan diulang
} while (kondisi);
```

blok kode dalam do akan selalu dijalankan sekali, bahkan jika kondisi awalnya salah. Kemudian, kondisi akan diperiksa, dan jika benar (true), perulangan akan dilanjutkan.
__contohnya :__

```php
$angka = 1;
do {
    echo "Angka: $angka<br>";
    $angka++;
} while ($angka <= 5);
```
Dalam contoh di atas, blok kode dalam do akan dijalankan sekali, dan kemudian kondisi akan diperiksa. Karena kondisinya benar, perulangan akan dilanjutkan dan mencetak angka dari 1 hingga 5.

## 9. Foreach
Foreach adalah jenis perulangan khusus dalam pemrograman PHP yang digunakan untuk mengiterasi (mengulang) elemen-elemen dalam sebuah array atau objek. For-each digunakan untuk mengeksekusi pernyataan atau blok kode yang sama pada setiap elemen dalam array atau objek, sehingga Anda tidak perlu menghitung indeks atau jumlah elemen secara manual.

```php
foreach ($array_or_object as $item) {
    // Blok kode yang akan diulang untuk setiap $item
}
```

$array_or_object: Array atau objek yang akan diiterasi.
$item: Variabel yang akan mewakili setiap elemen dalam array atau properti dalam objek.


__contohnya :__
```php
// Contoh penggunaan foreach dengan array
$fruits = array("Apel", "Pisang", "Jeruk", "Mangga");

foreach ($fruits as $fruit) {
    echo $fruit . "<br>";
}
```

## 10. Nested Loop
Nested loop adalah konsep dalam pemrograman di mana satu perulangan (loop) ditempatkan di dalam perulangan lain. Ini berarti Anda memiliki perulangan dalam perulangan, dan setiap iterasi dari perulangan luar akan mengulang seluruh perulangan dalamnya. Nested loop berguna ketika Anda perlu mengakses setiap elemen dalam dua dimensi atau lebih, seperti matriks atau tabel.

__contohnya :__
```php
for ($i = 1; $i <= 3; $i++) {
    for ($j = 1; $j <= 2; $j++) {
        echo "Iterasi luar: $i, Iterasi dalam: $j<br>";
    }
}
```
Penjelasan:

Loop luar ($i) akan dieksekusi tiga kali, dengan nilai $i dari 1 hingga 3.
Di dalam setiap iterasi loop luar, loop dalam ($j) akan dieksekusi dua kali, dengan nilai $j dari 1 hingga 2.
Dalam setiap iterasi loop dalam, pesan yang mencakup nilai $i dan $j akan dicetak.

__hasil output yang terjadi adalah :__
```php
Iterasi luar: 1, Iterasi dalam: 1
Iterasi luar: 1, Iterasi dalam: 2
Iterasi luar: 2, Iterasi dalam: 1
Iterasi luar: 2, Iterasi dalam: 2
Iterasi luar: 3, Iterasi dalam: 1
Iterasi luar: 3, Iterasi dalam: 2
```
## Contoh Kasus (3) Membuat Dropdown nomor
![for2](https://github.com/irfanltf/php-dasar/assets/48278734/1a7a9d93-650a-4d9f-a25d-9438baf7234f)

## Contoh Kasus (4) Membuat Dropdown Pilihan Warna
![foreach](https://github.com/irfanltf/php-dasar/assets/48278734/13b10a4c-6e03-4625-811d-7d12de86ce5c)



# 3. Pengolahan Form
## 1. Mengirim dan menerima data dari formulir HTML
## 2. Validasi input pengguna
## 3. Menggunakan metode GET dan POST
### Metode GET
### Metode POST


## License

[mirfanlutfi](https://github.com/irfanltf)
