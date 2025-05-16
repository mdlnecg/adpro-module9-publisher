![image](https://github.com/user-attachments/assets/72f29cfd-5bc7-432e-ad23-f4187d34dc98)# Tutorial 9 Pemrograman Lanjut: Publisher
### Madeline Clairine Gultom - 2306207846 - ADPRO A

> How much data your publisher program will send to the message broker in one run?

Data yang dikirim adalah sebanyak lima pesan dengan masing-masing pesan bertipe `UserCreatedEventMessage`.

> The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? 

Penggunaan URL yang sama ini bertujuan agar Publisher dan Subscriber dapat terhubung ke message broker yang sama sehingga pesan yang dikirim oleh Publisher dapat diterima oleh Subscriber.

# Message Broker (RabbitMQ)
### Running RabbitMQ as Message Broker
![image](https://github.com/user-attachments/assets/4ea55a0b-45f3-4332-8ec1-c1ae7368c3ab)

### Sending and processing event
![image](https://github.com/user-attachments/assets/08ad5eae-54be-4a3d-a0e5-4a84bc1c538d)
![image](https://github.com/user-attachments/assets/81373070-b52c-4d74-9324-9517b60e2906)

Melalui proses ini, kita dapat melihat ketika koneksi sudah terhubung dengan suatu message broker, lalu ketika kita jalankan `cargo run` pada Publisher, akan dikirimkan lima pesan yang kemudian diproses oleh Subscriber ketika kita jalani `cargo run` juga. Pada contoh di atas, saya mencoba untuk menjalani proses ini satu kali yang terbukti mengirimkan lima data ke Subscriber.

### Monitoring chart based on publisher
![image](https://github.com/user-attachments/assets/481833f1-0ca5-4506-90fa-a6f2a5ae579c)
![image](https://github.com/user-attachments/assets/4d3547dd-50fb-41cc-ac95-bda735b6edee)
Pada percobaan kali ini, saya mencoba melakukan run pada Publisher lebih dari sekali, maka data yang diterima dan diproses oleh Subscriber juga akan lebih banyak dari sebelumnya. Kita dapat lihat grafik pada RabbitMQ di bagian "Message Rates", terlihat bahwa ada peningkatan dan penurunan sesuai proses yang dijalani setiap lima detik. 
