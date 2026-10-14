Here are 5 new Python exercises for your 9th-grade students. These are a step up from the previous exercises, designed for working through together in class. Each one combines at least two concepts, so students have to think about how to structure their programs rather than just apply a single loop or condition.

# Exercise 1: Student Grade Analyzer

Selection + definite iteration

Scenario: A teacher wants a program to analyze a class's test results.

Write a program that asks how many students took a test, then asks for each student's score out of 100.

Requirements

1. Ask how many students' scores will be entered.
2. Use a loop to input each score.
3. Classify each score:
   - 80–100: A
   - 70–79: B
   - 60–69: C
   - 50–59: D
   - Below 50: F
4. Calculate and display the class average.
5. Display how many students passed (score of 50 or above).

Example output

```
How many students? 4
Enter score: 85 -> Grade A
Enter score: 72 -> Grade B
Enter score: 45 -> Grade F
Enter score: 90 -> Grade A

Class average: 73.0
Students passed: 3
```

Challenge: Also display the highest and lowest scores.

# Exercise 2: The ATM Security System

Indefinite iteration + selection

Scenario: A bank needs a simple ATM login system with limited attempts.

The correct PIN is `2468`.

Requirements

1. Ask the user to enter their PIN.
2. Give them a maximum of 3 attempts.
3. If the PIN is correct, display `"Access granted!"` and stop asking.
4. If the PIN is incorrect, display the number of attempts remaining.
5. If all attempts are used, display `"Account temporarily locked!"`.

Example output

```
Enter PIN: 1234
Incorrect PIN. 2 attempts remaining.

Enter PIN: 1111
Incorrect PIN. 1 attempt remaining.

Enter PIN: 2468
Access granted!
```

Challenge: After successful login, display a menu that lets the user check their balance, deposit money, or withdraw money. The menu should repeat until they choose to log out.

Teaching point: Discuss why a `while` loop is useful when the number of attempts depends on the user's input.

# Exercise 3: Treasure Hunt Grid

Nested loops + selection

Scenario: A game designer needs to generate a grid containing a hidden treasure.

The program creates a grid of rows and columns, with one treasure location.

Requirements

1. Ask the user for the number of rows and columns.
2. Ask for the treasure's row and column.
3. Use nested loops to print the grid.
4. Print `T` at the treasure location and `.` everywhere else.
5. Assume row and column numbering starts at 1.

Example output

For 4 rows, 5 columns, and treasure at row 2, column 4:

```
. . . . .
. . . T .
. . . . .
. . . . .
```

Challenge: Allow the player to guess the treasure's coordinates repeatedly until they find it. Give hints such as `"Move down"` or `"Move right"` based on the guess.

Teaching point: The outer loop controls the rows, while the inner loop controls the columns. Students must understand which variables are used in the nested conditions.

# Exercise 4: Number Detective

Selection + loops + validation

Scenario: A program analyzes a range of numbers and identifies their properties.

Requirements

1. Ask the user for a starting number and an ending number.
2. Ensure the ending number is greater than the starting number. Keep asking until the range is valid.
3. Loop through every number in the range, including both endpoints.
4. For each number, determine whether it is:
   - Even or odd
   - Divisible by 3
   - Divisible by both 2 and 3
5. Count how many numbers satisfy each condition and display the totals.

Example output

For the range 1 to 6:

```
1: Odd
2: Even
3: Odd, divisible by 3
4: Even
5: Odd
6: Even, divisible by 3, divisible by both

Even numbers: 3
Odd numbers: 3
Divisible by 3: 2
Divisible by both 2 and 3: 1
```

Challenge: Also identify all prime numbers in the range.

Teaching point: This exercise introduces a loop inside another loop if students use trial division to check whether each number is prime. It also encourages careful condition ordering.

# Exercise 5: Class Battle — Turn-Based Game

All concepts combined

Scenario: Create a simple turn-based battle between a player and a monster.

The player starts with 100 HP, and the monster starts with 80 HP.

Requirements

1. Display a menu each turn:
   - `1. Attack`
   - `2. Heal`
   - `3. Run away`
2. The menu repeats until the monster is defeated, the player is defeated, or the player runs away.
3. If the player attacks, deal a random amount of damage between 10 and 25. (You can introduce Python's `random` module for this.)
4. If the player heals, restore 15 HP, but HP cannot exceed 100.
5. After each attack or heal, the monster attacks for 10 damage if it is still alive.
6. Reject invalid menu choices without ending the game.
7. Display both characters' HP after each turn and announce the final result.

Example output

```
Player HP: 100 | Monster HP: 80

1. Attack
2. Heal
3. Run away
Choose: 1

You dealt 18 damage!
The monster dealt 10 damage!

Player HP: 90 | Monster HP: 62
```

Challenge: Add a critical hit that deals double damage, with a 20% chance of occurring.

Teaching point: Students must manage multiple conditions, update variables inside a `while` loop, and ensure that the monster cannot attack after being defeated.

## Suggested class plan

| Exercise                  | Main focus                        | Suggested time |
| ------------------------- | --------------------------------- | -------------- |
| 1. Student Grade Analyzer | Accumulators, counters, averages  | 20–25 min      |
| 2. ATM Security System    | `while`, attempts, nested menu    | 20–25 min      |
| 3. Treasure Hunt Grid     | Nested loops and coordinates      | 25–30 min      |
| 4. Number Detective       | Range validation and nested loops | 25–30 min      |
| 5. Class Battle           | Combining all concepts            | 30–40 min      |

My recommendation is to start with Exercise 1, then move to Exercise 3. The grade analyzer reinforces variables, counters, and selection, while the treasure hunt makes nested loops more concrete. Finish with the battle game as a collaborative problem-solving exercise.