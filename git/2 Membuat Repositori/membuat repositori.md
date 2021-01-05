## Membuat Repositori
untuk membuat repositori menggunakan git bisa mengetikkan script berikut : <br>
```console
git init .
```
atau
```console
git init nama_project
```
- `git` berfungsi menjalankan instruksi git didalam terminal. 
- `init` berfungsi untuk menginisialisasi folder tersebut akan dijadikan untuk repositori atau working area. 
***
## Tahapan File dalam Menyimpan Perubahan
git merupakan version control yang terstruktur, maka ada beberapa tahapan yang harus dilalui agar bisa menyimpan setiap perubahan yang dilakukan di working area. ada 3 tahap yang dilalui oleh git yaitu seperti berikut<br>

1. Tahap Modified
   <br> Pada tahap modified merupakan tahap pertama yang dilalui untuk menyimpan perupahan setelah membuat repositori, ditahap ini anda dapat melakukan perubahan-perubahan di dalam working area, seperti menambah `file`, `folder/directory` dan juga update `file`.
2. Tahap Stage
   <br> Pada tahap ini anda dapat menandai `file` atau `folder` yang akan disimpan ke dalam oleh git. untuk menandai `file` atau ` foldedr tersebut bisa menggunakan script berikut 
   ```console 
   git add . 
   ```
   atau
   ``` console
   git add nama_file1 nama_file2 nama_folder1
   ```
   anda juga bisa menandai satu persatu `file`.

3. Tahap Commit
   <br>Tahap ini merupakan tahap terakhir anda untuk menyimpan perubahan menggunakan git. anda dapat melakukan penyimpanan perubahan setelah anda menandai `file` atau `folder` di tahap kedua. untuk menyimpan perubahan anda bisa menulis script berikut :
   ```console
   git commit -m "pesan"
   ```

   - `commit` Melakukan penyimpanan perubahan pada file anda. 
   - `-m` Memberikan pesan pada file yang akan di commit (disimpan). 