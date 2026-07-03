# 🏦 Falaknama Banking System


---

# 📖 Overview

**Falaknama Banking System** is a **Console-Based Banking Application** developed using **Core Java**, **Object-Oriented Programming (OOP)** principles, and **Maven**.

The application simulates the core functionality of a real banking system by allowing users to create accounts, deposit money, withdraw funds, transfer money, and check balances through an interactive menu-driven console interface.

This project is designed for students and beginner Java developers to understand how real-world banking applications are structured while strengthening their knowledge of Java programming fundamentals.

---

# ✨ Features

## 👤 Dynamic Account Creation

Users can create multiple bank accounts during runtime by entering account details. Every account is stored dynamically, allowing the system to grow without predefined limits.

---

## 📋 Display All Accounts

Displays all registered customer accounts along with important information such as:

* Account Number
* Account Holder Name
* Mobile Number
* Current Balance

This feature helps administrators quickly view all customers.

---

## 💰 Check Account Balance

Users can enter an account number to instantly retrieve the available account balance.

---

## 💵 Deposit Money

Allows users to securely deposit money into an existing account.

Features include:

* Account verification
* Amount validation
* Updated balance calculation
* Transaction confirmation

---

## 💸 Withdraw Money

Customers can withdraw money after successful validation.

The system checks:

* Account existence
* Sufficient balance
* Valid withdrawal amount

This prevents invalid transactions.

---

## 🔄 Transfer Money

Transfers money from one account to another safely.

Validation includes:

* Sender verification
* Receiver verification
* Available balance
* Transaction completion

Balances are updated automatically.

---

## 🆔 UTR ID Generation

Every successful transfer generates a unique **UTR (Unique Transaction Reference)** ID for tracking purposes.

Example:

```
UTR20260703124589012
```

---

## 🧾 Transaction Receipt

After every successful transaction, the system prints a detailed receipt including:

* Transaction Type
* Sender
* Receiver
* Amount
* Date & Time
* UTR Number
* Updated Balance

---

## 🚫 Duplicate Account Validation

The application prevents duplicate account creation by checking unique account numbers before registration.

---

## ✅ Account Verification

Before performing any banking operation, the system verifies whether the entered account exists.

---

## ⚖️ Balance Validation

The system ensures that withdrawals and transfers cannot exceed the available account balance.

---

## 🖥️ Menu-Driven Console Application

A simple interactive menu makes navigation easy.

```
=========== Falaknama Banking System ===========

1. Create Account
2. Display All Accounts
3. Deposit Money
4. Withdraw Money
5. Transfer Money
6. Check Balance
7. Exit

===============================================
```

---

# ☕ Java Concepts Used

| Concept                | Description                                                       |
| ---------------------- | ----------------------------------------------------------------- |
| Classes                | Represents entities such as Account, Bank, and Transaction.       |
| Objects                | Used to create real bank account instances.                       |
| Constructors           | Initialize objects with default or custom values.                 |
| Encapsulation          | Protects account data using private variables and public methods. |
| OOP                    | Organizes the application into reusable classes.                  |
| ArrayList              | Stores customer accounts dynamically.                             |
| Scanner                | Reads user input from the console.                                |
| Methods                | Divides functionality into reusable operations.                   |
| Loops                  | Keeps the application running until the user exits.               |
| Switch Case            | Controls menu navigation.                                         |
| Conditional Statements | Validates transactions and account information.                   |
| Constructor Injection  | Passes required objects through constructors.                     |
| Method Calling         | Promotes modular and reusable code.                               |
| LocalDateTime          | Captures transaction timestamps.                                  |
| DateTimeFormatter      | Formats date and time into readable output.                       |

---

# 📂 Project Structure

```text
Falaknama_Banking_System
│
├── pom.xml
├── README.md
├── .gitignore
│
└── src
    └── main
        └── java
            └── com
                └── falaknama
                    ├── Account.java
                    ├── Bank.java
                    ├── Transaction.java
                    └── Main.java
```

---

# 📁 Java File Responsibilities

## 📄 Account.java

Responsible for representing an individual bank account.

Responsibilities:

* Store account information
* Maintain account balance
* Provide getters and setters
* Support deposits and withdrawals
* Encapsulate customer data

---

## 📄 Bank.java

Acts as the service layer of the application.

Responsibilities:

* Create accounts
* Search accounts
* Deposit money
* Withdraw money
* Transfer funds
* Display all accounts
* Validate users
* Manage ArrayList of accounts

---

## 📄 Transaction.java

Responsible for transaction-related operations.

Responsibilities:

* Generate UTR IDs
* Print receipts
* Record timestamps
* Format transaction details

---

## 📄 Main.java

Application entry point.

Responsibilities:

* Display menu
* Read user input
* Call banking methods
* Control application flow
* Handle program execution

---

# 💻 Sample Console Output

## Create Account

```text
========== Create Account ==========

Enter Account Number : 1001
Enter Name           : Nandu
Enter Mobile Number  : 9876543210
Enter Initial Deposit: 5000

------------------------------------
Account Created Successfully!
------------------------------------
```

---

## Display Accounts

```text
--------------- Account Details ---------------

Account Number : 1001
Name           : Nandu
Mobile         : 9876543210
Balance        : ₹5000.00

-----------------------------------------------
```

---

## Deposit Money

```text
Enter Account Number : 1001
Enter Deposit Amount : 2000

Deposit Successful!

Updated Balance : ₹7000.00
```

---

## Withdraw Money

```text
Enter Account Number : 1001
Enter Withdrawal Amount : 1000

Withdrawal Successful!

Remaining Balance : ₹6000.00
```

---

## Transfer Money

```text
From Account : 1001
To Account   : 1002
Amount        : 1500

Transfer Successful!
```

---

## Transaction Receipt

```text
====================================

Transaction Receipt

====================================

Transaction Type : Transfer

Sender           : 1001

Receiver         : 1002

Amount           : ₹1500.00

UTR ID           : UTR20260703124589012

Date             : 03-07-2026

Time             : 12:45 PM

Status           : SUCCESS

====================================
```

---

## Check Balance

```text
Enter Account Number : 1001

Available Balance

₹6000.00
```

---

# ⚙️ Installation Guide

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/Falaknama_Banking_System.git
```

---

## 2️⃣ Open in IntelliJ IDEA

* Launch IntelliJ IDEA
* Select **Open**
* Choose the cloned project folder
* Wait for Maven dependencies to load

---

## 3️⃣ Build Using Maven

```bash
mvn clean install
```

---

## 4️⃣ Run the Application

Execute:

```text
Main.java
```

The console-based banking menu will start automatically.

---

# 🛠 Technologies Used

| Technology    | Purpose                                 |
| ------------- | --------------------------------------- |
| Java 17       | Core application development            |
| Maven         | Dependency management and project build |
| IntelliJ IDEA | Integrated Development Environment      |
| Git           | Version control                         |
| GitHub        | Source code hosting and collaboration   |

---

# 🎯 Learning Outcomes

After completing this project, a beginner will understand:

* Core Java programming
* Object-Oriented Programming concepts
* Class and object design
* Constructors and method creation
* Encapsulation and data hiding
* Collections using ArrayList
* Exception-free input validation
* Menu-driven console applications
* Banking workflow implementation
* Dynamic data management
* Transaction processing
* Code modularization
* Java date and time API
* Maven project structure
* Clean coding practices
* Professional project organization
* Git and GitHub workflow fundamentals

---

# 🚀 Future Enhancements

The project can be enhanced with the following features:

* 🔐 User Login Authentication
* 🔑 PIN Verification
* 📜 Transaction History
* 📄 Mini Statement Generation
* 💹 Interest Calculation
* 💾 File Handling for Data Persistence
* 🗄 Database Integration
* 🐬 MySQL Support
* 🔌 JDBC Connectivity
* 🌐 Spring Boot REST API
* 🖥 JavaFX Desktop GUI
* 📱 Online Banking Features
* 📧 Email Notifications
* 📲 SMS Alerts
* 🔔 Real-Time Transaction Notifications
* ☁ Cloud Deployment
* 📊 Admin Dashboard
* 📈 Monthly Account Reports

---

# 🌟 Project Highlights

✅ Clean Object-Oriented Design

✅ Menu-Driven Architecture

✅ Modular Code Structure

✅ Dynamic Account Management

✅ Secure Transaction Validation

✅ Professional Console Output

✅ Unique Transaction Tracking

✅ Beginner-Friendly Implementation

✅ Easy to Extend

---

# 🤝 Contributing

Contributions are welcome!

If you would like to improve the project:

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request describing your improvements.

---

# 📜 License

This project is open-source and may be used for learning, educational, and personal development purposes.

---

# 👨‍💻 Author

**Nandu**

Java Developer | Core Java Enthusiast | Object-Oriented Programming Learner

---

<p align="center">

⭐ If you found this project helpful, consider giving it a **Star** on GitHub!

**Happy Coding! 🚀**

</p>
