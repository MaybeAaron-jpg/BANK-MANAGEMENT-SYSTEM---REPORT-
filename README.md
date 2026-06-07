# BANK-MANAGEMENT-SYSTEM---REPORT-
Bank Account Management System

> A console-based C++ application implementing core banking operations using  
> Object-Oriented Design and a sorted singly linked list data structure.

**Course:** 21CSC101T — Object Oriented Design Programming  
**Institution:** SRM Institute of Science and Technology, Ramapuram  
**Academic Year:** 2025–26 (Even Semester)  
**Guide:** Dr. J. Cypto, Assistant Professor, Dept. of CSE (BDA & CC)

**Team:**
- Aditya Shibu — RA2511027020171
- Aaron Sudhir — RA2511027020179
- P. Akash — RA2511027020143
- 
#Overview

The **Bank Account Management System** is a menu-driven C++ console application that simulates essential banking operations. It addresses the inefficiencies of manual account management — such as data entry errors, duplicate records, uncontrolled withdrawals, and lack of sorted record display — by implementing a structured software solution with proper validation at every step.

All account records are stored in-memory using a **sorted singly linked list**, ordered by account number, enabling efficient insertion, search, and deletion. A mandatory minimum balance of **Rs. 500** is enforced across all accounts to mirror real-world banking constraints.


#Objectives

- Enable creation of Savings or Current bank accounts with a unique account number and a minimum opening deposit of Rs. 500
- Allow deposits and withdrawals with real-time balance updates and validation
- Enforce a minimum balance constraint to prevent overdraft
- Support balance inquiry with complete account detail display
- Implement secure account deletion (node removal from linked list)
- Display all existing accounts in sorted tabular format for administrative reference
- Prevent duplicate account numbers through a uniqueness check before insertion

#Problem Statement

Traditional manual banking systems suffer from:
- Data entry errors and duplicate account records
- No minimum balance enforcement, allowing accounts to go negative
- Slow and inefficient record searches across large datasets
- Unvalidated account deletion risking accidental data loss
- No structured way to display accounts in sorted order

This system resolves all of the above through CRUD operations on a sorted linked list with proper input validation.


#Features

| Feature | Description |
| Create Account | Register a new account with name, type, and initial deposit (min Rs. 500) |
| Deposit | Add funds to an existing account; balance updated instantly |
| Withdraw | Deduct funds with minimum balance (Rs. 500) enforcement |
| Balance Inquiry | View full account details — number, name, type, and balance |
| Delete Account | Remove an account from the linked list (simulate account closure) |
| View All Accounts | Display all accounts in sorted tabular format by account number |
| Duplicate Check | Prevents creation of two accounts with the same account number |
| Input Validation | Handles invalid menu choices, negative amounts, and non-numeric input |


#Key OOP & DSA Concepts Used

| Concept | Application in Project |
| Class & Object | `Node` class models each bank account as an object |
| Encapsulation | Data fields (`accNo`, `name`, `balance`) bundled within `Node` |
| Modular Design | Separate function for each operation (Create, Deposit, Withdraw, etc.) |
| Sorted Linked List | Accounts maintained in ascending order by account number |
| Dynamic Memory | `new Node()` for allocation, `delete` for deallocation |
| CRUD Operations | Create → Insert, Read → Search/Show, Update → Deposit/Withdraw, Delete → Remove node |
| Input Validation | Minimum balance check, duplicate account check, non-numeric input handling |

---

#Project Structure

#How to Run

#Prerequisites
- A C++ compiler (g++ recommended)
- Terminal / Command Prompt

#Steps

```bash
# Clone the repository
git clone https://github.com/your-username/bank-management-system.git

# Navigate into the directory
cd bank-management-system

# Compile the program
g++ -o bank main.cpp

# Run the program
./bank
```

> On Windows, use `bank.exe` instead of `./bank`
