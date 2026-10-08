### 1. Movie Ticket Calculator — Selection

**Concepts:** `if / elif / else`, input, arithmetic

Create a program that asks for:

* Age
* Whether the person is a student (`yes/no`)

Ticket prices:

* Under 12 → Rp20,000
* 12–17 → Rp30,000
* 18+ → Rp40,000
* Students receive a Rp5,000 discount.

The program should display the final ticket price.

**Challenge:** Make sure invalid ages and invalid student answers are handled.

---

### 2. Number Guessing Game — Indefinite Iteration

**Concepts:** `while`, selection, comparison

Create a guessing game where the secret number is `37`.

The user keeps entering guesses until they get the correct answer.

After every guess, display:

* `"Too high!"`
* `"Too low!"`
* `"Correct!"`

**Challenge:** Count how many attempts the user needed.

---

### 3. Multiplication Table Generator — Definite Iteration

**Concepts:** `for`, `range()`

Ask the user for a number and print its multiplication table from 1 to 12.

Example:

```text
Enter a number: 7

7 x 1 = 7
7 x 2 = 14
...
7 x 12 = 84
```

**Challenge:** Allow the user to choose the starting and ending multiplier.

---

### 4. ATM Menu — Indefinite Iteration + Selection

**Concepts:** `while`, `if/elif/else`

Create a simple ATM program.

Starting balance:

```text
Rp500,000
```

Repeatedly show:

```text
1. Check Balance
2. Deposit
3. Withdraw
4. Exit
```

The user can continue using the ATM until they choose Exit.

Rules:

* Cannot withdraw more than the balance.
* Deposit amount must be positive.
* Withdrawal amount must be positive.

**Challenge:** Keep track of the number of transactions.

---

### 5. FizzBuzz — Selection + Definite Iteration

**Concepts:** `for`, `if/elif/else`, modulo `%`

Print numbers from 1 to 100.

* Multiples of 3 → `"Fizz"`
* Multiples of 5 → `"Buzz"`
* Multiples of both → `"FizzBuzz"`
* Otherwise → print the number.

Example:

```text
1
2
Fizz
4
Buzz
Fizz
7
...
```

**Challenge:** Change the program so the user chooses the two numbers.

---

## 6. Password Checker — Indefinite Iteration + Selection

**Concepts:** `while`, conditions, strings

Create a program that repeatedly asks the user to enter a password.

The password must:

* Be at least 8 characters
* Contain at least one number
* Contain at least one uppercase letter

Keep asking until the password satisfies all requirements.

Example:

```text
Enter password: hello
Password is too short.

Enter password: helloworld
Password needs a number.

Enter password: Hello123
Password accepted!
```

**Challenge:** Give a separate message explaining which requirement is missing.

---

## 7. Rectangle Pattern — Nested Loops

**Concepts:** nested `for` loops

Ask the user for the number of rows and columns, then print a rectangle of `*`.

Example:

```text
Rows: 4
Columns: 6

******
******
******
******
```

**Challenge:** Let the user choose the character:

```text
Character: #

######
######
######
######
```

---

## 8. Number Triangle — Nested Loops

**Concepts:** nested loops, `range()`

Ask the user for a number and print:

```text
1
12
123
1234
12345
```

For example, if the user enters `5`.

**Challenge:** Make it print:

```text
1
22
333
4444
55555
```

---

## 9. Multiplication Table Grid — Nested Loops

**Concepts:** nested `for` loops

Ask the user for a number `n` and produce a multiplication table from `1 × 1` to `n × n`.

For `n = 5`:

```text
1  2  3  4  5
2  4  6  8 10
3  6  9 12 15
4  8 12 16 20
5 10 15 20 25
```

**Challenge:** Format the numbers so the columns line up neatly.

---

## 10. Mini Quiz Game — All Four Concepts ⭐

This would be a good **larger homework/project**.

Create a quiz program with **5 questions**.

The program should:

1. Display a question.
2. Give the user multiple-choice answers.
3. Check whether the answer is correct using **selection**.
4. Keep track of the score.
5. Use a **loop** to move through all questions.
6. At the end, display the score and a message:

```text
5/5 → Excellent!
4/5 → Great job!
2–3/5 → Keep practicing!
0–1/5 → You need more practice.
```

**Bonus:** After finishing, ask:

```text
Would you like to play again? yes/no
```

and use a `while` loop to restart the quiz.

---

### A good progression for your class

| Exercise                | Main concept         | Difficulty |
| ----------------------- | -------------------- | ---------- |
| Movie Ticket Calculator | Selection            | ⭐          |
| Multiplication Table    | Definite iteration   | ⭐          |
| FizzBuzz                | Selection + `for`    | ⭐⭐         |
| Number Guessing         | Indefinite iteration | ⭐⭐         |
| Rectangle Pattern       | Nested loops         | ⭐⭐         |
| Number Triangle         | Nested loops         | ⭐⭐⭐        |
| ATM                     | Selection + `while`  | ⭐⭐⭐        |
| Password Checker        | `while` + selection  | ⭐⭐⭐        |
| Multiplication Grid     | Nested loops         | ⭐⭐⭐        |
| Quiz Game               | **All concepts**     | ⭐⭐⭐⭐       |

For a 9th-grade class, I'd particularly recommend **#5 FizzBuzz → #2 Number Guessing → #7 Rectangle → #9 Multiplication Grid → #10 Quiz Game** as a progression. It introduces each concept separately before asking them to combine everything.
