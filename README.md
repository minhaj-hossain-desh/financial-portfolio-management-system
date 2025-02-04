# 💼 Financial Portfolio Management System  

This project is a **Financial Portfolio Management System**, developed as part of an **Object-Oriented Programming (OOP) course group project**.  
It allows users to **manage, buy, sell, and track financial assets**, providing insights into portfolio performance over time.

---

## 🚀 Features
- 📊 **Asset Management** → Users can **add, buy, sell, and track** various assets.  
- 💰 **Supported Asset Types** → Includes **Stocks, Bonds, Government Bonds, and Cryptocurrencies**.  
- 📉 **Portfolio Tracking** → Displays **total portfolio value, profit/loss, and transaction history**.  
- 🔄 **Data Persistence** → Saves portfolio and transactions to files for future reference.  
- 🔍 **Historical Price Integration** → Uses `historical_prices.txt` to analyze price trends.  
- 📂 **User Management** → Supports **multiple users**, storing details in `users.txt`.  

---

## 🏗️ **OOP Concepts Used**
This project heavily utilizes **Object-Oriented Programming (OOP)** principles:

- **Encapsulation** → Asset-related data is protected within classes (`Stock`, `Bond`, `Cryptocurrency`), ensuring controlled access.
- **Inheritance** → `Asset` serves as a base class, with `Stock`, `Bond`, `GovernmentBond`, and `Cryptocurrency` inheriting from it.
- **Polymorphism** → Overriding functions like `calculateValue()` allow each asset type to behave uniquely.
- **Abstraction** → The `Asset` class provides a blueprint for financial instruments.

---

## 📂 **Files and Their Purpose**
- `Asset.h / Asset.cpp` → Defines the base `Asset` class and core financial asset properties.
- `Stock.h / Stock.cpp` → Implements the `Stock` asset, inheriting from `Asset`.
- `Bond.h / Bond.cpp` → Implements the `Bond` asset, inheriting from `Asset`.
- `GovernmentBond.h / GovernmentBond.cpp` → Extends `Bond` with additional government-specific features.
- `Cryptocurrency.h / Cryptocurrency.cpp` → Implements `Cryptocurrency`, inheriting from `Asset`.
- `PortfolioManager.h / PortfolioManager.cpp` → Handles **buying, selling, and tracking assets**.
- `FileManager.h / FileManager.cpp` → Manages **saving and loading portfolio/transaction data**.
- `Transaction.h / Transaction.cpp` → Stores **buy/sell transaction details**.
- `TransactionLog.h / TransactionLog.cpp` → Logs **all asset transactions**.
- `User.h / User.cpp` → Manages **user authentication and account handling**.
- `debug.h / debug.cpp` → Provides **debugging utilities**.
- `main.cpp` → **Entry point of the application**, bringing all components together.
- `Makefile` → Compiles the project using `make`.
- `users.txt` → Stores **registered user data**.
- `historical_prices.txt` → Provides **historical price data** for asset valuation.
- `test_portfolio.txt / test_transactions.txt` → Contains sample **test cases** for debugging.
- `AssetTest.cpp, StockTest.cpp, BondTest.cpp, PortfolioManagerTest.cpp, etc.` → **Unit tests** for individual components.

---

