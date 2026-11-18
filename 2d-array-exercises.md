# Python 2D Array Coding Exercises

These exercises help you practise **2D arrays in Python**. A 2D array is represented by a list of lists: each inner list represents one row.

## Instructions

- Use Python lists of lists to represent 2D arrays.
- Write a working Python program for each exercise.
- Use nested loops when processing rows and columns.
- Python indexes start at `0`. For example, `matrix[0][1]` refers to the first row and second column.
- Unless stated otherwise, do not use built-in functions that directly solve the task (such as `sum()`, `max()`, or `min()`).

---

## Level 1 – Beginner

### Exercise 1: My First 2D Array
**Difficulty: Very Easy**

Create a 2D array called `numbers`:

```python
numbers = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
```

Write a program that:

1. Displays the entire 2D array.
2. Displays the value in the first row and second column.
3. Displays the value in the third row and first column.
4. Displays the value in the second row and third column.

**Expected output:**

```text
[[1, 2, 3], [4, 5, 6], [7, 8, 9]]

First row, second column: 2
Third row, first column: 7
Second row, third column: 6
```

### Exercise 2: Storing Student Names
**Difficulty: Easy**

A teacher wants to organise students into 3 groups, with 2 students in each group.

Write a program that:

1. Creates an empty 2D array called `students`.
2. Asks the user to enter the names of 2 students for each of the 3 groups.
3. Stores the names in the correct rows.
4. Displays each group and its students.

**Example output:**

```text
Enter the name of student 1 in group 1: Alex
Enter the name of student 2 in group 1: Sarah
Enter the name of student 1 in group 2: John
Enter the name of student 2 in group 2: Emily
Enter the name of student 1 in group 3: David
Enter the name of student 2 in group 3: Mia

Group 1: Alex, Sarah
Group 2: John, Emily
Group 3: David, Mia
```

### Exercise 3: Updating a Value
**Difficulty: Easy**

You are given this 2D array:

```python
scores = [
    [75, 80, 90],
    [65, 70, 85],
    [95, 88, 78]
]
```

Write a program that:

1. Displays the original 2D array.
2. Asks the user to enter a row number (1–3).
3. Asks the user to enter a column number (1–3).
4. Asks the user to enter a new score.
5. Updates the selected value.
6. Displays the updated 2D array.

**Remember:** User-entered row and column numbers start at 1, but Python indexes start at 0. Convert the positions before accessing the list.

---

## Level 2 – Intermediate

### Exercise 4: Calculating Row Totals
**Difficulty: Intermediate**

A teacher records the scores of 4 students across 3 tests.

```python
scores = [
    [80, 75, 90],
    [65, 70, 85],
    [90, 88, 92],
    [72, 81, 78]
]
```

Write a program that:

1. Uses a loop to calculate the total score for each student.
2. Displays each student's three test scores.
3. Displays each student's total score.

**Expected output:**

```text
Student 1 total: 245
Student 2 total: 220
Student 3 total: 270
Student 4 total: 231
```

### Exercise 5: Calculating Column Averages
**Difficulty: Intermediate**

Using the `scores` array from Exercise 4, write a program that:

1. Calculates the total score for Test 1, Test 2, and Test 3.
2. Calculates the average score for each test.
3. Displays each test's total and average.

**Expected averages:**

```text
Test 1 average: 76.75
Test 2 average: 78.5
Test 3 average: 86.25
```

**Hint:** A column contains the values at the same column index across different rows. You will need to loop through the rows for each column.

### Exercise 6: Searching for a Number
**Difficulty: Intermediate**

You are given this 2D array:

```python
numbers = [
    [5, 8, 3, 2],
    [7, 8, 1, 4],
    [9, 6, 8, 5]
]
```

Write a program that:

1. Asks the user to enter a number to search for.
2. Searches through every element in the 2D array.
3. Checks whether the number exists.
4. If found, displays every position where it appears.
5. If it does not exist, displays an appropriate message.

**Example output:**

```text
Enter a number to search for: 8

Number found at:
Row 1, Column 2
Row 2, Column 2
Row 3, Column 3
```

*Display row and column positions starting from 1.*

### Exercise 7: Finding the Highest and Lowest Values
**Difficulty: Intermediate**

You are given this 2D array:

```python
temperatures = [
    [28, 30, 27],
    [32, 29, 31],
    [25, 26, 28]
]
```

Write a program that:

1. Finds the highest temperature in the 2D array.
2. Finds the lowest temperature in the 2D array.
3. Displays both values.

**Challenge:** Use nested loops without using `max()` or `min()`.

---

## Level 3 – Advanced

### Exercise 8: Calculating the Diagonal Totals
**Difficulty: Challenging**

You are given this square 2D array:

```python
numbers = [
    [2, 4, 6],
    [1, 5, 9],
    [3, 7, 8]
]
```

The **main diagonal** runs from the top-left corner to the bottom-right corner.

Write a program that:

1. Displays the values on the main diagonal.
2. Calculates the total of the main diagonal.
3. Displays the values on the opposite diagonal, from the top-right corner to the bottom-left corner.
4. Calculates the total of the opposite diagonal.

**Expected output:**

```text
Main diagonal: 2, 5, 8
Main diagonal total: 15

Opposite diagonal: 6, 5, 3
Opposite diagonal total: 14
```

### Exercise 9: Adding Two 2D Arrays
**Difficulty: Challenging**

You are given two 2D arrays:

```python
array_a = [
    [1, 2, 3],
    [4, 5, 6]
]

array_b = [
    [7, 8, 9],
    [1, 2, 3]
]
```

Write a program that:

1. Creates a new empty 2D array called `result`.
2. Adds the values in `array_a` and `array_b` that are in the same positions.
3. Stores each answer in the corresponding position in `result`.
4. Displays the two original arrays and the resulting array.

**Expected result:**

```text
[8, 10, 12]
[5, 7, 9]
```

**Challenge:** Modify your program so it can add two 2D arrays with any matching number of rows and columns.

### Exercise 10: Classroom Seating Management System
**Difficulty: Advanced**

A teacher wants a program to manage a classroom seating plan. The classroom has 3 rows, with 4 seats in each row.

Create a 2D array called `seats` to store the names of students sitting in each seat. Use `"Empty"` for seats that are not occupied.

Your program should display this menu:

```text
===== CLASSROOM SEATING SYSTEM =====

1. Display seating plan
2. Seat a student
3. Remove a student
4. Find a student
5. Count empty seats
6. Exit
```

Write a program that:

1. Starts with all seats marked as `"Empty"`.
2. Allows the user to select an option from the menu.
3. Performs the selected operation.
4. Returns to the menu after each operation until the user selects Exit.

**Additional requirements:**

- When seating a student, ask for the row number (1–3), column number (1–4), and student's name.
- Do not allow a student to be seated if the selected seat is already occupied.
- When removing a student, ask for the row and column, then mark that seat as `"Empty"`.
- When finding a student, search the entire seating plan and display the student's row and column if found.
- When counting empty seats, display the total number of seats marked `"Empty"`.
- Display an error message if the user enters an invalid menu option, row, or column.
- Use nested loops to display and search the seating plan.

**Challenge:** Prevent the same student from being seated in more than one seat.

---

## Skills Covered

| Exercise | Main programming concept |
|---|---|
| 1 | Creating and accessing 2D arrays |
| 2 | Inputting and displaying 2D arrays |
| 3 | Updating values using row and column indexes |
| 4 | Calculating row totals |
| 5 | Calculating column totals and averages |
| 6 | Searching a 2D array |
| 7 | Finding maximum and minimum values |
| 8 | Working with diagonals |
| 9 | Adding two 2D arrays |
| 10 | Combining 2D arrays, nested loops, selection and input validation |

**Good luck, and remember to test your programs with different values!**
