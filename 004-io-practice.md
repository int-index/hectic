# Haskell Input/Output Practice

This collection of exercises will check your ability to compose Haskell
programs doing input/output.

## Part 1

Write a program that greets the user by name.

Example interaction, with user input marked by `>`:

```
What's your name?
> Jack
Hello, Jack!
```

## Part 2

Write a program that takes a traffic light color as input and outputs a
permissible action:

Example interactions, with user input marked by `>`:

1. The user enters "green":
   ```
   Traffic light?
   > green
   Go!
   ```

2. The user enters "red":
   ```
   Traffic light?
   > red
   Stop.
   ```

3. The user enters "yellow":
   ```
   Traffic light?
   > yellow
   Stop if possible.
   ```

4. The user enters "purple":
   ```
   Traffic light?
   > purple
   Unknown color.
   ```

## Part 3

Write a program that outputs a countdown from 999 to 1:

```
999
998
997
...
4
3
2
1
Start!
```

## Part 4

Implement a guessing game. The computer generates a random number and
repeatedly prompts the user to guess it until the user enters a correct number.

Example interactions, with user input marked by `>`:

* The computer generates `6`. The user enters "5", then "9", then "6".
  ```
  Guess a number from 0 to 10:
  > 5
  Too small.
  > 9
  Too big.
  > 6
  Correct!
  ```

* The computer generates `2`. The user enters "7", then "2".
  ```
  Guess a number from 0 to 10:
  > 7
  Too big.
  > 2
  Correct!
  ```

* The computer generates `10`. The user enters "99", then "10".
  ```
  Guess a number from 0 to 10:
  > 99
  Out of range.
  > 10
  Correct!
  ```
