This repository contains multiple examples of Java-based client-server architectures implemented using TCP sockets and multithreading techniques.

## 📂 Project Structure
.
├── SingleThreaded/

│ ├── Client.java # Basic one-to-one socket communication

│ └── Server.java

├── Multithreaded/

│ ├── Client.java # Client spawns 100 threads; server handles each in new thread

│ └── Server.java

├── ThreadPool/

│ └── Server.java # Server uses fixed thread pool to manage client connections

├── README.md


---

## 🔧 Technologies Used

- Java 8+
- TCP/IP Socket Programming
- Multithreading (Thread, Runnable)
- Thread Pooling (`ExecutorService`, `Executors.newFixedThreadPool`)

---

## 💡 Project Descriptions

### 🧵 1. SingleThreaded

A basic server that handles one client at a time. Great for understanding fundamental concepts of sockets, I/O streams, and communication protocol.

> Folder: `SingleThreaded/`

### 🧵 2. Multithreaded

Each incoming client connection is handled in a new Java `Thread`, simulating 100 clients connecting concurrently to the server.

> Folder: `Multithreaded/`

### 🧵 3. ThreadPool

Improves over thread-per-connection by using a fixed-size thread pool to efficiently manage resources and scale better under load.

> Folder: `ThreadPool/`

---

## 🚀 How to Run

> Use separate terminals for client and server.

### Compile
javac FolderName/*.java

Run Server
java FolderName.Server

Run Client (if applicable)
java FolderName.Client


✅ Features
🔌 TCP Socket-based Communication

🧵 Single-threaded, Multithreaded, and Thread Pool Architectures

🧹 Clean exception and resource handling

📚 Educational examples for networking and multithreading in Java

📸 Sample Output
Server is listening on port 8010
Connected to /127.0.0.1:XXXXX
Response from Server Hello from server /127.0.0.1
🧑‍💻 Author
Mainak

📄 License
This project is licensed under the MIT License.
