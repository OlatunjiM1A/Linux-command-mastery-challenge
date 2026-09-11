# Day 28 Commands — Bash Scripting Foundations

1. **#!/bin/bash (shebang)** — The first line of a script that tells the
   system which interpreter should run it. Without it, the script's
   behavior depends on how it's called, which is unreliable.

2. **chmod +x script.sh** — Makes a script file executable, which is
   required before it can be run directly rather than passed as an
   argument to bash.

3. **./script.sh** — Runs an executable script located in the current
   directory. The ./ is necessary because the current directory isn't
   normally part of the shell's search path for security reasons.

4. **VAR=value** — Assigns a value to a shell variable. No spaces are
   allowed around the equals sign, unlike most other languages.

5. **$() command substitution** — Runs a command and substitutes its
   output directly into another command or variable assignment (e.g.
   today=$(date)).

6. **read -p** — Prompts the user with a message and waits for input,
   storing whatever they type into a variable.

7. **if / elif / else / fi** — The core conditional structure in bash,
   letting a script branch its behavior based on whether a condition is
   true or false. fi closes the if block, similar to how loops need an
   explicit end keyword.

8. **-gt / -lt / -eq** — Comparison operators used inside conditionals
   for numeric tests: greater than, less than, and equal to,
   respectively.

9. **for loop** — Repeats a block of commands once for each item in a
   list (e.g. looping through a list of server names or filenames).

10. **while loop** — Repeats a block of commands as long as a given
    condition remains true, useful when the number of iterations isn't
    known in advance.
