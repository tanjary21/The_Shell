# Practical1: The Shell

## Goals
* Practice how to create, copy, move, navigate directories and files with `cd, ls, mv, mkdir`
* Learn how to run files (difference between `sh filename.sh` vs. `./filename.sh`)
* Learn how to use help for commands, for example for `touch` command to create a new file
* Learn how to change permissions with `chmod` command
* Play with redirecting of input/output using angle brackets `<, >` and the pipe operator `|`

## Exercises
1. Please run the command `$SHELL`.

2. Check what your current working directory is. Navigate to `/home/runner/Practical1-The-Shell`

3. Create a new directory `d1` under your current working directory. Navigate into `d1`.

4. Run the command `echo $PATH`

5. Repeat step 4, but use `>` to save the output to a file `paths.txt`

6. Move `paths.txt` to `/home/runner/Practical1-The-Shell`, but rename it to `paths_clone.txt`. **Hint: ** Use `mv`

7. Navigate to `/home/runner/Practical1-The-Shell/d1`. Create a new file `runMe.sh` using the `touch` command. Add the following lines to the file one at a time
  `echo "Hello World"`
  `echo "Hello Mars"`

8. Run the command `sh runMe.sh`. Did it work?
Run the command `./runMe.sh`. Did it work? Use `ls` find out why it didn't work. Use `chmod` to make it work

9. `grep` is a function that lets you search for a particular word given an input. Use `--help` to see how to do it

10. Run `runMe.sh` using one of the methods in Step 8, search the output for the word `"Hello"` using `grep`, and save the result into another file `grep_output.txt`  **Hint: ** Use the `|` and `>` operators
