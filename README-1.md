# Banking Loans Management System

A command-line Python project that simulates basic loan management
workflows. It lets a user apply for a loan, make EMI payments, clear a
loan, and review payment history. Loan records are stored locally in a
JSON file.

> **Note:** This is an educational project, not a real banking or
> lending service. It does not connect to a bank or process real
> payments.

## Features

-   **Loan application:** Collects the applicant's name and salary, then
    checks the project's salary eligibility rule.
-   **Loan calculation:** Calculates a sample loan amount, EMI, and
    tenure using the rules defined in the program.
-   **EMI payment:** Records EMI payments and updates the outstanding
    balance and remaining tenure.
-   **Loan clearance:** Supports full clearance and eligible partial
    clearance.
-   **Payment history:** Displays recorded payments, remaining balance,
    loan status, and next EMI due date.
-   **Date validation:** Accepts dates in `DD-MM-YYYY` format.
-   **Local JSON storage:** Saves loan records in `loans.json` so data
    can be loaded again when the program runs.

## Tech Stack

-   Python
-   JSON for local data storage
-   Python standard-library modules: `os`, `datetime`, and `json`

## Project Structure

``` text
Banking-Loans/
├── bankingLoans.py   # Main application
├── loans.json        # Local loan-record storage
└── README.md         # Project documentation
```

## Requirements

-   Python **3.12 or newer** is recommended for the f-string syntax used
    in the current source.
-   Git is optional and only needed if you want to clone or contribute
    to the repository.

## Run Locally

1.  Clone the repository:

    ``` bash
    git clone https://github.com/vijayanimela/Banking-Loans.git
    ```

2.  Move into the project directory:

    ``` bash
    cd Banking-Loans
    ```

3.  Run the program:

    ``` bash
    python bankingLoans.py
    ```

    On some Windows installations, you may need:

    ``` bash
    py bankingLoans.py
    ```

## How to Use

When the program starts, it displays a menu:

1.  **Apply for Loan** --- enter the requested applicant details and
    follow the prompts.
2.  **Pay EMI** --- enter the loan ID and the EMI amount requested by
    the program.
3.  **Clear Loan** --- enter the loan ID and follow the prompts for full
    or partial clearance.
4.  **View Payment History** --- enter the loan ID to view payment
    records and current loan details.
5.  **Exit** --- close the program.

The program generates a loan ID for each saved loan. Keep that ID if you
want to make payments or view the history later.

## Data Storage

Loan information is stored in `loans.json` in the project folder. The
application reads this file at startup and writes updates when loan
records change.

**Important:** `loans.json` is local application data, not a secure
production database. Avoid adding real customer details or sensitive
financial information to this repository.

## Learning Outcomes

This project demonstrates:

-   Functions and modular program structure
-   Conditional logic and loops
-   Input validation and exception handling
-   Working with dates
-   Reading and writing JSON files
-   Basic record management and calculations

## Future Improvements

-   Add automated tests and stronger input validation.
-   Separate business logic from user-interface code.
-   Improve loan confirmation and error handling.
-   Add a database for persistent storage.
-   Add authentication and a graphical or web interface.
-   Review financial calculations and edge cases before any real-world
    use.

## Repository

[View Banking-Loans on
GitHub](https://github.com/vijayanimela/Banking-Loans)

------------------------------------------------------------------------

Created as a Python learning project by **Vijay Kumar**.
