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

Kelompok 3: 0
Kelompok 7 : 0
Kelompok 5 : 60
Kelompok 2 : 0;
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

## License

[mirfanlutfi](https://github.com/irfanltf)
