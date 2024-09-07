# TUGAS-PRAKTIKUM-3-SISTEM-OPERASI-SK3B

**NAMA : MIKI PURNAWAN**

**KELAS : SK3B**

**NIM : 09011282328122**


1. Lihat peralatan I/O, character device, yang ada pada system komputer

   -Lihat peralatan I/O menggunakan command prompt "ls -l /dev | grep ^c"

![c1](https://github.com/user-attachments/assets/d8bd06c5-8983-42bc-89fb-1a8048c1ac24)

   -Lihat character device menggunakan command prompt "ls -l /dev/tty0" untuk command prompt ini tidak harus diakhiri tty0, bisa juga pakai zero atau yang lain, yang jelas I/O yang ingin dilihat character device nya

![Screenshot 2024-09-07 115336](https://github.com/user-attachments/assets/40ae0fa7-310e-4823-9fc1-0441f58374e9)

2. Buatlah sub direktori januari, februari dan maret sekaligus pada direktori Latihan5

   -Untuk mengerjakan nomor 2, pertama-tama kita buat dulu direktori utama yang menampung direktori Januari, Februari dan Maret yang kita beri nama Latihan5. Untuk membuat direktori kita gunakan command "mkdir Latihan5" setelah itu masuk ke direktori nya dengan menggunakan command "cd \Latihan5", kemudian kita buat direktori januari, februari dan maret nya menggunakan command yang sama yaitu "mkdir Januari && mkdir Februari && mkdir Maret"

   ![c2](https://github.com/user-attachments/assets/1e329426-56fe-4c86-b5e5-a9e7d1a00620)

3. Buatlah file dataku yang berisi nama, nim dan alamat anda pada sub direktori januari dan copy-kan file tersebut ke sub direktori februari dan maret

   -Setelah kita sudah membuat direktori nya, sekarang kita membuat sebuah file yang berisi nama, nim, dan alamat tapi karena saya keliru membaca soal saya malah membuat file dengan isi nama, nim, kelas, dan alamat. Baiklah untuk membuat file kita masuk dulu ke direktori Januari setelah itu kita gunakan command "touch Dataku.txt" setelah itu kita gunakan command prompt "nano Dataku.txt" note : jika nano tidak bisa digunakan, cobalah untuk menginstall nano terlebih dahulu menggunakan command "sudo apt install nano
" Setelah mengetik command tersebut kita akan masuk ke tampilan/isi dari file Dataku.txt itu jadi langkah selanjutnya adalah mengisi file tersebut dengan nama, nim, dan alamat (kelas tidak perlu diisi) Setelah mengisi ketik ctrl + x kemudian nano akan memberikan peringatan atau tulisan apakah isi file nya akan disave atau tidak, jika ada ketik Y kemudian enter dan jangan lupa cek isi nya dengan command cat Dataku.txt. Kita sudah berhasil membuat file Dataku.txt yang berisi nama, nim, dan kelas, sekarang kita akan mengcopy file Dataku.txt di direktori Januari ke direktori Februari dan Maret caranya dengan menggunakan command "cp Dataku.txt (tujuan copy nya ke direktori mana, untuk mengecek ketik pwd ketika berada di direktori yang diinginkan)" jika sudah coba cek di direktori maret dan februari apakah file Dataku.txt berhasil tercopy menggunakan command ls

![c3](https://github.com/user-attachments/assets/c54ba73b-653a-4567-ac0f-4a31c062a7ac)

4. Ubahlah ijin akses file dataku pada sub direktori januari sehingga group dan others dapat melakukan write

   - Untuk mengubah izin akses file pada direktori januari kita gunakan command "chmod go+w (lokasi file yang ingin diubah aksesnya contoh : /home/miki-purnawan/Latihan/Januari/Dataku.txt)" setelah itu cek file nya apakah sudah berubah izin akses nya dengan cara "ls -l (lokasi file berada contohnya sama seperti saat mengubah akses file)" jika output nya adalah "-rw-rw-rw-" atau ada w di kedua dan tiga maka benar karena rw kedua dan ketiga itu untuk Group dan Others serta rw adalah Read Write 

![c4](https://github.com/user-attachments/assets/f38d1210-c086-450b-ae67-e95a1016d7a5)

5. Ubahlah ijin akses file dataku pada sub direktori februari sehingga user dapat melakukan baik write, read maupun execute, tetapi group dan others hanya bisa read dan execute

  - Sekarang kita ubah ijin akses file dataku pada direktori februari agar hanya user yang dapat melakukan read write dan execute tetapi grup dan others hanya read execute, caranya gunakan command "chmod u=rwx,go=rx (lokasi file yang ingin diubah izin aksesnya)" kemudian jika sudah periksa izin akses nya menggunakan command yang sama seperti di nomor 4 yaitu ls -l (lokasi file) tapi jika kalian sudah berada di direktori februari kalian hanya perlu ls -l Dataku.txt saja, jika output nya adalah -rwxr-xr-x-" maka itu benar karena sesuai dengan tugas nya

![c5](https://github.com/user-attachments/assets/50ce4e0e-fd0f-4e2a-94f0-ea36944bf9ed)

6. Ubahlah ijin akses file dataku pada sub direktori maret sehingga semua dapat melakukan write, read dan execute

   - Untuk melakukan ini kita cukup gunakan command "chmod a=rwx (a = all yang berarti semua bisa read, write dan execute) Dataku.txt (jika kalian sudah berada di direktori Maret, jika tidak kalian harus mengetik lokasi file nya berada)" kemudian cek izin akses nya apakah output nya adalah -rwx-rwx-rwx atau -rwxrwxrwx- jika seperti itu maka benar

![c6](https://github.com/user-attachments/assets/fda842f5-34a6-4aee-b2ce-47dfcf96ec7d)

7. Hapuslah direktori maret

   - Gunakan command "rm -rf Maret (jika kalian berada di direktori Latihan5, jika tidak kalian bisa gunakan command rm - rf (lokasi direktori yang ingin dihapus))" setelah itu cek menggunakan ls di direktori Latihan5 saja atau bisa mengikuti cara seperti saya

![c7](https://github.com/user-attachments/assets/ef60590d-eaa6-4184-908e-cb3087d6d98f)

8. Ubahlah kepemilikan sub direktori februari sehingga user dan group hanya read, dan cobalah untuk membuat membuat direktori baru haha pada sub direktori februari

   -Kita ubah izin akses direktori februari menggunakan command "chmod 444 (lokasi direktori yang ingin diubah)" kemudian coba lah untuk membuat direktori baru di dalam direktori februari atau coba masuk ke dalam direktori februari, jika permission denied maka kita sudah berhasil mengubah izin akses direktori nya

![c8](https://github.com/user-attachments/assets/ddd37a62-7bdc-4eae-892e-025fd205fb7b)

9. Modifikasi umask dari file dataku pada sub direktori januari menjadi 027 dan berapakan nilai default-nya ? 

   -Untuk nomor 9 kita cek dulu nilai default nya berapa dengan command "umask" biasanya nomor umask default adalah 0002, kemudian modifikasi umask ke 027 dengan cara "umask 027" efek umask yang sudah dimodifikasi hanya berlaku untuk file/direktori baru dan untuk yang lama itu harus diubah sendiri menggunakan chmod (027 artnya 0 = user tidak ada batasan, 2 = group hanya bisa read dan 7 = others dibatasi sepenuhnya) jika ingin mengecek efek dari umask 027 kita cukup buat file baru kemudian cek izin akses nya jika outputnya adalah -rw-r----- maka itu sesuai dengan umask 027

![c9](https://github.com/user-attachments/assets/33f3b785-7435-438d-b443-07caf6d9363c)

10. Buatlah link dari file dataku ke file dataku.ini dan file dataku.juga dan dengan perintah list perhatikan berapa link yang terjadi

   -Untuk membuat link dari file Dataku.txt ke .juga dan .ini kita gunakan perintah "ln (lokasi file dataku contoh : /home/miki-purnawan/Desktop/Latihan5/Januari/Dataku.txt kemudian spasi dan ketikkan lokasi yang sama hanya saja ubah Dataku.txt menjadi Dataku.ini begitupun dengan Dataku.juga) jika sudah dilink langkah selanjutnya adalah mengecek berapa link yang terjadi dengan command : ls -l (jika kalian berada di direktori Januari, jika tidak ikutin yang seperti di gambar)

![c10](https://github.com/user-attachments/assets/224ea7c2-3a76-48b0-aeb2-f972ffae5d1b)

