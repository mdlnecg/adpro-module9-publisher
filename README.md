![image](https://github.com/user-attachments/assets/72f29cfd-5bc7-432e-ad23-f4187d34dc98)# Tutorial 9 Pemrograman Lanjut: Publisher
### Madeline Clairine Gultom - 2306207846 - ADPRO A

> How much data your publisher program will send to the message broker in one run?

Data yang dikirim adalah sebanyak lima pesan dengan masing-masing pesan bertipe `UserCreatedEventMessage`.

> The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? 

Penggunaan URL yang sama ini bertujuan agar publisher dan subscriber dapat terhubung ke message broker yang sama sehingga pesan yang dikirim oleh publisher dapat diterima oleh subscriber.

# Message Broker (RabbitMQ)
### Running RabbitMQ as Message Broker
![image](https://github.com/user-attachments/assets/4ea55a0b-45f3-4332-8ec1-c1ae7368c3ab)

### Sending and processing event
![image](https://github.com/user-attachments/assets/08ad5eae-54be-4a3d-a0e5-4a84bc1c538d)
![image](https://github.com/user-attachments/assets/81373070-b52c-4d74-9324-9517b60e2906)

Melalui proses ini, kita dapat melihat ketika koneksi sudah terhubung dengan suatu message broker, lalu ketika kita jalankan `cargo run` pada publisher, akan dikirimkan lima pesan yang kemudian diproses oleh subscriber ketika kita jalani `cargo run` juga. Pada contoh di atas, saya mencoba untuk menjalani proses ini satu kali yang terbukti mengirimkan lima data ke subscriber.
