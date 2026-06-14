# Credit Card Management System (CCMS)

## Overview

The Credit Card Management System (CCMS) is a Mainframe-based application developed using COBOL, JCL, VSAM, and CICS. The project simulates real-world credit card operations, including customer onboarding, card issuance, transaction processing, payment handling, balance maintenance, and statement generation.

The system demonstrates how credit card transactions are processed and managed within banking environments while maintaining accurate customer account information and financial records.

---

## Technologies Used

- COBOL
- JCL
- VSAM
- CICS

---

## Key Features

### Customer Management
- Customer registration and maintenance
- Customer profile management
- Account creation and management

### Card Management
- Credit card issuance
- PIN setup and maintenance
- Card activation and status management

### Card Number Generation
- Credit card numbers are generated using the **Luhn Algorithm** to ensure validity and compliance with industry standards.

### CVV Generation
- CVV is generated using:
  - PAN (Primary Account Number)
  - Expiry Date
  - Service Code

### Transaction Processing
The system supports:

- Purchase Transactions
- Cash Withdrawal Transactions
- EMI Transactions
- Payment Transactions

Each transaction undergoes validation and balance updates before being approved.

---

## Balance Management

The system continuously maintains:

- Outstanding Balance (OTB)
- Current Balance
- Available Credit Limit

Whenever a transaction is performed, balances are automatically updated to reflect the latest account status.

---

## Payment Allocation Logic

When a customer makes a payment, the amount is allocated according to business rules:

1. Interest Amount
2. Late Payment Fee
3. Principal Outstanding

### Example

Customer Payment = ₹1,000

Allocation:
- ₹500 → Interest
- ₹200 → Late Fee
- ₹300 → Principal

This ensures proper settlement of dues before reducing the principal balance.

---

## Billing and Statement Processing

The system performs:

- Interest Calculation
- Late Fee Assessment
- Outstanding Balance Calculation
- Monthly Statement Generation
- Payment Processing
- Balance Reconciliation

---

## Batch Processing

Batch jobs are executed using JCL for:

- Interest Processing
- Fee Processing
- Statement Generation
- Report Generation
- Balance Reconciliation
- Data Backup and Archival

---

## VSAM Data Files

The application stores data using VSAM files, including:

- Customer File
- Card File
- Account File
- Transaction File
- Parameter File

---

## Learning Outcomes

Through this project, I gained practical knowledge in:

- Mainframe Application Development
- COBOL Programming
- CICS Online Processing
- JCL Batch Processing
- VSAM File Management
- Credit Card Lifecycle Management
- Cards and Payments Domain
- Transaction Processing
- Billing and Statement Generation
- Balance Management
- Banking Business Rules and Workflows

---

## Project Workflow

1. Customer Registration
2. Card Issuance
3. Card Number Generation using Luhn Algorithm
4. CVV Generation
5. Transaction Processing
6. OTB and Current Balance Updates
7. Customer Payment Processing
8. Payment Allocation (Interest → Fee → Principal)
9. Interest and Fee Calculation
10. Statement Generation
11. Reporting and Reconciliation

---

## Author

**Sathvika Lingamolla**

Mainframe Developer | Cards & Payments
