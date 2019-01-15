# Latihan 1 Calculator

```
Contoh Soal:
Buatlah sebuah form pada file ‘calculator.php’ yang berisi : 
2 textfield , name='angka1' dan name='angka2' 
1 Option dengan 4 option ( value nya =  +,  - , * , / ) 
1 Submit dengan value ‘Hitung’
```
<br>
Pertama buat file calculator.php

```php
<html>
<head>
<title>Kalkulator</title>
</head>
<body>
	<form action="hasil_calculator.php" method="post">
		<input type="text" name="angka1"> 
		<select name="operator">
            		<option value="+">+</option>
            		<option value="-">-</option>
            		<option value="x">x</option>
			<option value="/">/</option>
        	</select>
		<input type="text" name="angka1">
		<input type="submit" value="Hitung">
	</form>
</body>
</html>
```
