# Small-Step Semantics

This collection of exercises will check your understanding of basic
evaluation/execution principles.

## Part 1

Given `sqr` defined as follows:

```haskell
sqr = \x -> x * x
```

Reduce `sqr (sqr 5)`, naming each reduction rule.

## Part 2

Given `double` defined as follows:

```haskell
double = \n -> n + n
```

Reduce `double (double (double 2))`, naming each reduction rule.

## Part 3

Given `f` defined as follows:

```
f = \k -> if k == 0
          then k + 10
          else k * 2
```

Reduce `f (f 0)`.

## Part 4

Given `f` defined as follows:

```
f =
  \x ->
    if x == 0
    then 1
    else x * f (x - 1)
```

Reduce `f 3`. Hint: β-reduce as soon as possible.

## Part 5

Given the following program:

```
module Main where

main =
  getLine >>= \s -> putStrLn s >> putStrLn s
```

Reduce `main`, keeping track of side effects.

## Part 6

Given the following program:

```
module Main where

main =
  prompt "Enter the first line:" >>=
    \firstStr ->
      prompt "Enter the second line" >>=
        \secondStr ->
          putStrLn "Sorted lines:" >>
            if firstStr < secondStr
            then putTwoLines firstStr secondStr
            else putTwoLines secondStr firstStr

putTwoLines a b =
  putStrLn a >> putStrLn b

prompt str =
  putStrLn str >> getLine
```

Reduce `main`, keeping track of side effects.
