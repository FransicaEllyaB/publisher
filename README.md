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

Gambar terminal `publisher` di mana telah berhasil menjalankan cargo run untuk mengirim data melalui message broker

![{1A8F535C-573A-4EC6-B754-5C932BE191FF}](https://github.com/user-attachments/assets/c136420b-5e26-4200-9f8f-ff5ce841fd1c)

> Screen of Chart pada `rabbitmq`
Screenshoot RabitMQ di mana ada spike pada message rates yang disebabkan karena menjalankan publisher berkali-kali.

![Screenshot 2025-05-12 230349](https://github.com/user-attachments/assets/ecc92114-8bb1-4322-a395-30954cc59bd3)