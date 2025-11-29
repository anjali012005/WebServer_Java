```yaml
project: WebServer_Java
description: >
  Java networking project demonstrating Single-threaded,
  Multithreaded, and ThreadPool-based server architectures.
  Includes a multithreaded client for load testing.
technologies:
  - Java 8+
  - ServerSocket
  - Socket
  - Threads
  - ExecutorService
  - Consumer Functional Interface
```

<img width="1893" height="762" alt="image" src="https://github.com/user-attachments/assets/f7482e83-8dd6-4748-9640-9f2f72cb4a0c" />



# 🚀 WebServer_Java

This project demonstrates how to build **network servers in Java** using:

- ✔ Single-threaded architecture  
- ✔ Multithreaded (one thread per client) architecture  
- ✔ ThreadPool-based architecture  
- ✔ A multithreaded client for stress/load testing  

Perfect for beginners learning **Java socket programming + concurrency**.

---

## 📁 Project Structure

```
WebServer_Java/
│
├── SingleThreaded/        # Basic server (1 client at a time)
├── ThreadPool/            # Server using ExecutorService
│
├── Server.java            # Multithreaded server
├── Client.java            # Multithreaded client
├── Server.class
├── Client.class
│
└── README.md
```

---

## ⚙️ Features

### 🔸 Single-Threaded Server
- Handles one client at a time  
- Easiest to understand  
- Good for learning basic blocking I/O  

### 🔸 Multithreaded Server
- Creates a new thread for each client  
- Uses `Consumer<Socket>`  
- Handles 100+ parallel clients  

### 🔸 Thread Pool Server
- Reuses threads efficiently  
- Prevents server overload  
- Best for real-world applications  

### 🔸 Multithreaded Client
- Spawns 100 threads  
- Each connects to the server  
- Prints server response  

---

## ▶️ How to Run

### **1. Compile Server**
```
javac Server.java
```

### **2. Run Server**
```
java Server
```

Output:
```
Server is listening on port 8010
```

### **3. Compile Client**
```
javac Client.java
```

### **4. Run Client**
```
java Client
```

Output example:
```
Response from Server: Hello from server /127.0.0.1:8010
```

---

## 📚 Learning Concepts

You will learn:

- How Java `ServerSocket` accepts connections  
- How `Socket` sends/receives data  
- How threads handle multiple clients  
- Why thread pools are efficient  
- Real client-server request flow  

---

## 🌟 Future Enhancements

- Add logging (SLF4J)
- Build simple HTTP server  
- Replace blocking I/O with Java NIO  
- Add GUI dashboard to monitor connections  

---

## 💛 Author<br/>
Anjali Daharwal<br/>
CS Student | Web Developer | Java Developer | Full-Stack Developer


