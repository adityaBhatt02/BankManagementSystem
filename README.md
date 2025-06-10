**🏦 Bank Management System (Java Swing + MySQL)**
A full-featured desktop banking application built using Java Swing for GUI and MySQL for database storage. The application simulates real-world ATM functionalities including signup, login, deposit, withdrawal, balance enquiry, PIN change, and fast cash.

**📌 Features**
🔐 User Authentication: Login with secure PIN
🧾 Account Registration: Multi-step signup (3 stages)
💸 Deposit / Withdraw: Input amount, real-time DB updates
💳 Fast Cash: Quick preset withdrawals
💱 Balance Enquiry: View current account balance
🔄 Change PIN: Securely update account PIN
🚪 Exit: Logout with confirmation

**🛠️ Tech Stack**
•Language: Java
•GUI: Java Swing
•Database: MySQL
•Connectivity: JDBC
•Modules Required:
   ->jcalendar-1.3.3.4.jar
   ->mysql-connector-java-8.0.xx.jar (MySQL JDBC driver)


**⚙️ Database Setup**
1)Open MySQL CLI or Workbench

2)Create the database and tables:

CREATE DATABASE bankmanagementsystem;
USE bankmanagementsystem;

-- Sample table; actual schema may vary based on your code
CREATE TABLE login (
  cardnumber VARCHAR(20) PRIMARY KEY,
  pin VARCHAR(10)
);
-- Additional tables: signup, bank, transactions, etc.

3)In Connn.java, ensure your credentials are correct:
Connection c = DriverManager.getConnection("jdbc:mysql://localhost:3306/bankmanagementsystem", "root", "your_password");

**Running the App**
1)Clone the repo:
git clone https://github.com/adityaBhatt02/BankManagementSystem.git

2)Open in your IDE and configure:
   •Add required JARs to the classpath
   •Set up MySQL as per the above instructions

3)Run the Login.java class (or any appropriate launcher class).
