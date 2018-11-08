# Terminal, Editor, Compiler, Version Control

This collection of exercises will check your ability to operate in a terminal
emulator, edit files, and compile Haskell programs. The instructions assume the
use of [Ubuntu](https://ubuntu.com) or macOS with `ghc` and `git` installed and
added to `$PATH`.

## Part 1

Using `pwd`, `ls`, `mkdir`, and `cd`...

1. Print the working directory.
2. List the contents of the current working directory.
3. Create a new directory, `lesson1`.
4. Verify that the new directory was created.
5. Change the current working directory to `lesson1`.
6. Verify that the working directory was changed.

## Part 2

Using `gedit` (Ubuntu) or `open -e` (macOS)...

1. Inside `lesson1`, open a new file `Main.hs`.
2. Write a program that outputs a line of text.
3. Save the file and close the editor.
4. Verify that the file was created.
5. Find your directory and file using a graphical file manager.

## Part 3

Using `ghc` and the `./` syntax...

1. Compile the program, choosing an appropriate name for the binary.
2. List the files in the current directory to see the build artifacts.
3. Run the program and verify its output.

## Part 4

Using `git` and `mv`...

1. Change the working directory to `~`.
2. Create a new directory, `hectic-solutions`.
3. Initialize a `git` repository in `hectic-solutions`.
4. Move the `lesson1` directory to `hectic-solutions`.
5. Add `Main.hs` to the index, but not the build artifacts.
6. Check the current index (staged).
7. Commit.
8. Create a GitHub repository and follow instructions to set up a remote.

## Part 5

Modify the program to output a different line of text. Compile and test it.
Commit the change and push.
