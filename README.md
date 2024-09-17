# Bank Management System

This project is a simple **Bank Management System** implemented in C. The system allows users to create accounts, delete accounts, deposit and withdraw money, transfer funds between accounts, and view their transaction history. It also stores account information and keeps track of transactions for each account.

## Features

- **Create Account**: Register a new account with personal details.
- **Delete Account**: Remove an existing account.
- **Deposit Money**: Add money to an account.
- **Withdraw Money**: Withdraw funds from an account with password verification.
- **View Account**: Display account information.
- **Transfer Money**: Transfer money between two bank accounts.
- **View Transactions**: Show the transaction history for a specific account.

## Data Structures

The system uses the following two main structures:
- **Account**: Holds details like name, age, address, phone number, email, account number, customer ID, password, and balance.
- **Transaction**: Records each transaction with details such as the account number, transaction type (deposit, withdrawal, transfer), amount, and date.

## Files

- **Main Source Code**: `bank_management_system.c`
- **Account Structure**: 
  ```c
typedef struct
  {
      char name[50];
      int age;
      char address[100];
      char phoneNumber[15];
      char email[50];
      int accountNumber;
      int customerID;
      int password;
      float balance;
  } account;

# Transaction Structure
typedef struct
{
    int accountNumber;
    char type[20];
    float amount;
    char date[20];
} transaction;

# Functionality
1. createAccount()
Creates a new account and assigns a unique account number and customer ID to the user.

2. deleteAccount()
Removes an account from the system by account number and user name.

3. depositMoney()
Deposits an amount to the user’s account.

4. withdrawMoney()
Withdraws a specified amount from the user's account, provided the account has sufficient balance.

5. viewAccount()
Displays account details like account number, customer ID, name, age, address, phone number, email, and balance.

6. transferMoneyToBankAccount()
Transfers money between two accounts after password verification.

7. viewTransactions()
Shows the transaction history for a specific account.

# How to Run the Program
# Clone the repository: 
git clone https://github.com/your-username/bank-management-system.git

# Compile the code: Use the following command to compile the C program:
gcc bank_management_system.c -o bank_management_system

# Run the program: Run the compiled binary to start the Bank Management System:
./bank_management_system

# Navigate the Menu: 
The program will present a menu where you can select actions like creating accounts, depositing money, viewing transactions, etc.

# Example
Here is an example interaction with the program: 
Bank Management System
1. Create Account
2. Delete Account
3. Deposit Money
4. Withdraw Money
5. View Account
6. Transfer Money
7. View Transactions
8. Exit
Enter your choice: 1

Your name: John Doe
Your age: 30
Your address: 123 Main St
Your phone number: 5551234567
Your email: john@example.com
Your password: 1234
Account created successfully!
Account Number: 123456789
Customer ID: 7654321

# Future Improvements
Save account and transaction data to files to persist between program runs.
Add encryption for passwords.
Implement interest calculation for savings accounts.

# License
This project is licensed under the MIT License. Feel free to use and modify it as per your needs.
Feel free to replace any placeholders with actual information, and modify the README to suit your project’s needs!







