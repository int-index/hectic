# Haskell Syntax

This collection of exercises will check your ability to read Haskell programs.

## Part 1

Perform syntactic analysis of the following Haskell snippet:

```haskell
seventeen =
  2 + (3 * 5)

twentyfive =
  (2 + 3) * 5

xx =
  2 + 3 * 5
```

## Part 2

Perform syntactic analysis of the following Haskell snippet:

```haskell
module Main where

main =
  putStrLn "What's your name?" >> (getLine >>= greet)

greet =
  \name -> putStrLn "Hello" >>
           putStrLn name
```

## Part 3

Perform syntactic analysis of the following Haskell snippet:

```haskell
module Main where

main = putMany "hello" "bye" 4

putMany =
  \line ->
  \lastline ->
  \count -> if count == 0
            then putStrLn lastline
            else putStrLn line >>
                 putMany line lastline (count - 1)
```
