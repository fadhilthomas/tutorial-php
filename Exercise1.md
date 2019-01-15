# Latihan1

## Latihan Form Handling

```
Contoh Soal:
Buatlah sebuah form  pada file grade.php yang berisi : 
1 textbox
1 submit dengan value = 'generate'  

Buatlah sebuah conditional statement yang dapat menentukan grade nilai,
Dengan ketentuan / kondisi sebagai berikut : 
>Untuk nilai 80 s.d. 100  = Grade anda 'A'
>Untuk nilai 70 s.d. 79 = Grade Anda 'B' 
>Untuk nilai 60 s.d. 69 = Grade Anda 'C'
>Untuk nilai dibawah < 60 = Anda tidak lulus

Hasilnya tampilkan ke halaman file php baru yaitu cek_grade.php
```
<br>
Pertama buat file grade.php


```php
<html>
<head>
<title>Cek Nilai</title> //Untuk Judul
</head>
<body>
    <form action="cek_grade.php" method="post"> //Form dengan action ke file 'cek_grade.php' dan metode 'POST'
        Nilai: <input type="text" name="nilai"> //Textbox dengan nama 'nilai'
        <br><br>
        <input type="submit" value="Generate"> //Tombol submit dengan value 'generate'
    </form>
</body>
</html>
```
<br>
Kedua buat file cek_grade.php

```php
<html>
<head>
<title>Hasil Nilai</title>
</head>
<body>
<?php
	if(isset($_POST["nilai"])){
		$nilai = $_POST["nilai"]; //Nilai dari 'nilai' dimasukkan ke dalam variable $nilai;
		if($nilai >= 80 && $nilai <= 100){
			echo "Grade anda 'A'";
		}else if($nilai >= 70 && $nilai <= 79){ 
			echo "Grade anda 'B'";
		}
		else if($nilai >= 60 && $nilai <= 69){
			echo "Grade anda 'C'";
		}
		else if($nilai < 60){
			echo "Anda tidak lulus";
		}
	}
?>

</body>
</html>
```
<br>
<br>
## Penjelasan
<br>
* Fungsi $_POST["nilai"] adalah untuk menerima data dari 'nilai' yang menggunakan meteode POST. Jadi apabila metodenya menggunakan get maka pakai $_GET["nilai"]. Kemudian fungsi isset adalah untuk memeriksa apakah data 'nilai' ada nilanya atau tidak. Jadi apabila (if) 'nilai' tidak kosong, maka kode di dalam if akan dieksekusi.
* Kemudian dalan if($nilai >= 80 && $nilai <= 100). Jika isi dari variable $nilai 80 sampai 100 maka akan mencetak tulisan "Grade anda 'A'" dengan echo.
* Apabila if yang di atas tidak terpenuhi maka, akan memeriksa kondisi dibawahnya dengan menambahkan syntax 'else if'. Jika isi dari variable $nilai 70 sampai 79 maka akan mencetak tulisan "Grade anda 'B'" dan seterusnya sampai if terakhir di bawah.
<br>
Kemudian lakukan ujicoba.
