# TUTORIAL
---
### Nama  : Fransisca Ellya Bunaren
### NPM   : 2306152286
### Kelas : Adpro B
---
### REFLEKSI
> How much data your publisher program will send to the message broker in one run?

Program publisher akan mengirimkan sejumlah data sebesar total  5 buah data ke *message broker* dalam satu kali jalan.

> The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?

Jika publisher dan subscriber menggunakan URL koneksi yang sama (amqp://guest:guest@localhost:5672), maka keduanya berkomunikasi melalui broker yang sama. Publisher dapat mengirim pesan ke queue yang akan dibaca oleh subscriber. Ini adalah cara dasar kerja sistem message queue di mana banyak komponen dapat saling berkomunikasi secara asinkron melalui satu broker pusat.

> Screen of running RabbitMQ

![image](https://github.com/user-attachments/assets/dc5636e2-9ac9-4f11-a58b-52c412569095)

> Screen of Cargo run Publisher
Pada gambar ini, program `publisher` dijalankan 2 kali sehingga publisher mengirimkan pesan sebanyak total 10 dan program `subscriber` akan menerima 10 data.
![image](https://github.com/user-attachments/assets/9f7efc54-3177-4fe2-8d61-d63b92b1d36e)