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

**2. Variabel dalam PHP bersifat case sensitif**
PHP membedakan variabel yang ditulis dengan huruf besar dan kecil , sehingga **$belajar** tidak sama dengan **$Belajar** ataupun **$BELAJAR**, ketiganya akan dianggap sebagai variabel yang berbeda.

```php
<?php
   $ayli = "Prilia";
   echo $Ayli; // Notice: Undefined variable: Ayli
?>
Dalam contoh diatas, PHP mengeluarkan error karena tidak menemukan variabel $Ayli.
```
