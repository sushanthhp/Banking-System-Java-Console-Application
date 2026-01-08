# Banking System – Java Console Application

A backend-focused **Banking System** built using **Core Java**, designed with clean architecture, proper exception handling, and file persistence.

This project demonstrates real-world banking operations such as account creation, deposits, withdrawals, transfers, and transaction history tracking.

---

## 🚀 Features

- Create bank accounts
- Deposit money
- Withdraw money with balance validation
- Transfer money between accounts (atomic operation)
- View account details
- View transaction history
- File persistence using Java Serialization
- Clean separation of concerns (Model, Service, Utility, Exceptions)

---

## 🛠️ Technologies Used

- Java (Core Java)
- Java Collections (`Map`, `List`)
- Java Serialization (`ObjectInputStream`, `ObjectOutputStream`)
- Custom Exception Handling
- IntelliJ IDEA

---

## 🧩 Project Structure

model → Domain entities (Account, Transaction, BankData)
service → Business logic (BankService)
exception → Custom exceptions
util → File persistence utilities
Main.java → CLI controller

yaml
Copy code

---

## 💾 Persistence

- Data is stored using **binary file persistence**
- Accounts and transactions are serialized into `bank-data.dat`
- Data is automatically loaded on application startup

---

## ▶️ How to Run

1. Clone the repository
2. Open in IntelliJ IDEA
3. Run `Main.java`
4. Use the menu to interact with the system

---

## 📌 Design Highlights

- Service layer does not perform input/output
- Exceptions are thrown from services and handled in `Main`
- Transactions are immutable
- Transfer operation is atomic (all-or-nothing)
- No database dependency (file-based persistence)

---

## 📈 Future Enhancements

- Convert to Spring Boot REST API
- Replace file persistence with database (MySQL)
- Add user authentication
- Add JUnit tests

---

## 👤 Author

Sushanth H P
B.Tech Graduate | Java Backend Developer
