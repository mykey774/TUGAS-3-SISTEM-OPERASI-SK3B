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
" Setelah mengetik command tersebut kita akan masuk ke tampilan/isi dari file Dataku.txt itu jadi langkah selanjutnya adalah mengisi file tersebut dengan nama, nim, dan alamat (kelas tidak perlu diisi) Setelah mengisi ketik ctrl + x kemudian nano akan memberikan peringatan atau tulisan apakah isi file nya akan disave atau tidak, jika ada ketik Y kemudian enter dan jangan lupa cek isi nya dengan command cat Dataku.txt. Kita sudah berhasil membuat file Dataku.txt yang berisi nama, nim, dan kelas, sekarang kita akan mengcopy file Dataku.txt di direktori Januari ke direktori Februari dan Maret caranya dengan menggunakan command

sudo apt install nano


