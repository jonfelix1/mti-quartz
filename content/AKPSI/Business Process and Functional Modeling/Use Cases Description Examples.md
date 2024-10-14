---
tags:
- akpsi
- topic
- note
Class: "[[Information System Analysis and Design Class (AKPSI)]]"
Topic: "[[Business Process and Functional Modeling]]"
---

# Use Cases Description Examples

---

## Use Case 1: Borrow Book
- **Name**: Borrow Book
- **ID Number**: UC-001
- **Type**: Essential
- **Primary Actor**: Library Member
- **Brief Description**: The user borrows a book from the library.
- **Importance Level**: High
- **Stakeholders**:
  - **Library Member**: Wants to borrow books.
  - **Librarian**: Manages the borrowing process.
  - **Library System**: Updates book borrowing records.
- **Trigger(s)**: The user selects a book to borrow from the system.

### Relationships:
- **Association**: Communication between the library member and the librarian.
- **Include**: Search Book, Update Borrow Records.

### Flow of Events:

**Normal Flow**:
1. The Library Member searches for a book.
2. The Library Member selects a book to borrow.
3. The Librarian approves the borrow request.
4. The Library System updates the borrowing record.

**Sub-flows**:
- If the Library Member does not find the desired book, they may repeat the search process.

**Alternate Flows**:
- If the Librarian rejects the borrow request due to a pending fine, the process is terminated.

---

## Use Case 2: Register User
- **Name**: Register User
- **ID Number**: UC-002
- **Type**: Real
- **Primary Actor**: Library Member
- **Brief Description**: A user registers for a library account.
- **Importance Level**: Medium
- **Stakeholders**:
  - **Library Member**: Wants to create an account to use the library system.
  - **Library System**: Verifies and stores user information.
- **Trigger(s)**: The user attempts to register for the library system.

### Relationships:
- **Association**: Communication between the library member and the system.
- **Extend**: User Login, Confirm Registration.

### Flow of Events:

**Normal Flow**:
1. The Library Member enters personal information (name, email, etc.).
2. The Library System verifies the information.
3. The Library Member confirms the registration details.
4. The system stores the user’s information and creates an account.

**Sub-flows**:
- The Library System sends a confirmation email to verify the email address.

**Alternate Flows**:
- If the email address is invalid, the system prompts the user to enter a valid email.

---

## Use Case 3: Process Payment
- **Name**: Process Payment
- **ID Number**: UC-003
- **Type**: Essential
- **Primary Actor**: Library Member
- **Brief Description**: The user makes a payment for overdue books.
- **Importance Level**: High
- **Stakeholders**:
  - **Library Member**: Wants to clear overdue payments.
  - **Library System**: Processes the payment.
- **Trigger(s)**: The user attempts to borrow a book but is prompted to pay an overdue fee.

### Relationships:
- **Include**: Calculate Overdue Amount, Update Payment Record.

### Flow of Events:

**Normal Flow**:
1. The Library System displays the overdue amount.
2. The Library Member selects the payment method.
3. The Library System processes the payment.
4. The payment record is updated, and the overdue status is cleared.

**Sub-flows**:
- The system may offer different payment options such as credit card, debit card, or online banking.

**Alternate Flows**:
- If the payment is declined, the system prompts the user to select another payment method.

