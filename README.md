# 🏦 Banking System in Java (JDBC)

A beginner-friendly Java project that implements a **Banking System** using **JDBC** (Java Database Connectivity). This project demonstrates core concepts of **database interactions**, **object-oriented programming**, and **security features** like transaction PINs.

---

## ✨ Features

- 👤 **User Registration and Login**:  
  - Register with your full name, email, and password.  
  - Secure login to manage accounts.

- 💳 **Account Management**:  
  - 🏷️ Open new bank accounts.  
  - 📊 Check account balance.  
  - ➕ Credit money and ➖ Debit money.  
  - 🔄 Transfer money securely using a transaction PIN.

- 🔒 **Enhanced Security**:  
  - All transactions require a **4-digit security PIN** for added safety.

---

## 🗄️ Database Design

### 📂 Database: `BankingSystem`

#### 📋 Tables:
1. **`User` Table**:  
   Stores user information.  
   - `full_name` (VARCHAR)  
   - `email` (VARCHAR, UNIQUE)  
   - `password` (VARCHAR)  

2. **`Accounts` Table**:  
   Stores account details.  
   - `account_number` (INT, AUTO_INCREMENT)  
   - `full_name` (VARCHAR)  
   - `balance` (DECIMAL)  
   - `email` (VARCHAR, FOREIGN KEY)  
   - `security_pin` (CHAR)

---

## ⚙️ How It Works

1. **User Registration**:  
   - Users provide their name, email, and password.  
   - The system stores this data securely in the database.

2. **Login**:  
   - Authenticate using email and password.

3. **Account Operations**:  
   - Users can perform operations like creating accounts, checking balances, crediting/debiting money, and transferring funds.

4. **Transaction Security**:  
   - Every transaction is verified using a 4-digit security PIN.

---

## 🚀 Getting Started

### Prerequisites
- 🖥️ Java Development Kit (JDK)  
- 🛠️ MySQL Server  
- ✏️ IDE (e.g., IntelliJ IDEA, Eclipse)

### Installation

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-repo-link/banking-system-java
   ```

2. Set up the database using the provided SQL script:  
   - Import `database.sql` into your MySQL server.

3. Configure database credentials in the project file:  
   Update the `DBConnection` class with your MySQL username and password.

4. Run the project from your IDE.

---

## 📁 Folder Structure

- `src`  
  - `com.bankingsystem`  
    - `User.java`  
    - `Accounts.java`  
    - `AccountManager.java`  
    - `BankingApp.java`  
  - `DBConnection.java`  

---

## 🛡️ License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

