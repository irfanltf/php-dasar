# php-dasar
* [Tipe data dalam PHP](#1-tipe-data)
  + [Tipe data String](#1-tipe-data-string)
  + [Tipe data Integer](#2-tipe-data-inteeger)
  + [Tipe data Float)](#3-tipe-data-float)
  + [Tipe data Boolean](#4-tipe-data-boolean)
  + [Tipe data Null](#5-tipe-data-null)
* [Struktur Kendali](#2-Struktur-Kendali)
  + [Pernyataan if](#1-pernyataan-if)
  + [Pernyataan else](#2-pernyataan-else)
  + [Pernyataan else-if](#3-pernyataan-else-if)
  + [Pernyataan operator ternary](#4-pernyataan-operator-ternary)
  + [Pernyataan switch case](#5-pernyataan-switch-case)
  + [Pernyataan for](#6-pernyataan-for)
  + [Pernyataan while](#7-pernyataan-while)
  + [Pernyataan do while](#8-pernyataan-do-while)
  + [Pernyataan foreach](#9-pernyataan-foreach)
  + [Pernyataan nested loop](#10-pernyataan-nested-loop)
  
  
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


# 2. Struktur Kendali
Struktur kendali adalah bagian dari bahasa pemrograman yang memungkinkan Anda mengontrol alur eksekusi program berdasarkan kondisi atau keputusan tertentu. Ini memungkinkan program Anda untuk membuat keputusan tentang tindakan yang akan diambil berdasarkan berbagai situasi yang mungkin terjadi selama eksekusi. Dalam bahasa pemrograman PHP, ada beberapa jenis struktur kendali utama:

##



## License

[mirfanlutfi](https://github.com/irfanltf)
