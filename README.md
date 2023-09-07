# php-dasar
materi php dasar
# Tipe Data dalam PHP

Tipe data dalam pemrograman PHP adalah cara untuk mengklasifikasikan dan mengelompokkan nilai-nilai berdasarkan jenis atau karakteristik tertentu. Pemahaman yang baik tentang tipe data sangat penting karena mereka memengaruhi bagaimana Anda memanipulasi dan memproses data dalam aplikasi PHP Anda. Dalam PHP, ada beberapa tipe data dasar yang umum digunakan.

## 1. Tipe Data String

Tipe data string digunakan untuk merepresentasikan teks atau karakter. String dalam PHP didefinisikan dengan tanda kutip ganda (" ") atau tanda kutip tunggal (' ').

```php
$nama = "Efika";
$alamat = 'Lampung Barat';
```

## 2. Tipe Data String

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



## License

[mirfanlutfi](https://github.com/irfanltf)
