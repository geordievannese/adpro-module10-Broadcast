## understanding How It Works

![alt text](img/One.png)

In this experiment, I explored a broadcast chat application using asynchronous programming and WebSockets in Rust. I started a single server process to listen for incoming connections and launched three clients from different terminals. When any client sent “hello1,” “hello2,” or “hello3,” the server received it and immediately broadcasted it to all connected clients. Each client then printed every message sent by the others, demonstrating real-time delivery. Under the hood, asynchronous tasks let the server handle multiple connections concurrently without blocking. This pattern shows how async programming excels for real-time applications like chat, where responsiveness and concurrency are essential.