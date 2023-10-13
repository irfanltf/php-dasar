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
* [Array Pada PHP](#4-array-php)
  + [Apa itu Array](#1-apa-itu-array)
  + [Jenis-jenis Array](#2-jenis-jenis-array)
  + [Manipulasi Array](#3-manipulasi-array)
* [Cookie dan Session](#5-cookie-dan-session)
  + [Variabel Super Global dalam PHP](#1-variabel-super-global-dalam-php)
  + [Session](#2-session)
  + [Cookie](#3-cookie)
* [Function](#6-Function)
  + [Apa itu Function](#1-apa-itu-function)
  + [Jenis-Jenis Function](#2-jenis-jenis-function)
    + [Build in Function](#build-in-function)
    + [Custom Function](#custom-function)
    + [Custom Rekursif](#rekursif-function)
    + [Anonim Function](#anonim-function)
    + [Callback Function](#callback-function)
  + [Parameter dalam Function](#3-parameter-dalam-function)
  + [Nilai Kembali (Return)](#4-return)
* [Object Oriented Programming PHP](#7-oop-pada-php)
  + [Class](#1-class)
  + [Object](#2-object)
  + [Properti](#3-properti)
  + [Method](#4-method)
  + [Constructor](#5-constructor)
  + [Inheritence](#6-inheritence)
  + [Overidding](#7-overidding)
  + [Visibility](#8-visibility)
  + [Setter dan Getter](#9-setter-dan-getter)
  + [Static Keyword](#10-static-keyword)
  + [Constant](#11-constant)
  + [Abstract Class](#12-abstract-class)
  + [Interface](#13-interface)
  + [Autoloading](#14-Autoloading)
  + [Namespace](#15-namespace)
* [Berkerja dengan Database](#8-bekerja-dengan-database)
  + [Menghubungkan ke database](#1-menghubungkan-ke-database)
  + [Create data ke database](#2-create-data-ke-database)
  + [Read data pada database](#3-read-data-pada-database)
  + [Update data pada database](#4-update-data-pada-database)
  + [Delete data pada database](#5-update-data-pada-database)
    
    
  
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
Pengolahan form adalah bagian penting dari pengembangan web yang memungkinkan pengguna berinteraksi dengan halaman web Anda. Dalam PHP, Anda dapat dengan mudah mengirim dan menerima data dari formulir HTML.
## 1. Mengirim dan menerima data dari formulir HTML
Untuk mengirim data dari formulir HTML ke PHP, Anda perlu menentukan action dan method dalam elemen <form>. action adalah URL atau arah data ingin dikirimkan ke mana, sedangkan method dapat berupa GET atau POST.
__mengirim__
```php
<form action="proses.php" method="post">
    <input type="text" name="nama">
    <button type="submit">Kirim</button>
</form>
```
__menerima__
Di dalam skrip PHP yang ditentukan dalam action, Anda dapat mengakses data formulir menggunakan $_POST (untuk metode POST) atau $_GET (untuk metode GET). Contoh PHP untuk mengambil data nama yang dikirim dengan metode POST:
```php
$nama = $_POST["nama"];
```

## 2. Validasi input pengguna
Validasi input pengguna adalah langkah penting untuk memastikan bahwa data yang dikirim oleh pengguna sesuai dengan aturan atau format yang diharapkan.

Contoh validasi sederhana untuk memeriksa apakah sebuah input tidak kosong:
```php
if (isset($_POST["nama"]) && !empty($_POST["nama"])) {
    // Data nama sudah diisi
    $nama = $_POST["nama"];
} else {
    // Data nama kosong, berikan pesan kesalahan
    $error = "Nama harus diisi.";
}
```

## 3. Menggunakan metode GET dan POST
### Metode GET
Metode GET: Data formulir dikirim sebagai query string dalam URL. Metode ini cocok untuk mengambil data yang tidak sensitif seperti pencarian atau filter. Namun, karena data ditampilkan dalam URL, ini bisa tidak aman jika digunakan untuk data sensitif.
Contoh URL dengan metode GET: https://contoh.com/cari.php?kata=kucing

## Contoh Kasus (1) Mengirim dan Menerima dengan Metode GET

__(Mengirim)__ buat file dengan nama _kirim_get.php_
![get kirim](https://github.com/irfanltf/php-dasar/assets/48278734/3677adc4-d216-4c95-8560-a9ce6bbe0ebd)

__(Menerima)__ buat file dengan nama _terima_get.php_
![get_terima](https://github.com/irfanltf/php-dasar/assets/48278734/295b5c63-690b-4acf-a35a-2097ccd7b7b9)


### Metode POST
Metode POST: Data formulir dikirim secara tersembunyi dalam badan permintaan HTTP. Metode ini lebih aman untuk data sensitif seperti kata sandi. Dalam PHP, Anda mengakses data dengan $_POST.

## Contoh Kasus (2) Mengirim dan Menerima dengan Metode POST
__(Mengirim)__ buat file dengan nama _kirim_post.php_
![post_kirim](https://github.com/irfanltf/php-dasar/assets/48278734/42800f39-b14f-484f-82e7-38aab3a9ff35)

__(Menerima)__ buat file dengan nama _terima_post.php_
![post_terima](https://github.com/irfanltf/php-dasar/assets/48278734/b5bb72c0-cf4f-47a2-9fa3-2c4894b92033)

# 4. Array php
## 1. Apa itu Array

__Apa itu Array?__
Array adalah _struktur data_ yang digunakan untuk menyimpan kumpulan nilai atau elemen dalam satu variabel. Ini memungkinkan kita untuk _mengelola data dalam kelompok_, seperti daftar item atau koleksi data terkait. Array memiliki indeks yang memungkinkan kita mengakses setiap elemen dengan cara yang terstruktur.

__Apa Fungsinya?__
Array sangat berguna dalam pemrograman karena memungkinkan kita untuk:

__Mengorganisasi Data:__ Array membantu dalam pengorganisiran data yang serupa. Contohnya, kita dapat menggunakan array untuk menyimpan daftar nama atau angka.

__Efisiensi:__ Dengan menggunakan array, kita dapat mengakses dan memanipulasi data secara efisien. Kita dapat mengakses elemen array dengan cepat menggunakan indeksnya.

__Iterasi:__ Array memungkinkan kita untuk mengulangi (loop) melalui elemen-elemen dalam struktur data dengan mudah, misalnya untuk mencetak daftar, menghitung nilai rata-rata, dll.

__Pencarian dan Pengurutan:__ Array memberikan fasilitas untuk mencari dan mengurutkan data, yang penting dalam pemrosesan data.

__Mengelola Data Terkait:__ Ketika kita memiliki data terkait, seperti data siswa dengan nama, usia, dan nilai, array dapat digunakan untuk mengelola data ini dalam satu struktur.

__cara membuat array ada 2 cara :__
```php
// 1. menggunakan simbol berikut : []
$array = [1,4,6,7,9];

//2. menggunakan simbol keyword array()
$array = array(1,4,6,7,9);
```

## 2. Jenis-jenis Array

- __Array Numerik:__ Ini adalah jenis array yang memiliki indeks numerik berurutan dan dimulai dari 0.

  __contoh :__
  
  ```php
  $nilai = array(90, 85, 78, 92, 88);
  ```

  __cara mengakses nilai dalam array numberik :__

  ```php
  echo $nilai[2];

  // tulis nama variable, lalu didalam kurung siku isi dengan index ke berapa nilai yang ingin diambil
  // hasil outputnya adalah 78
  ```
  
- __Array Asosiatif:__ Ini adalah jenis array yang menggunakan kunci (key) atau nama sebagai indeks untuk setiap elemen, Array Asosiatif memiliki key dan value.

  __contoh :__

```php
$siswa = array("nama" => "Nisa Aulia", "usia" => 19, "kelas" => "MI B");
```

  __cara mengakses nilai dalam array asosiatif :__

  ```php
  echo $siswa["nama"];

  // tulis nama variable, lalu didalam kurung siku isi key untuk mengambil value yang diinginkan
  // hasil outputnya adalah Nisa Aulia
  ```
  
- __Array Multidimensi:__ Ini adalah array yang berisi array lain. Ini dapat berupa array numerik dalam array numerik, array asosiatif dalam array asosiatif, atau campuran dari keduanya.

  __contoh :__
  
  ```php
  $matriks = array(
    array(1, 2, 3),
    array(4, 5, 6),
    array(7, 8, 9)
  );
  ```


  __cara mengakses nilai dalam array asosiatif :__

  ```php
  echo $matriks[1][2];

  // tulis nama variable, lalu didalam kurung siku isi dengan index array paling luar, lalu index array selanjutnnya
  // hasil outputnya adalah 5
  ```


  ## Contoh Kasus (1) bagaimana mengakses data-data dibawah ini:'

  
1. jika saya ingin mengakses __umurnya riski hidayat__ bagaimana caranya?
2. jika saya ingin mengakses __nilai pemweb-nya alya__ bagaimana caranya?
3. jika saya ingin mengakses __nilai rbjk-nya fikri__ bagaimana caranya?
4. jika saya ingin mengakses __nama iratih__ bagaimana caranya?
5. jika saya ingin mengakses __usia dari salzabila__ bagaimana caranya?
   
![array1](https://github.com/irfanltf/php-dasar/assets/48278734/e70ef484-ddf8-4db6-a657-9a65de143df7)



  ## Contoh Kasus (2) menampilkan semua dalam table pada html:
__bisa lakukan seperti ini :__
![array2](https://github.com/irfanltf/php-dasar/assets/48278734/d3ac652d-8f1c-4725-aefe-eadda37baa06)

__atau seperti ini :__
![array3](https://github.com/irfanltf/php-dasar/assets/48278734/c1789b1a-ca4b-464f-95c4-73eac898a321)




## 3. Manipulasi Array

count(): Menghitung jumlah elemen dalam array.
```php
$buah = array("Apel", "Jeruk", "Mangga");
echo count($buah); // Output: 3
```

array_push(): Menambahkan elemen ke akhir array.
```php
$buah = array("Apel", "Jeruk");
array_push($buah, "Mangga");
// $buah sekarang menjadi: array("Apel", "Jeruk", "Mangga")
```

array_pop(): Menghapus elemen terakhir dari array.
```php
$buah = array("Apel", "Jeruk", "Mangga");
array_pop($buah);
// $buah sekarang menjadi: array("Apel", "Jeruk")
```

array_shift(): Menghapus elemen pertama dari array.
```php
$buah = array("Apel", "Jeruk", "Mangga");
array_shift($buah);
// $buah sekarang menjadi: array("Jeruk", "Mangga")
```

array_unshift(): Menambahkan elemen ke awal array.
```php
$buah = array("Jeruk", "Mangga");
array_unshift($buah, "Apel");
// $buah sekarang menjadi: array("Apel", "Jeruk", "Mangga")
```

array_merge(): Menggabungkan dua atau lebih array.
```php
$buah1 = array("Apel", "Jeruk");
$buah2 = array("Mangga", "Pisang");
$buah = array_merge($buah1, $buah2);
// $buah sekarang menjadi: array("Apel", "Jeruk", "Mangga", "Pisang")
```

array_slice(): Memotong array menjadi bagian tertentu.
```php
$buah = array("Apel", "Jeruk", "Mangga", "Pisang");
$potongan = array_slice($buah, 1, 2);
// $potongan menjadi: array("Jeruk", "Mangga")
```

array_search(): Mencari nilai dalam array dan mengembalikan indeksnya.
```php
$buah = array("Apel", "Jeruk", "Mangga");
$indeks = array_search("Jeruk", $buah); // $indeks menjadi 1
```

array_key_exists(): Memeriksa apakah indeks tertentu ada dalam array asosiatif.
```php
$siswa = array("nama" => "John", "usia" => 20);
$ada = array_key_exists("usia", $siswa); // $ada menjadi true
```

sort(): Mengurutkan array numerik secara ascending.
```php
$angka = array(5, 3, 1, 4, 2);
sort($angka); // $angka menjadi: array(1, 2, 3, 4, 5)
```


rsort(): Mengurutkan array numerik secara descending.
```php
$angka = array(5, 3, 1, 4, 2);
rsort($angka); // $angka menjadi: array(5, 4, 3, 2, 1)
```

## Studi Kasus (1) 

terdapat sebuah array dibawah ini :
```php
// Inisialisasi array data produk
$produk = [
    ["id" => 1, "nama" => "Laptop", "harga" => 10000000],
    ["id" => 2, "nama" => "Smartphone", "harga" => 5000000],
    ["id" => 3, "nama" => "Tablet", "harga" => 3000000],
    ["id" => 4, "nama" => "Mouse", "harga" => 50000],
    ["id" => 5, "nama" => "Keyboard", "harga" => 100000],
];
```

array teersebut akan ditampilkan dalam bentuk html seperti gambar berikut :

![array4](https://github.com/irfanltf/php-dasar/assets/48278734/09bad454-27fc-4065-9412-51035adb09c3)

__scenario :__

1. Jumlah Produk diperoleh dari total data yang terdapat pada array
2. Tambahkan data pada array, yaitu data headset dengan id 6 dan harga 200000
3. Hapus data dengan ID 3
4. Urutkan dari harga termurah
5. Semua data ditampilkan pada bagian daftar produk mahal diatas satu juta
6. filter data dan tampilkan pada bagian produk
7. Sehingga harusnya datanya tampil seperti diatas


Kelompok 3: 50
Kelompok 7 : 50
Kelompok 5 : 70
Kelompok 2 : 50;
Kelompok 1 :
Kelompok 4 :
Kelompok 6 :


# 6. Cookie dan Session
## 1. Variabel Super Global dalam PHP
Variabel super global adalah variabel yang dapat diakses dari mana saja di dalam skrip PHP tanpa harus menggabungkan variabel dari cakupan lain. Beberapa variabel super global yang umum digunakan dalam PHP adalah:

$_GET: Digunakan untuk mengambil data dari URL melalui metode GET. Data ini dapat diperoleh dengan menambahkan query string ke URL.

$_POST: Digunakan untuk mengambil data yang dikirimkan ke server melalui metode POST. Biasanya digunakan untuk mengirim data melalui formulir.

$_REQUEST: Menggabungkan data dari $_GET dan $_POST. Namun, penggunaan $_REQUEST sebaiknya dihindari karena dapat menimbulkan masalah keamanan.

$_SESSION: Digunakan untuk mengelola data sesi pada server. Data dalam $_SESSION dapat diakses selama sesi pengguna berlangsung.

$_COOKIE: Digunakan untuk mengambil dan mengelola data cookie yang disimpan di sisi klien. Data ini dapat digunakan untuk mengenali pengguna ketika mereka kembali ke situs web.

$_SERVER: Berisi informasi tentang server dan lingkungan eksekusi PHP. Ini mencakup informasi seperti alamat IP pengguna, alamat URL, dan banyak lagi.

$_ENV: Berisi variabel lingkungan yang dapat digunakan untuk mengambil informasi dari sistem operasi atau server.

$_GLOBALS: Digunakan untuk mengakses variabel global dari cakupan global. Variabel dalam $_GLOBALS dapat diakses dan diubah dari mana saja dalam skrip.

## 2. Session
Session adalah cara untuk menyimpan data di server yang terkait dengan sesi pengguna tertentu. Data sesi dapat diakses dan digunakan di berbagai halaman web selama sesi pengguna berlangsung. 

Cara kerja session:

- Ketika sesi dimulai dengan session_start(), server akan memberikan ID sesi unik kepada pengguna.
- Data sesi disimpan di server dengan menggunakan ID sesi sebagai kunci.
- Setiap kali pengguna mengakses halaman web, server akan menggunakan ID sesi ini untuk mengambil data sesi yang sesuai.

__bagaimana cara menjalankan session pada php?__
1. Memulai Sesi: Untuk menggunakan session, Anda harus memulai sesi dengan session_start(). Ini biasanya ditempatkan di bagian atas halaman PHP sebelum output apa pun ke browser pengguna.
   ```php
   session_start();
   ```
2. Menyimpan Data dalam Sesi: Anda dapat menyimpan data dalam sesi dengan mengakses array asosiatif $_SESSION. Data ini dapat berupa variabel, array, atau objek.
   ```php
   $_SESSION['user_id'] = 9080980;
   $_SESSION['user_name'] = "Abdul Halim";
   ```
3. Mengambil Data dari Sesi: Data yang disimpan dalam sesi dapat diambil kembali dengan cara yang sama seperti Anda mengakses elemen dalam array asosiatif.
   ```php
   $user_id = $_SESSION['user_id'];
   $user_name = $_SESSION['user_name'];
   ```

4. Menghapus Data dari Sesi: Anda dapat menghapus data dari sesi dengan menggunakan perintah unset() atau dengan menghapus elemen dari array $_SESSION.
    ```php
    unset($_SESSION['user_name']);
    ```
5. Mengakhiri Sesi: Anda dapat mengakhiri sesi dengan session_destroy(). Ini akan menghapus semua data sesi yang ada. Setelah ini, pengguna perlu memulai sesi baru jika ingin mengakses data sesi.
   ```php
   session_destroy();
   ```
## Contoh Kasus (1) menambahkan session pada saat login

__buat halaman login.php__

![login](https://github.com/irfanltf/php-dasar/assets/48278734/807de84b-b341-46bf-a006-62370f80e776)


__buat halaman beranda.php__

![beranda](https://github.com/irfanltf/php-dasar/assets/48278734/3379e3d2-1406-427e-91f6-332539f5c441)

__buat halaman logout.php__
![logout](https://github.com/irfanltf/php-dasar/assets/48278734/10328dd2-b251-4dc7-9fc2-a85c46db8c2a)






   

## 3. Cookie
Cookies adalah metode lain untuk menyimpan data pada sisi klien. Cookies adalah informasi kecil yang dikirim oleh server web dan disimpan di komputer pengguna. Mereka digunakan untuk mengidentifikasi pengguna, menyimpan preferensi, dan melacak aktivitas pengguna.

Dalam PHP, Anda dapat menggunakan variabel super global $_COOKIE untuk mengakses data dari cookie yang diterima dari klien. Selain itu, Anda dapat menggunakan fungsi-fungsi PHP untuk mengatur dan mengirim cookie ke klien.

```php
setcookie("user_name", "Irfanltf", time() + 3600, "/");
```
Penjelasan:

- setcookie() digunakan untuk mengatur cookie. Dalam contoh di atas, kita mengatur cookie dengan nama "user_name" dan nilainya "Irfanltf".
- time() + 3600 mengatur waktu kadaluarsa cookie dalam detik dari saat ini. Dalam contoh ini, cookie akan kadaluarsa dalam 1 jam.
- "/" adalah jalur atau direktori tempat cookie dapat digunakan. Dalam contoh ini, cookie dapat digunakan di seluruh situs web.

```php
if (isset($_COOKIE['user_name'])) {
    $user_name = $_COOKIE['user_name'];
    echo "Halo, $user_name!";
} else {
    echo "Cookie 'user_name' tidak ditemukan.";
}
```
Penjelasan :
Kode di atas memeriksa apakah cookie "user_name" ada dalam $_COOKIE.
Jika cookie ditemukan, nilainya akan diambil dan digunakan. Jika tidak, pesan kesalahan akan ditampilkan.

__menghapus cookie__
```php
setcookie("user_name", "", time() - 3600, "/");
```

Penjelasan:

Untuk menghapus cookie, Anda dapat mengatur waktu kadaluarsa cookie ke masa lalu (dalam contoh di atas, waktu -3600).

__Keamanan Cookies:__

- Hindari menyimpan data sensitif seperti kata sandi dalam cookies.
- Hindari menyimpan data besar atau terlalu banyak dalam cookies karena ini dapat mempengaruhi kinerja situs.
- Selalu validasi data yang Anda terima dari cookies sebelum menggunakannya, karena pengguna dapat memanipulasi cookies.
- Gunakan HTTPS untuk mengamankan data saat mengirimkan dan menerima cookies.

Cookies adalah cara yang umum digunakan untuk mengidentifikasi pengguna dan menyimpan preferensi di situs web. Mereka berguna untuk mengingatkan pengguna saat mereka kembali ke situs Anda. Namun, pastikan untuk menggunakan mereka dengan bijak dan memerhatikan keamanan.


## Contoh Kasus (2) Menambahkan Cookie pada file sebelumnya

__tambahkan cookie pada saat validasi pada file login.php__
```php
if (isset($_POST['login'])) {
    $username = $_POST['username'];
    $password = $_POST['password'];

    // Contoh validasi sederhana, seharusnya dilakukan validasi yang lebih aman
    if ($username === 'user123' && $password === 'password123') {
        // Simpan ID pengguna ke dalam sesi
        $_SESSION['user_id'] = 123;
        header('Location: beranda.php');
        exit();
    } else {
        $pesan_error = 'Username atau password salah';
    }
}
```

__gunakan cookie pada file beranda.php__
```php
<?php
session_start();

// Jika pengguna belum login, alihkan ke halaman login
if (!isset($_SESSION['user_id'])) {
    header('Location: login.php');
    exit();
}

// Ambil ID pengguna dari sesi
$user_id = $_SESSION['user_id'];
?>
```


# 6. Function
Fungsi (function) adalah bagian penting dalam bahasa pemrograman PHP. Mereka memungkinkan Anda untuk mengelompokkan kode yang dapat digunakan kembali ke dalam blok logis dan memberikan nama pada blok tersebut. PHP memiliki berbagai jenis fungsi yang dapat Anda gunakan untuk melakukan berbagai tugas. Berikut adalah beberapa materi tentang fungsi PHP:
## 1. Apa itu Function
Fungsi adalah blok kode yang dapat digunakan kembali dan memberikan nama pada blok tersebut. Mereka digunakan untuk mengorganisasi kode Anda, membuat kode lebih mudah dibaca, dan menghindari pengulangan.
## 2. Jenis-Jenis Function
### Build in Function
Fungsi built-in (atau fungsi bawaan) dalam PHP adalah fungsi yang sudah disediakan oleh PHP itu sendiri dan dapat langsung digunakan tanpa perlu mendefinisikan ulang. Fungsi ini mencakup berbagai fungsi yang melakukan tugas-tugas umum seperti manipulasi string, pengolahan array, operasi matematika, input/output, dan banyak lagi.

Berikut beberapa contoh fungsi built-in dalam PHP beserta penjelasan singkat:
strlen(): Fungsi ini digunakan untuk menghitung panjang (jumlah karakter) dari sebuah string.
```php
$teks = "Hello, World!";
echo strlen($teks); // Output: 13
```

strtolower() dan strtoupper(): Fungsi ini mengubah huruf dalam sebuah string menjadi huruf kecil atau huruf besar.
```php
$teks = "Hello, World!";
echo strtolower($teks); // Output: hello, world!
echo strtoupper($teks); // Output: HELLO, WORLD!
```

date(): Fungsi ini digunakan untuk mengambil tanggal dan waktu saat ini atau dapat memformat tanggal sesuai dengan kebutuhan.
```php
echo date("Y-m-d"); // Output: Tanggal saat ini dalam format "YYYY-MM-DD"
echo date("H:i:s"); // Output: Waktu saat ini dalam format "HH:MM:SS"
```
dan masih banyak yang lainnya....



### Custom Function
Anda dapat membuat fungsi kustom Anda sendiri untuk melakukan tugas tertentu. Fungsi kustom didefinisikan dengan kata kunci function.
```php
function namaFungsi($parameter1, $parameter2, ...) {
    // Kode yang akan dieksekusi ketika fungsi dipanggil
    // Anda dapat melakukan operasi atau mengembalikan nilai di sini
    return $hasil;
}

```

__contohnya__
```php
function tambah($angka1, $angka2) {
    $hasil = $angka1 + $angka2;
    return $hasil;
}

$hasilTambah = tambah(5, 3);
echo "Hasil penjumlahan: " . $hasilTambah; // Output: Hasil penjumlahan: 8
```

## Contoh Kasus (1) Membuat function konversi ke mata uang rupiah

__buat fungsinya dahulu pada file fungsi.php__
![fungsi](https://github.com/irfanltf/php-dasar/assets/48278734/99416867-07c8-4ffd-bd16-3e189a336f63)

__panggil fungsinya, tapi jangna lupa di include dulu filenya__
![penjualan](https://github.com/irfanltf/php-dasar/assets/48278734/1b64a2ee-a859-4653-9e6f-41e084833a52)




### Rekursif Function
Fungsi yang memanggil dirinya sendiri. Ini sering digunakan untuk mengatasi permasalahan yang dapat dipecahkan secara rekursif, seperti perhitungan faktorial atau pencarian dalam struktur data seperti pohon.
### Anonim Function
Fungsi yang tidak memiliki nama dan biasanya digunakan sebagai argumen untuk fungsi lain atau disimpan dalam variabel.
### Callback Function
ungsi yang digunakan sebagai argumen untuk fungsi lain dan dipanggil saat peristiwa tertentu terjadi.
## 3. Parameter dalam Function
Fungsi dapat menerima parameter sebagai input. Parameter adalah nilai yang diberikan kepada fungsi saat dipanggil. Anda dapat menggunakan parameter untuk membuat fungsi lebih fleksibel.
## 4. Return
Fungsi dapat mengembalikan nilai menggunakan pernyataan return. Nilai ini dapat digunakan di dalam program Anda.

# 7 OOP Pada php
Materi PHP tentang Object-Oriented Programming (OOP) adalah cara untuk mengorganisasi dan mengelola kode PHP Anda dengan menggunakan konsep objek dan kelas. OOP memungkinkan Anda untuk membuat kode yang lebih terstruktur, mudah dipahami, dan mudah dipelihara.
## 1 Class
<img width="973" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/8c34a695-a7ff-4fec-9cf4-36e9238bd256">

___`sumber ilustrasi: https://lovelyristin.com/cara-membuat-class-dan-objek-pada-python`___

Kelas adalah blueprint atau cetakan yang digunakan untuk membuat objek. Ini adalah struktur utama dalam pemrograman berorientasi objek yang mendefinisikan karakteristik (properti) dan perilaku (method) yang dimiliki oleh objek.
Contoh: Jika kita mempertimbangkan konsep mobil, kelas akan berisi informasi tentang bagaimana mobil itu seharusnya, seperti tipe, roda, kecepatan dan cara mengendarainya.

![class mobil](https://github.com/irfanltf/php-dasar/assets/48278734/f92dd151-7545-4b63-81d5-665b6c3ff137)


## 2 Object

<img width="887" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/48122d46-f15c-49dd-935b-b249c6d728ce">


<img width="915" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/e7b186ff-6d07-4fcb-8ad5-3c609033fa95">

___`sumber ilustrasi: https://lovelyristin.com/cara-membuat-class-dan-objek-pada-python`___

Objek adalah instance konkret dari sebuah kelas. Ini adalah hasil nyata dari blueprint atau cetakan yang telah dibuat. Objek memiliki karakteristik (properti) dan perilaku (method) sesuai dengan yang telah ditentukan oleh kelas.
Contoh: Jika kita memiliki kelas "Mobil", maka mobil spesifik yang Anda miliki di dunia nyata adalah objek. Misalnya, mobil dengan tipe "CUV" dan warna "Merah" adalah objek yang diciptakan berdasarkan kelas "Mobil".

![object mobil](https://github.com/irfanltf/php-dasar/assets/48278734/5e5ccec1-4a3b-400e-b707-fbe7c11e8996)



## 3 Properti

<img width="896" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/7e0de879-e506-47d7-ae61-83f93f29924e">

___`sumber ilustrasi: https://lovelyristin.com/cara-membuat-class-dan-objek-pada-python`___

Properti adalah variabel yang digunakan untuk menyimpan data dalam objek. Properti mendefinisikan karakteristik objek dan dapat berupa angka, teks, atau tipe data lainnya.
Contoh: Dalam kelas "Mobil," properti-properti mungkin mencakup merek, warna, nomor plat, tahun pembuatan, dan sebagainya.

![properti](https://github.com/irfanltf/php-dasar/assets/48278734/43be07fb-bb9d-4ff3-8f3d-59f03d761120)


## 4 Method

<img width="896" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/d32e650e-d188-482b-a9d4-7f508cd174d6">

___`sumber ilustrasi: https://lovelyristin.com/cara-membuat-class-dan-objek-pada-python`___

Method adalah fungsi atau tindakan (prilaku) yang dapat dilakukan oleh objek. Method mendefinisikan perilaku objek dan memungkinkan objek untuk berinteraksi dengan lingkungannya atau objek lainnya.
Contoh: Dalam kelas "Mobil," method-method mungkin mencakup "Maju" "Berhenti," "Ganti Oli," dan sebagainya.

![method](https://github.com/irfanltf/php-dasar/assets/48278734/723b87e9-add6-4947-8975-0038907755ea)

![object](https://github.com/irfanltf/php-dasar/assets/48278734/4549eb1d-d4cc-4b47-bd2d-46a68ee982b1)


## Mari berfikir!!!!
1. Jika contoh kasusnya Sepedah Kira kira apa saja properti dan methodnya
2. jika contoh kasusnya Sepatu kira-kira apa saja properti dan methodnya
3. jika contoh kasusnya Buku kira-kira apa saja properti dan methodnya
4. jika conoth kasusnya Rumah kira-kira apa saja properti dan methodnya
5. jika contoh kasusnya Manusia kira-kira apa saja properti dan methodnya
6. jika contoh kasusnya Film kira-kira apa saja properti dan methodnya
7. jika contoh kasusnya Barang kira-kira apa saja ya properti dan methodnya
8. jika contoh kasusnya Mahasiswa kira-kira apa saja ya properti dan methodnya
9. dan yang lainya, mari kita anlisis agar lebih paham tentang class, object, properti dan method


## 5 Constructor


Constructor adalah method atau function yang otomatis akan dijalankan saat class diinstansiasi (dibuat sebuah object), pada bagian constructor kita dapat melakukan apapun yang bisa dilakukan dalam method / function kecuali mengembalikan nilai / return value. Dalam PHP, constructor didefinisikan dengan nama khusus, yaitu __construct.

![construct](https://github.com/irfanltf/php-dasar/assets/48278734/14b59e64-e517-4f9f-9fd3-5455a8f43b7e)



Saat Anda mendefinisikan lebih dari satu constructor dalam sebuah kelas di PHP, yang terakhir didefinisikan akan menggantikan yang sebelumnya. Artinya, PHP tidak mendukung overload constructor seperti beberapa bahasa pemrograman lainnya yang memungkinkan Anda memiliki beberapa constructor dengan jumlah dan jenis parameter yang berbeda.

![constructs](https://github.com/irfanltf/php-dasar/assets/48278734/ab9d8ad7-35d7-429d-9c40-23a94ba00c12)

Jika Anda ingin memberikan fleksibilitas dalam penginisialisasian objek dengan jumlah parameter yang berbeda, Anda dapat menggunakan parameter default dalam constructor tunggal dan kemudian menguji kondisi di dalam constructor untuk menentukan tindakan yang harus diambil berdasarkan parameter yang diterima. Ini adalah pendekatan umum dalam PHP ketika Anda ingin mengatasi situasi seperti itu.

![constructs](https://github.com/irfanltf/php-dasar/assets/48278734/9a9fcfad-6437-46c7-b80d-9c4fdebe52dd)

### Contoh Mengakses method ddan properti pada class mobil pada class pengendara

![mengakses pada class lain](https://github.com/irfanltf/php-dasar/assets/48278734/04826c56-ed41-4bfc-88b9-64122bf71479)

### Contoh jika class diakses pada file yang berbeda, gunakan function `require_once`
![mengakses pada class lain2](https://github.com/irfanltf/php-dasar/assets/48278734/9e42873e-92d9-4b11-a982-c8b573890479)

## 6 Inheritence
Inheritance (Pewarisan) adalah salah satu konsep penting dalam pemrograman berorientasi objek (OOP) yang memungkinkan kelas (class) baru untuk mewarisi sifat dan perilaku (properti dan method) dari kelas yang sudah ada (kelas induk atau superclass). Konsep ini memungkinkan Anda untuk membangun hierarki kelas di mana kelas anak (subclass atau derived class) dapat mewarisi atribut dan metode dari kelas induknya.

jika mengacu pada kasus sebelumnya adalah seperti berikut ini :

![inheriten](https://github.com/irfanltf/php-dasar/assets/48278734/e3731071-f525-4822-bb88-c2c105e382e8)

![inheriten2](https://github.com/irfanltf/php-dasar/assets/48278734/f42e402d-be9c-4b61-995b-d58b7a3bd259)


## 7 Overidding

Overriding adalah salah satu konsep penting dalam pemrograman berorientasi objek (OOP) yang memungkinkan kelas anak (subclass) untuk mengganti (override) implementasi dari sebuah method yang sudah ada di kelas induk (superclass). Dengan kata lain, dalam overriding, kelas anak menyediakan implementasi ulang untuk method yang sudah didefinisikan di kelas induk.

jika mengacu pada kasus sebelumnya adalah seperti berikut ini :

![inheriten](https://github.com/irfanltf/php-dasar/assets/48278734/912f8070-0ea6-4c94-93fe-66c0a6b4d6ee)

![overriding2](https://github.com/irfanltf/php-dasar/assets/48278734/71cfeaa0-e5a9-4e48-a213-652b82727d1c)


## 8 Visibility

Visibility (atau access modifiers) adalah salah satu konsep penting dalam pemrograman berorientasi objek (OOP) yang mengatur aksesibilitas (tingkat visibilitas) terhadap properti dan method dalam suatu kelas. Terdapat tiga tingkat visibilitas utama dalam PHP:

Public: Properti atau method yang didefinisikan sebagai public dapat diakses dari mana saja, baik dari dalam kelas itu sendiri, dari kelas turunan (subclass), maupun dari luar kelas.



Protected: Properti atau method yang didefinisikan sebagai protected hanya dapat diakses dari dalam kelas itu sendiri dan dari kelas turunan (subclass) yang meng-extend kelas tersebut. Properti atau method protected tidak dapat diakses dari luar kelas.

Private: Properti atau method yang didefinisikan sebagai private hanya dapat diakses dari dalam kelas itu sendiri. Properti atau method private tidak dapat diakses dari kelas turunan atau dari luar kelas.

contohnya sebagai berikut :

![visibility](https://github.com/irfanltf/php-dasar/assets/48278734/0c762337-c28b-4365-9279-6e8437de1006)

Dalam contoh ini, kita telah menambahkan tingkat visibilitas yang berbeda pada properti dan method di kelas Mobil dan Pengendara. Properti tipe dideklarasikan sebagai public, properti roda dideklarasikan sebagai protected, dan properti kecepatan dideklarasikan sebagai private. Begitu pula dengan method klakson(), infoRoda(), dan infoKecepatan().

Kemudian, dalam kelas Pengendara, kita mengakses properti dan method dari kelas Mobil yang memiliki tingkat visibilitas protected dan private dengan menggunakan objek $this dalam method infoPengendara()

## 9 Setter dan Getter

Setter dan getter adalah metode khusus yang digunakan dalam pemrograman berorientasi objek (OOP) untuk mengakses dan mengubah properti (variabel) privat (private property) dalam suatu kelas. Metode ini digunakan untuk menerapkan prinsip enkapsulasi, di mana properti yang bersifat privat tidak dapat diakses secara langsung dari luar kelas. Dengan menggunakan setter dan getter, Anda dapat mengontrol bagaimana akses dan perubahan properti tersebut terjadi.

Setter: Setter adalah metode yang digunakan untuk mengubah (set) nilai properti privat dalam kelas. Setter biasanya memiliki parameter yang mewakili nilai baru yang ingin diatur pada properti.

Getter: Getter adalah metode yang digunakan untuk mengambil (get) nilai properti privat dalam kelas. Getter biasanya tidak memiliki parameter dan mengembalikan nilai properti.

Contohnya :

![setterhgetter](https://github.com/irfanltf/php-dasar/assets/48278734/17a19bab-b830-40f4-b634-50b7b30de7f5)

Keuntungan menggunakan setter dan getter meliputi:

Enkapsulasi: Properti privat dapat disembunyikan dari akses langsung dari luar kelas, sehingga menghindari perubahan yang tidak sah.

Validasi: Anda dapat menerapkan validasi dalam setter untuk memastikan bahwa nilai yang diatur pada properti sesuai dengan aturan tertentu sebelum disimpan.

Fleksibilitas: Jika Anda perlu mengubah perilaku setter atau getter di masa depan, Anda dapat melakukannya tanpa mengubah cara penggunaan properti dalam kode yang sudah ada.

Penggantian Properti: Jika Anda ingin mengubah cara properti disimpan atau diambil, Anda hanya perlu mengubah setter atau getter, bukan seluruh kode yang menggunakannya.

Penggunaan setter dan getter merupakan praktik baik dalam OOP untuk memastikan pengelolaan data yang aman dan terstruktur.

## 10 Static keyword

Keyword static digunakan dalam pemrograman berorientasi objek (OOP) untuk mendefinisikan properti atau method yang terkait dengan kelas itu sendiri, bukan dengan instance (objek) dari kelas tersebut. Ini berarti properti dan method static dapat diakses tanpa harus membuat objek dari kelas tersebut. Keyword static digunakan untuk membuat sesuatu menjadi "terkait dengan kelas" daripada "terkait dengan objek."

Properti Static: Properti static adalah properti yang terkait dengan kelas, bukan dengan objek. Properti ini dapat digunakan untuk menyimpan data yang bersifat global untuk seluruh objek dari kelas tersebut. Properti static dideklarasikan dengan menggunakan kata kunci static sebelum nama properti.

Method Static: Method static adalah method yang terkait dengan kelas, bukan dengan objek. Method ini dapat digunakan tanpa harus membuat objek dari kelas tersebut. Method static dideklarasikan dengan menggunakan kata kunci static sebelum nama method.

```php
class Contoh {
    public static $propertiStatic = "Ini adalah properti static.";
    
    public static function methodStatic() {
        return "Ini adalah method static.";
    }
}

// Mengakses properti static tanpa membuat objek
echo Contoh::$propertiStatic . "<br>";

// Memanggil method static tanpa membuat objek
echo Contoh::methodStatic() . "<br>";
```

## 11 Constant

Konstanta (constants) adalah nilai tetap yang tidak dapat diubah selama eksekusi program. Dalam pemrograman berorientasi objek (OOP), konstanta sering digunakan untuk menyimpan nilai-nilai yang tetap dan terkait dengan kelas. Konstanta didefinisikan dengan menggunakan kata kunci const atau define() dalam PHP.

![const](https://github.com/irfanltf/php-dasar/assets/48278734/fbf9fe65-0ab3-4ae8-a4af-7f967dddc39e)

Pentingnya penggunaan konstanta dalam OOP:

Tetap dan Terlindungi: Konstanta tidak dapat diubah selama eksekusi program, sehingga nilainya tetap konsisten.

Mudah Dikelola: Konstanta membantu dalam mengelola nilai-nilai tetap yang berhubungan dengan suatu kelas atau program, seperti nilai-nilai konfigurasi atau konstanta matematis.

Menghindari Kesalahan: Menggunakan konstanta daripada angka atau string secara langsung dapat mengurangi kesalahan manusia dalam kode.

Kode Lebih Mudah Dipahami: Konstanta memberikan nama yang berarti untuk nilai-nilai tetap, membuat kode lebih mudah dipahami oleh pembaca.

## 12 Abstract Class

Abstract class (kelas abstrak) adalah kelas yang tidak dapat diinstansiasi (tidak dapat membuat objek langsung), tetapi digunakan sebagai kerangka dasar untuk kelas-kelas turunannya (subclass). Dalam PHP, Anda mendefinisikan sebuah kelas sebagai abstrak dengan menggunakan kata kunci abstract.

Kelas abstrak dapat memiliki metode abstrak (abstract methods), yang hanya dideklarasikan (tanpa implementasi) dalam kelas abstrak. Implementasi dari metode abstrak ini harus diberikan oleh kelas-kelas turunan (subclass). Tujuan utama dari kelas abstrak adalah untuk memaksakan implementasi metode tertentu dalam kelas-kelas turunan.


## 13 Interface
Interface (antarmuka) adalah kontrak yang menggambarkan perilaku yang harus diikuti oleh kelas-kelas yang mengimplementasikannya. Dalam PHP, Anda dapat mendefinisikan sebuah interface dengan menggunakan kata kunci interface. Interface berisi deklarasi metode (tanpa implementasi) yang harus diimplementasikan oleh kelas-kelas yang menggunakan interface tersebut.

## 14 Autoloading
Autoloading adalah teknik dalam PHP yang memungkinkan Anda secara otomatis memuat kelas (class) yang dibutuhkan tanpa harus secara manual menyertakan setiap file kelas. Autoloading sangat berguna dalam pengembangan berorientasi objek (OOP) karena memungkinkan Anda untuk mengorganisasi kelas Anda ke dalam berbagai file tanpa harus mengimpor file secara manual setiap kali Anda membutuhkannya.

Dalam PHP, Anda dapat menggunakan fungsi spl_autoload_register() untuk mendaftarkan sebuah fungsi autoloader kustom yang akan dipanggil ketika PHP mencoba untuk mengakses kelas yang belum dimuat. Autoloader ini akan mencoba mencari file yang sesuai dengan nama kelas dan memuatnya jika ditemukan.

## 15 namespace

Namespace adalah fitur dalam PHP yang digunakan untuk mengatur dan mengelompokkan kelas, fungsi, dan konstanta ke dalam "ruang nama" (namespace) yang terpisah. Ini membantu menghindari konflik nama antara berbagai bagian kode dalam proyek yang lebih besar atau antara kode yang berasal dari berbagai sumber eksternal. Namespace juga meningkatkan keterbacaan dan pemeliharaan kode.

Namespace adalah seperti alamat atau label yang membantu PHP menemukan dan mengorganisir kode Anda. Bayangkan Anda memiliki banyak barang di rumah, dan Anda ingin menjaga agar barang-barang tersebut tidak bercampur aduk. Anda menggunakan label atau nama yang berbeda untuk setiap kotak agar Anda tahu di mana barang-barang tertentu disimpan.

Dalam PHP, ketika Anda membuat program yang lebih besar, Anda juga memiliki banyak "barang" (kelas, fungsi, dll.). Anda ingin mengatur mereka sehingga tidak ada kebingungan atau konflik nama. Namespace adalah cara Anda memberi "label" kepada setiap bagian kode Anda sehingga PHP tahu di mana menemukan hal itu.

Contoh:

Misalkan Anda memiliki dua kelas dengan nama yang sama, "Kendaraan," tetapi satu digunakan untuk mengendalikan mobil dan yang lainnya untuk pesawat. Ini akan membingungkan PHP jika Anda tidak memberikan petunjuk yang jelas.

```php
// Kelas Kendaraan untuk mobil
class Kendaraan {
    // ...
}

// Kelas Kendaraan untuk pesawat
class Kendaraan {
    // ...
}
```

Dengan menggunakan namespace, Anda memberikan petunjuk kepada PHP tentang di mana setiap Kelas "Kendaraan" berada:


```php
// Kelas Kendaraan untuk mobil
namespace Mobil;

class Kendaraan {
    // ...
}

// Kelas Kendaraan untuk pesawat
namespace Pesawat;

class Kendaraan {
    // ...
}
```

# 8 Berkerja dengan Database
  ## 1 Menghubungkan ke database

  buka localhost/phpmyadmin pada browser
  
  <img width="552" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/59bc8d00-5dc6-4de5-85ee-d42140d4dcb5">


  buat database, dan berinama databasenya

  <img width="659" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/28a92e6a-9e6d-4cf4-a579-716b985c1959">

  tentukan nama table dan jumlah kolom dari table yang akan dibuat

  <img width="980" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/41148b58-6e83-4031-bdf2-52b0a78e44ed">

  tentukan nama kolom, tipe data, dan juga set id menjadi primary key, serta auto increment

  <img width="1246" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/adc6885d-0715-4cf2-9b60-94d7ddbe0566">

  simpan, lalu akan tampil sebagai berikut :

  <img width="971" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/a41d79c4-5673-4dd2-b711-0243c36ecc98">

  selanjutnya adalah menghubungkan kode php ke database

  1. buat file koneksi.php yang isinya adalah konfigurasi untuk menghubungkan ke database
     
     ![var konek](https://github.com/irfanltf/php-dasar/assets/48278734/45b56bae-6f8a-4156-b81e-265e557e1c35)

  2. selanjutkan panggil class mysqli dengan parameter variabel konfigurasikan yang sudah dibuat

     ![class mysqli](https://github.com/irfanltf/php-dasar/assets/48278734/b3457301-1c30-40fa-9548-3849e489dca6)

  3. terakhir cek koneksinya, jika ada konfigurasi yang tidak benar, maka kode selanjutnya akan di die, dan ditampilkan errornya

    ![cek koneksi](https://github.com/irfanltf/php-dasar/assets/48278734/bde237fc-15d4-4027-9526-895b5f56e189)

  5. jika kita akses file koneksi.php, dan misalkan konfigurasinya salah, maka akan tampil error seperti ini

     <img width="1184" alt="image" src="https://github.com/irfanltf/php-dasar/assets/48278734/59d50052-d4cb-456c-b329-9baebd27f860">




  ## 2 Create data ke database
  ## 3 Read data pada database
  ## 4 Update data pada database
  ## 5 Delete data pada database













## License

[mirfanlutfi](https://github.com/irfanltf)
