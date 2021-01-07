## Melihat Perbandingan dengan Git Diff
Pada tutorial sebelumnya anda sudah melihat perubahan repositori menggunakan git log. sekarang anda akan mempelajari bagaimana cara untuk melihat perbandingan perubahan yang ada pada repositori anda. <br>
Anda dapat menggunakan script dibawah ini untuk melihat perbandingan yang ada pada repositori.
```console
git dif nomor_commit
```
Pada tutorial sebelumnya anda sudah mempelajari bagaimana cara untuk melihat `nomor commit`. Jika anda lupa bagaimana cara untuk melihatnya anda bisa cek di tutorial sebelumnya. <br><br>

Jika anda menggunakan script diatas maka hasilnya akan seperti ini.

![Hasil git Diff](1.png)

Pada gambar di atas anda melihat simbol `+` , simbol tersebut berarti anda menambahkan barisan kode. 
<br>
Jika anda melihat simbol `-` berarti anda menghapus barisan kode tersebut.

sumber `Petanikode` <br>
Contoh:

Ditambahkan:

```html 
+ <p>ini kode yang ditambahkan</p>
```
Dihapus:

```html 
- <i>ini kode yang dihapus</i>
```
Dimodifikasi/diubah:

```html 
- <span>ini kode sebelum diubah</span>
+ <span>ini kode sesudah diubah</span>
```

Sekarang kita akan mencoba merubah isi dari `index.html`.

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
Apa yang dilakukan git diff? Perintah git diff akan membandingkan perubahan yang baru saja dilakukan dengan revisi/commit terakhir.

## Melihat Perbandingan pada File
Apa bila kita melakukan banyak perubahan, maka akan banyak sekali tampil output. Karena itu, kita mungkin hanya perlu melihat perubahan untuk file tertentu saja. Untuk melihat perbandingan perubahan pada file tertentu, gunakan perintah berukut.

```console
git diff index.html
```
Perintah di atas akan melihat pebedaan perubahan pada file index.html saja.

## Melihat Perbandingan antar Revisi/Commit
Perintah untuk membandingkan perubahan pada revisi dengan revisi yang lain adalah sebagai berikut.

```console
git diff <nomer commit> <nomer commit>
```

contoh:

```console
git diff cf08ca0837cf26f1c595be36bb3a6b815e311be1 06f735af7724558164c87f6b1ce3ca7778eb1c1b
```
## Perbandingan Antar Cabang (Branch)
Kita memang belum masuk ke materi percabangan di Git. Tapi tidak ada salahnya megetahui cara melihat perbandingan perubahan antar cabang.

```cosole
git diff <nama cabang> <nama cabang>
```
