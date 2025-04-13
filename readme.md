Nama : Muhammad Alif Pratama

Kelas : TK2B

Mata Kuliah : Sistem Operasi

1.  Login sebagai studentOS dan lihat status proses, perhatikan kolom keluaran ps –au sebagai 
berikut :

     a. Nama proses yang bukan root yaitu alif

     b. PID dan COMMAND dari proses yang paling banyak menggunakan CPU Semua proses menunjukkan %CPU = 100 Maka dipilih proses yang aktif (R+): PID: 1302 COMMAND: ps -au

  ![Cuplikan layar 2025-04-13 124714](https://github.com/user-attachments/assets/0202d50a-38de-4989-87ce-28f77c0eceaa)


     c.Buyut proses dan PID dari proses tersebut Tracing dari proses ps -au:
 
 ![image](https://github.com/user-attachments/assets/2f7d4dd7-ee8e-484e-827d-761d35b16e3d)

Jadi, buyut prosesnya adalah: 
PID: 1   COMMAND: /init

     d. beberapa proses daemon 

  ![Cuplikan layar 2025-04-13 114517](https://github.com/user-attachments/assets/f0e06c04-2c65-4dcf-9ca2-8f57ef05efc9)

     e. jalankan printah berikut
  
  -$ csh
  
 ![Cuplikan layar 2025-04-13 115037](https://github.com/user-attachments/assets/b1f74178-bac7-422a-abee-cc2369d3de6f)

-$ who , $ bash , $ ls dan $ sh

![Cuplikan layar 2025-04-13 115229](https://github.com/user-attachments/assets/9d7aefec-3659-41c4-a1e4-2a6a6b544ee7)

-$ ps

![image](https://github.com/user-attachments/assets/7f6cccc1-3c10-40bc-b17e-284121e4865d)

PID terbesar: 1275 (sh) Urutan lengkap sampai ke induk utama (PPID = 1) ditelusuri dengan ps -fp [PID]

2. Program prog.sh dengan Trap

   a). Buka file prog.sh
   ![Cuplikan layar 2025-04-13 121021](https://github.com/user-attachments/assets/898b8e16-be55-4610-8807-0c926923c740)
   b). Tulis skrip
   ![Cuplikan layar 2025-04-13 120511](https://github.com/user-attachments/assets/7e6e19d2-1c63-417f-be40-04b8ba55caf3)
   c). Ubah file agar bisa dieksekusi, jalankan program sebagai background, dan catat nomor PID dari proses tersebut
   ![Cuplikan layar 2025-04-13 121258](https://github.com/user-attachments/assets/c1e9ebf9-2e4b-4bb7-a2db-285558bde671)
   d). Kirim sinyal satu per satu
![Cuplikan layar 2025-04-13 121638](https://github.com/user-attachments/assets/f2ddaf7a-5e59-470c-9cc1-acc1a5c913e1)
   Nomor sinyal yang digunakan menghentikan proses diatas yaitu $ kill -2 872
3. Program myjob.sh dengan Auto-Hapus File

   a). Buka file myjob.sh

   ![Cuplikan layar 2025-04-13 122233](https://github.com/user-attachments/assets/38d141a2-cdc0-4628-9d51-9eee68cee82c)

   b). Isi skrip

  ![Cuplikan layar 2025-04-13 122154](https://github.com/user-attachments/assets/cf0e65f5-5047-4930-89d6-7d6d2166fad6)


   c). Buat executable, jalankan dibackground, dan Cek nomor PID nya

  ![image](https://github.com/user-attachments/assets/b262befa-baa9-4b2d-96e8-650b5172d19d)

   d). Hentikan proses dengan sinyal 15 

   ![Cuplikan layar 2025-04-13 133001](https://github.com/user-attachments/assets/18c674c5-1d01-4b4e-b34d-b9a2d2dc88d2)
   
   proses dihentikan dengan kill -15 1391, muncul:
   
   ![Cuplikan layar 2025-04-13 133015](https://github.com/user-attachments/assets/c74a5cb9-1e35-4007-802d-c69a03ecd8ca)

File berkas dan hasil otomatis terhapus Fungsi trap berjalan sukses.


   


   

   




  

   




