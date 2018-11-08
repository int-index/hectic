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

1. ```
   Traffic light?
   > green
   Go!
   ```

2. ```
   Traffic light?
   > red
   Stop.
   ```

3. ```
   Traffic light?
   > yellow
   Stop if possible.
   ```

4. ```
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

* ```
  Guess a number from 0 to 10:
  > 5
  Too small.
  > 9
  Too big.
  > 6
  Correct!
  ```

* ```
  Guess a number from 0 to 10:
  > 99
  Out of range.
  ```
