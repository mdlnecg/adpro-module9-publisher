# Tutorial 9 Pemrograman Lanjut: Publisher
### Madeline Clairine Gultom - 2306207846 - ADPRO A

> How much data your publisher program will send to the message broker in one run?

Data yang dikirim adalah sebanyak lima pesan dengan masing-masing pesan bertipe `UserCreatedEventMessage`.

> The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean? 

Penggunaan URL yang sama ini bertujuan agar publisher dan subscriber dapat terhubung ke message broker yang sama sehingga pesan yang dikirim oleh publisher dapat diterima oleh subscriber.

# Message Broker (RabbitMQ)
### Running RabbitMQ as Message Broker
![image](https://github.com/user-attachments/assets/4ea55a0b-45f3-4332-8ec1-c1ae7368c3ab)
