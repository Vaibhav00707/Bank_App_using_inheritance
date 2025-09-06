Enhanced Banking Application
A comprehensive Java-based banking application that demonstrates object-oriented programming principles, including inheritance, polymorphism, and file handling.

Features
Account Management: Create savings or checking accounts with unique account numbers

Transaction Processing: Deposit, withdraw, and transfer funds between accounts

Security: 4-digit PIN authentication with account locking after multiple failed attempts

Transaction History: View complete transaction records with timestamps

Interest Calculation: Calculate interest based on account type and time period

Data Persistence: Automatic saving and loading of account data

Admin Functions: Special admin PIN (9999) for account unlocking and interest rate changes

Theme Support: Multiple UI themes (Classic, Dark, Light, Professional)

Inheritance Implementation: Proper OOP design with BankAccount as base class and specialized account types

Account Types
Savings Account
Higher interest rate (2.5%)

Annual bonus feature (1% of balance)

Standard withdrawal limits

Checking Account
Lower interest rate (1.5%)

Overdraft protection (default $500 limit)

Customizable overdraft limits (admin only)

Class Structure
text
BankApp (Main class)
│
├── BankAccount (Abstract base class)
│   ├── SavingsAccount (Concrete subclass)
│   └── CheckingAccount (Concrete subclass)
Technologies Used
Java Programming Language

Object Serialization for data persistence

Java Time API for transaction timestamps

Java Collections Framework for data management

How to Run
Compile the application:

bash
javac *.java
Run the application:

bash
java BankApp
Follow the on-screen menu to:

Create a new account

Login to an existing account

Perform banking operations

Usage Instructions
Creating an Account:

Select option 2 from the main menu

Provide your full name

Choose account type (Savings or Checking)

Set a 4-digit PIN

Make an initial deposit

Note your account number for future logins

Logging In:

Select option 1 from the main menu

Enter your account number and PIN

After 3 failed attempts, account will be locked

Use admin PIN (9999) to unlock locked accounts

Banking Operations:

Deposit funds (option 1)

Withdraw funds (option 2)

Transfer to other accounts (option 3)

Check balance (option 4)

View transaction history (option 5)

Calculate interest (option 6)

Change theme (option 7)

Switch accounts (option 8)

Access account settings (option 9)

Use account-specific features (option 10)

Admin Functions
Admin PIN: 9999

Unlock locked accounts

Change interest rates

Modify checking account overdraft limits

Data Storage
Account data is automatically saved to bank_data.dat when:

Creating a new account

Making transactions

Changing account settings

Exiting the application

Data is automatically loaded from this file when the application starts.

Inheritance Implementation
The application demonstrates proper use of inheritance:

BankAccount is an abstract base class containing:

Common fields (account holder name, account number, balance, etc.)

Common methods (deposit, withdraw, transfer, etc.)

Abstract method (getAccountType())

SavingsAccount extends BankAccount with:

Higher interest rate

Annual bonus feature

CheckingAccount extends BankAccount with:

Overdraft protection

Customizable overdraft limits

Notes
All monetary values are represented in dollars

Transaction history includes timestamps for all operations

The application handles edge cases like insufficient funds and invalid inputs

Data is preserved between application sessions through serialization

Future Enhancements
Potential improvements for future versions:

Database integration instead of file storage

Network connectivity for remote access

Web or mobile interface

Enhanced security features

Support for additional account types

Currency support beyond dollars

Interest compounding calculations

License
This project is for educational purposes to demonstrate Java OOP concepts and inheritance implementation.
