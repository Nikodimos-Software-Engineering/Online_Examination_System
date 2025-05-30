# Online Examination System

A Java-based desktop application for conducting, managing, and evaluating exams in real-time. The system supports concurrent users through socket programming and multithreading, ensures data persistence using a relational database, and maintains a log of activities via file I/O.

## Features

- Real-time exam conduction and evaluation
- User-friendly Swing-based GUI
- Role-based access (Admin/Student)
- Real-time chat system
- Community posting board (Q&A)
- Session management for timed exams
- Secure authentication with password hashing
- Modular structure using MVC pattern

## Prerequisites

- Java JDK 11 or higher
- Maven 3.6 or higher
- MySQL 8.0 or higher

## Project Structure

```
Online_Examination_System/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── examsystem/
│   │   │           ├── client/
│   │   │           ├── server/
│   │   │           ├── common/
│   │   │           └── resources/
│   │   └── resources/
│   └── test/
│       └── java/
├── lib/
├── docs/
└── logs/
```

## Setup Instructions

1. Clone the repository:

   ```bash
   git clone [repository-url]
   cd Online_Examination_System
   ```

2. Configure the database:

   - Create a MySQL database
   - Update `src/main/resources/config/database.properties` with your database credentials

3. Build the project:

   ```bash
   mvn clean install
   ```

4. Run the server:
   ```bash
   java -jar target/online-examination-system-1.0-SNAPSHOT.jar
   ```

## Development

- The project uses Maven for dependency management
- Follow the MVC pattern for new features
- Write unit tests for new functionality
- Use the provided logging system for debugging

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
