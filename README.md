# TUGAS-PRAKTIKUM-3-SISTEM-OPERASI-SK3B

**NAMA : MIKI PURNAWAN**

**KELAS : SK3B**

**NIM : 09011282328122**


1. Lihat peralatan I/O, character device, yang ada pada system komputer

   -Lihat peralatan I/O menggunakan command prompt "ls -l /dev | ^c"

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

![c4](https://github.com/user-attachments/assets/f38d1210-c086-450b-ae67-e95a1016d7a5)

![c5](https://github.com/user-attachments/assets/50ce4e0e-fd0f-4e2a-94f0-ea36944bf9ed)

![c6](https://github.com/user-attachments/assets/fda842f5-34a6-4aee-b2ce-47dfcf96ec7d)

![c7](https://github.com/user-attachments/assets/ef60590d-eaa6-4184-908e-cb3087d6d98f)

![c8](https://github.com/user-attachments/assets/ddd37a62-7bdc-4eae-892e-025fd205fb7b)

![c9](https://github.com/user-attachments/assets/33f3b785-7435-438d-b443-07caf6d9363c)

![c10](https://github.com/user-attachments/assets/224ea7c2-3a76-48b0-aeb2-f972ffae5d1b)

