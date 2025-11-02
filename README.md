# 🧠 Online Examination System

A **Java-based desktop application** for conducting, managing, and evaluating exams in real-time.
The system enables multiple users to connect simultaneously using **socket programming and multithreading**, stores data securely in a **MySQL database**, and maintains logs using **file I/O**.

---

## 🚀 Features

* Real-time exam conduction and auto-evaluation
* Role-based access (Admin / Student)
* Secure login with password hashing
* Timed exams with session management
* Multi-threaded server for concurrent users
* Simple and modern Swing-based user interface
* Activity logging through file operations

---

## 🧩 Project Structure

```
examsystem/
├── client/
│   └── ClientMain.java
├── common/
├── resources/
│   └── mysql-connector-j-9.3.0.jar
├── server/
│   └── ServerMain.java
```

---

## ⚙️ Prerequisites

* **Java JDK 11** or higher
* **MySQL 8.0** or higher (make sure MySQL is installed and running)

---

## 🧱 Setup Instructions

1. **Download or clone the repository:**

   ```bash
   git clone https://github.com/Nikodimos-Software-Engineering/Online_Examination_System.git
   cd Online_Examination_System/examsystem
   ```

2. **Ensure MySQL is running.**
   The system connects to the database using:

   ```java
   jdbc:mysql://localhost:3306/online_exam_system
   ```

   If needed, update the connection details in your source code to match your local setup.

3. **Run the Server:**

   * Open your IDE or terminal.
   * Run:

     ```bash
     java client/ServerMain.java
     ```
   * Or directly execute the provided JAR file:

     ```bash
     java -jar resources/mysql-connector-j-9.3.0.jar
     ```

4. **Run the Client:**

   * Open another terminal (or another computer in the same network).
   * Run:

     ```bash
     java client/ClientMain.java
     ```

---

## 🧠 Development Notes

* The project follows the **MVC architecture** (Model-View-Controller).
* All networking logic uses **Java sockets**.
* Logging is handled using simple file-based logs in the `resources` folder.
* You can test the system locally by running both **Client** and **Server** on the same machine.

---

## 🧩 Folder Summary

| Folder       | Description                                                 |
| ------------ | ----------------------------------------------------------- |
| `client/`    | Handles GUI, user interaction, and client-side logic        |
| `server/`    | Manages users, exams, and communication between clients     |
| `common/`    | Shared classes, constants, and utilities used by both sides |
| `resources/` | Contains JAR files and configuration data                   |

---

## 📜 License

This project is licensed under the **MIT License** – see the `LICENSE` file for details.

---
