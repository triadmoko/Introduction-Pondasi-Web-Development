## Melihat Perbandingan dengan Git Diff
Pada tutorial sebelumnya anda sudah melihat perubahan repositori menggunakan git log. sekarang anda akan mempelajari bagaimana cara untuk melihat perbandingan perubahan yang ada pada repositori anda. <br>
Anda dapat menggunakan script dibawah ini untuk melihat perbandingan yang ada pada repositori.
```console
git diff nomor_commit
```
Pada tutorial sebelumnya anda sudah mempelajari bagaimana cara untuk melihat `nomor commit`. Jika anda lupa bagaimana cara untuk melihatnya anda bisa cek di tutorial sebelumnya. <br><br>

Jika anda menggunakan script diatas maka hasilnya akan seperti ini.

![Hasil git Diff](1.png)

Pada gambar di atas anda melihat simbol `+` , simbol tersebut berarti anda menambahkan barisan kode. 
<br>
Jika anda melihat simbol `-` berarti anda menghapus barisan kode tersebut.

<b>sumber : Petani Kode<b>
Contoh:

Ditambahkan:

`+ <p>ini kode yang ditambahkan</p>`
Dihapus:

`- <i>ini kode yang dihapus</i>`
Dimodifikasi/diubah:

- <span>ini kode sebelum diubah</span>
+ <span>ini kode sesudah diubah</span>
Sekarang kita akan mencoba merubah isi dari index.html.

Sebelum diubah:
```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Belajar Git - Project 01</title>
    </head>
    <body>
        <p>Hello Semua, Saya sedang belajar Git</p>
    </body>
</html>
```
Setelah diubah:
```html
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Belajar Git - Project 01</title>
    </head>
    <body>
        <p>Hello Dunia!, Saya sedang belajar Git</p>
    </body>
</html>
```
Setelah itu lakukan jalankan perintah git diff lagi.

Perbedaan revisi
