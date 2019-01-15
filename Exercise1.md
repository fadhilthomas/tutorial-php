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

Pertama buat file grade.php

```
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
