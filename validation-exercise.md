# Python Homework: Movie Ticket Booking System

### Topic: Input Validation

Imagine you are creating a simple program for a cinema.

Your program should allow a customer to **book movie tickets**, but it must make sure that the information they enter is valid.

Your program must use all **four types of input validation** we have studied:

* Presence Check
* Range Check
* Lookup Check
* Length Check

---

## Your Program

The program should ask the customer for:

### 1. Customer Name

Ask:

```text
Enter your name:
```

The customer **must enter a name**.

Use a **Presence Check**.

---

### 2. Movie

Give the customer a list of movies to choose from.

For example:

```text
1. Minecraft
2. Inside Out 2
3. Spider-Man
4. How to Train Your Dragon
```

The customer should enter the **movie name**.

Use a **Lookup Check** to make sure they selected one of the available movies.

---

### 3. Number of Tickets

Ask the customer how many tickets they want.

The cinema allows a customer to purchase between **1 and 8 tickets**.

Use a **Range Check**.

---

### 4. Booking Code

Ask the customer to create a booking code.

The booking code must contain **exactly 6 characters**.

Use a **Length Check**.

---

## Ticket Price

Each ticket costs **$10**.

Your program should calculate the total cost.

For example:

```text
Number of tickets: 3
Ticket price: $10
Total: $30
```

---

## Final Booking

If all the information is valid, display a booking summary similar to:

```text
===== BOOKING CONFIRMED =====

Customer: Alex
Movie: Spider-Man
Tickets: 3
Booking Code: ABC123

Total Price: $30

Thank you for your booking!
```

If an input is invalid, your program should display a **clear error message**.

For example:

```text
How many tickets would you like? 15

Invalid number of tickets.
You can purchase between 1 and 8 tickets.
```

---

## ⭐ Challenge

Make your program **ask the customer again when they enter invalid information**.

For example:

```text
How many tickets would you like? 0

Invalid number of tickets.
Please enter a number between 1 and 8.

How many tickets would you like? 3
```

The program should only continue once valid information has been entered.

---

## Requirements

Your program must:

* Use `input()`.
* Use all **four types of validation**.
* Calculate the total ticket price.
* Display a final booking summary.
* Give useful error messages.
* Be written using your own code.

