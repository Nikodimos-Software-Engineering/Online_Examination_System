# Online Examination System - Project Structure

## 📁 Root Directory Structure

```
Online_Examination_System/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── com/
│   │   │   │   └── examsystem/
│   │   │   │       ├── client/
│   │   │   │       ├── server/
│   │   │   │       ├── common/
│   │   │   │       └── resources/
│   │   │   └── resources/
│   │   └── test/
│   │       └── java/
│   ├── lib/
│   └── docs/
├── build/
└── logs/
```

## 📦 Package Structure

### 1. Client Package (`com.examsystem.client`)

```
client/
├── gui/
│   ├── admin/
│   │   ├── AdminDashboard.java
│   │   ├── ExamEditor.java
│   │   └── UserManagement.java
│   ├── student/
│   │   ├── StudentDashboard.java
│   │   ├── ExamView.java
│   │   └── ResultView.java
│   └── common/
│       ├── LoginFrame.java
│       └── ChatWindow.java
├── controller/
│   ├── AdminController.java
│   ├── StudentController.java
│   └── AuthController.java
└── model/
    ├── User.java
    ├── Exam.java
    └── Result.java
```

### 2. Server Package (`com.examsystem.server`)

```
server/
├── core/
│   ├── ServerMain.java
│   ├── ClientHandler.java
│   └── ThreadManager.java
├── service/
│   ├── AuthenticationService.java
│   ├── ExamService.java
│   ├── ChatService.java
│   └── LoggingService.java
└── dao/
    ├── DatabaseManager.java
    ├── UserDAO.java
    ├── ExamDAO.java
    └── ResultDAO.java
```

### 3. Common Package (`com.examsystem.common`)

```
common/
├── model/
│   ├── Question.java
│   ├── Answer.java
│   └── Message.java
├── util/
│   ├── Constants.java
│   ├── ConfigManager.java
│   └── SecurityUtil.java
└── exception/
    ├── ExamException.java
    └── DatabaseException.java
```

### 4. Resources Package

```
resources/
├── config/
│   ├── database.properties
│   └── server.properties
├── sql/
│   └── schema.sql
└── icons/
    └── (UI icons)
```

## 📝 Key Files and Their Purposes

### Core Application Files

- `ServerMain.java`: Entry point for the server application
- `ClientMain.java`: Entry point for the client application
- `DatabaseManager.java`: Database connection and management
- `ThreadManager.java`: Handles concurrent user connections

### Configuration Files

- `database.properties`: Database connection settings
- `server.properties`: Server configuration settings
- `schema.sql`: Database schema definition

### Documentation

- `README.md`: Project overview and setup instructions
- `API.md`: API documentation
- `USER_GUIDE.md`: User manual

## 🔧 Build and Dependencies

### Required Libraries

- JDBC Driver (MySQL/SQLite)
- JUnit (for testing)
- Log4j (for logging)
- Bcrypt (for password hashing)

### Build Tools

- Maven for dependency management
- JAR packaging for distribution
