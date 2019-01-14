# Dasar-Dasar PHP

## Aturan Penulisan Variabel dalam PHP

**1. Penulisan variabel harus diawali dengan tanda $**

Variabel di dalam PHP harus diawali dengan dollar sign atau tanda dollar ($).

Contoh penulisan variabel yang **benar** dalam PHP:
```php
<?php
   $i;
   $nama;
   $Umur;
   $_lokasi_rumah;
   $ANGKA_MAKSIMUM;
?>
```
Dan berikut adalah contoh penulisan variabel yang **salah**:

```php
<?php
   $4ever; //variabel tidak boleh diawali dengan angka
   $_salah satu; //varibel tidak boleh mengandung spasi
   $nama*^; //variabel tidak boleh mengandung karakter khusus: * dan ^
?>
```
\
**2. Variabel dalam PHP bersifat case sensitif**

PHP membedakan variabel yang ditulis dengan huruf besar dan kecil , sehingga **$belajar** tidak sama dengan **$Belajar** ataupun **$BELAJAR**, ketiganya akan dianggap sebagai variabel yang berbeda.

```php
<?php
   $ayli = "Prilia";
   echo $Ayli; // Notice: Undefined variable: Ayli
?>
Dalam contoh diatas, PHP mengeluarkan error karena tidak menemukan variabel $Ayli.
```


## Cara Menampilkan Nilai Variabel (print, echo)

Untuk menampilkan nilai atau isi dari variabel, tinggal menampilkannya dengan perintah **echo** atau **print**, seperti berikut ini:

```php
<?php
   $a = 'Aku sayang';
   $b = 'Lia';
    
   echo $a . $b;
?>
```
Hasil yang didapat adalah:
```
Aku SayangLia
```
\
Kenapa kata Sayang dan Lia menyatu, karena ~~Sayang dan Lia tak mau berpisah~~ dalam variable $a dan $b, tidak memiliki spasi. Jadi agar hasil outputnya terdapat spasi maka perlu ditambahkan spasi, seperti berikut:
```php
<?php
   $a = 'Aku sayang';
   $b = 'Lia';

   echo $a . " " . $b;
?>
```
Hasil yang didapat adalah:
```
Aku Sayang Lia
```
\
Contoh lain (1):
```php
<?php
   $b = 'Lia';
   $a = 'Aku sayang $a';
   echo $a;
?>
```
Output
```
Aku Sayang Lia
```
\
Contoh lain (2):
```php
<?php
   $x = 5;
   $y = 4;
   echo $x + $y;
?>
```
Output
```
9
```
\
Contoh lain (2):
```php
<?php
   $a = 'Mas';
   $b = 'Ayli';
   echo $a . " & " . $b;
?>
```
Output
```
Mas & Ayli
```

