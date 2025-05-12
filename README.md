# TUTORIAL
---
### Nama  : Fransisca Ellya Bunaren
### NPM   : 2306152286
### Kelas : Adpro B
---
### REFLEKSI
> How much data your publisher program will send to the message broker in one run?  
Program publisher akan mengirimkan sejumlah data sebesar total X byte/kilobyte/megabyte yang berasal dari Y pesan masing-masing berukuran sekitar Z byte ke message broker dalam satu kali dijalankan.

> The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? 
Jika publisher dan subscriber menggunakan URL koneksi yang sama (amqp://guest:guest@localhost:5672), maka keduanya berkomunikasi melalui broker yang sama. Publisher dapat mengirim pesan ke queue yang akan dibaca oleh subscriber. Ini adalah cara dasar kerja sistem message queue di mana banyak komponen dapat saling berkomunikasi secara asinkron melalui satu broker pusat.