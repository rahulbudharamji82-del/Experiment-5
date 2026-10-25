Student CRUD Application
📌 Aim
To develop a Java console-based application to perform basic CRUD (Create, Read, Update, Delete) operations on a student database using JDBC and MySQL.

📝 Description
This project is a student management system designed to handle student records securely and efficiently. The application connects to a MySQL database using the MySQL Connector/J driver. It features a modular architecture where the Main class handles the core loop and user choices, while dedicated classes like UpdateData handle specific database operations using parameterized queries.

✨ Features
Interactive console-based menu for navigating database operations.

Secure record updates using JDBC PreparedStatement to prevent SQL injection.

Automated driver validation and connection checking upon startup.

Modular structure separating application flow logic from record-handling operations.

🛠️ Technologies Used
Java — Core programming language
JDBC (Java Database Connectivity) — Database communication API
MySQL & MySQL Connector/J — Database and driver components
📂 Project Structure
student-crud-app/
├── Main.java               # Application entry point and menu controller
├── UpdateData.java         # Handles record modification logic
├── DatabaseConnection.java # Manages database connection and driver loading
├── META-INF/               # Connector metadata
└── com/mysql/cj/           # MySQL JDBC driver classes

⚙️ Installation and Setup
Prerequisites
Java Development Kit (JDK) installed.
MySQL Server running locally or remotely.
MySQL JDBC Driver (mysql-connector-j) included in the project configuration.
Step 1: Clone the repository
git clone YOUR_GITHUB_REPOSITORY_URL
Replace YOUR_GITHUB_REPOSITORY_URL with your GitHub repository URL.

Step 2: Navigate to the project folder
cd student-crud-app
Step 3: Compile the application
javac Main.java UpdateData.java
Step 4: Run the application
java Main
The console will display an interactive text menu (1. Insert, 2. Update, 3. Delete, 4. Display, 5. Exit).

🔄 How It Works
The application starts and Main.java validates the MySQL driver via DatabaseConnection.loadDriver().

A continuous while (true) loop presents a console text menu to the user.

Based on the user's input, the application switches execution to the respective utility handler (e.g., UpdateData for updates).

UpdateData prompts the user for a Student ID and new details, executing a secure SQL update statement.

🎯 Learning Outcomes
Understand how to connect Java applications to MySQL databases using JDBC.

Learn how to implement secure database queries using PreparedStatement.

Structure console-based applications using modular Java classes.

Handle external dependencies and database drivers.

🔮 Future Improvements
Add a graphical user interface (GUI) or web interface.
Implement comprehensive error handling and input validation for all CRUD fields.
Add support for connection pooling to improve database performance.
Write automated unit tests for data operations.
