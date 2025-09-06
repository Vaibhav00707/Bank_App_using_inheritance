# 💳 Enhanced Banking Application

A comprehensive **Java-based banking application** that demonstrates key **object-oriented programming (OOP) principles**, including **inheritance, polymorphism, and file handling**.

---

## ✨ Features

- **Account Management**: Create savings or checking accounts with unique account numbers.  
- **Transaction Processing**: Deposit, withdraw, and transfer funds between accounts.  
- **Security**: 4-digit PIN authentication with account locking after multiple failed attempts.  
- **Transaction History**: Complete transaction records with timestamps.  
- **Interest Calculation**: Interest applied based on account type and time period.  
- **Data Persistence**: Automatic saving/loading of account data using serialization.  
- **Admin Functions**: Unlock accounts, adjust rates, manage overdraft limits via admin PIN (`9999`).  
- **Theme Support**: Multiple UI themes (Classic, Dark, Light, Professional).  
- **Inheritance Implementation**: OOP design with `BankAccount` as base class and specialized account types.  

---

## 🏦 Account Types

### 🔹 Savings Account
- Higher interest rate (**2.5%**)  
- Annual bonus (**1% of balance**)  
- Standard withdrawal limits  

### 🔹 Checking Account
- Lower interest rate (**1.5%**)  
- Overdraft protection (default **$500**)  
- Customizable overdraft limits (**admin only**)  

---

## 🛠 Class Structure

BankApp (Main class)
│
├── BankAccount (Abstract base class)
│ ├── SavingsAccount (Concrete subclass)
│ └── CheckingAccount (Concrete subclass)


---

## 🧑‍💻 Technologies Used

- **Java Programming Language**  
- **Object Serialization** (for data persistence)  
- **Java Time API** (for timestamps)  
- **Java Collections Framework** (for data management)  

---

## 🚀 How to Run

1. **Compile the application**:
   ```bash
   javac *.java
Run the application:

java BankApp


Follow the on-screen menu to:

Create an account

Login to an existing account

Perform banking operations

📋 Usage Instructions
🔑 Creating an Account

Select option 2 from the main menu

Enter your full name

Choose account type (Savings/Checking)

Set a 4-digit PIN

Make an initial deposit

Note your account number for future logins

🔑 Logging In

Select option 1 from the main menu

Enter account number & PIN

After 3 failed attempts, the account locks

Use admin PIN (9999) to unlock

💵 Banking Operations

Deposit funds (1)

Withdraw funds (2)

Transfer funds (3)

Check balance (4)

View transaction history (5)

Calculate interest (6)

Change theme (7)

Switch accounts (8)

Account settings (9)

Account-specific features (10)

👨‍💼 Admin Functions

Admin PIN: 9999

Unlock locked accounts

Change interest rates

Modify overdraft limits

💾 Data Storage

Account data is saved to bank_data.dat when:

Creating accounts

Performing transactions

Changing account settings

Exiting the app

Data automatically loads at application startup.

🧩 Inheritance Implementation

BankAccount (abstract)

Fields: account holder, number, balance, etc.

Methods: deposit, withdraw, transfer, etc.

Abstract: getAccountType()

SavingsAccount

Higher interest rate

Annual bonus feature

CheckingAccount

Overdraft protection

Custom overdraft limits

📌 Notes

Monetary values represented in USD ($)

Transactions include timestamps

Handles edge cases (invalid input, insufficient funds)

Data persists between sessions via serialization

🔮 Future Enhancements

Database integration (replace file storage)

Network connectivity for remote banking

Web or mobile interface

Advanced security features

Support for multiple currencies

Compound interest calculations

Additional account types

📜 License

This project is developed for educational purposes to demonstrate Java OOP concepts and inheritance implementation.

