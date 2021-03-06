Tutorial Penggunaan Git
                                                                                                                                        
Apa itu Git? 

- Git adalah salah satu sistem pengontrol versi (Version Control System) pada proyek perangkat lunak yang diciptakan oleh Linus Torvalds.
- Pengontrol versi bertugas mencatat setiap perubahan pada file proyek yang dikerjakan oleh banyak orang maupun sendiri.
- Git dikenal juga dengan distributed revision control (VCS terdistribusi), artinya penyimpanan database Git tidak hanya berada dalam satu tempat saja


Menambahkan Global Config

- Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi user name dan user email                            
- Konfigurasi ini bisa dilakukan untuk global repostiry atau individual repository.                                   
- Apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi kegagalan saat menjalankan perintah git commit                    
- Lakukan "git config --global user.email dan name " supaya bisa login github ketika push #  
![config](https://user-images.githubusercontent.com/46749350/51788075-b75c4300-212e-11e9-8323-2d41c528e2c2.jpg)

Perintah Dasar Git

- git init, perintah untuk membuat repository local
- git add, perintah untuk menambahkan file baru, atau perubahan pada file pada staging sebelum proses commit.
- git commit, perintah untuk menyimpan perubahan kedalam database git.
- git push -u origin master, perintah untuk mengirim perubahan pada repository local menuju server repository.
- git clone [url], perintah untuk membuat working directory yang diambil dari repositry sever.
- git remote add origin [url], perintah untuk menambahkan remote server/reopsitory server pada local repositry (working directory)     

Membuat Repository Local

- Buka direktory aktif, misal: c:/Latihan
- Buat direktory project praktikum pertama dengan nama Latihan
- Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya masuk kedalam direktori tersebut dengan perintah cd (change directory)
- Direktory aktif menjadi: c:/Latihan
- Buatlah direktory "Latihan" kemudian masuk ke direktory tersebut                                               
![cd](https://user-images.githubusercontent.com/46749350/51788097-fe4a3880-212e-11e9-88a0-f73a8a545c25.jpg)                         


- Lakukan "git init" untuk menjadikan repository lokal                                                            
![git init](https://user-images.githubusercontent.com/46749350/51788185-f2ab4180-212f-11e9-8a1e-f9e192a50229.jpg)

- Buat File Bernama "README.md" (text file), jika file berhasil dibuat, akan tampil seperti dlm gambar                              
![echo](https://user-images.githubusercontent.com/46749350/51788211-3736dd00-2130-11e9-9b29-40e2b5880ed7.jpg)

- Kemudian tambahkan file tersebut ke repository dengan " git add README.md, file yang berhasil ditambahkan akan terlihat seperti di gambar, dengan "git status"                                                           
![git add readme](https://user-images.githubusercontent.com/46749350/51788268-b1676180-2130-11e9-9213-9a648b56d6c6.jpg)

- Untuk Menyimpan perubahan sebuah file ke repository local gunakan printah " git commit -m "perubahan yang terjadi"                 
![git commit](https://user-images.githubusercontent.com/46749350/51788283-0b682700-2131-11e9-9395-8fc54405cb46.jpg)


Membuat Repository Server

- Server reopsitory yang akan kita gunakan adalah http://github.com
- Anda harus membuat akun terlebih dahulu. • Pada laman github, klik tombol start a project, atau
- Dari menu (icon +) klik New Repository                                                                             
![new repo](https://user-images.githubusercontent.com/46749350/51792503-91eb2b80-2166-11e9-83b1-8f39c8c78aea.jpg)


Membuat Repository Server 

- Isi nama repositorynya, misal: Latihan1.
- lalu klik tombol Create repository                                                                                
![judul](https://user-images.githubusercontent.com/46749350/51792527-23f33400-2167-11e9-98ea-f0b8e4c4beec.jpg)

Menambahkan Remote Repository 

- Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.
- Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url]                                          
![url](https://user-images.githubusercontent.com/46749350/51792628-a5979180-2168-11e9-84fc-4b9e346eb0d9.jpg)

Push (Mengirim perubahan ke server) 

- Untuk mengirim perubahan pada local repository ke server gunakan perintah git push.
- Perintah ini akan meminta memasukkan username dan password pada akun github.com
- Gunakan printah " git push -u origin master"                                                                               
![git push](https://user-images.githubusercontent.com/46749350/51788309-6732b000-2131-11e9-8968-8e8644b729e7.jpg)


Melihat hasilnya pada server repository 

- Buka laman github.com, arahkan pada repositori- nya.
- Maka perubahan akan terlihat pada laman tersebut. #                                                              
![tampilan](https://user-images.githubusercontent.com/46749350/51788328-a8c35b00-2131-11e9-98ee-d13a9ffaa1f7.jpg)
