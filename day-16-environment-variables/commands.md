# Day 16 Commands — Environment Variables

1. **printenv** — Prints all environment variables currently set in the
   shell session, one per line.

2. **printenv HOME** — Prints the value of one specific environment
   variable (HOME in this case), instead of dumping the entire list.

3. **echo $VAR** — Prints the value of a variable by referencing it with
   a dollar sign. Works for both environment variables and regular
   shell variables.

4. **export** — Marks a variable as an environment variable, making it
   available to child processes and programs started from this shell,
   not just the shell itself.

5. **unset** — Removes a variable entirely from the current shell
   session, whether it was exported or not.

6. **env** — Runs a command in a modified environment, or with no
   command, prints the current environment variables — similar to
   printenv.

7. **source** — Reads and executes a file's commands in the current
   shell session, rather than a new subshell. Commonly used to reload a
   config file like .bashrc without opening a new terminal.

8. **echo $PATH** — Prints the current PATH variable, which is the list
   of directories the shell searches through when looking for a command
   to run.

9. **export PATH=$PATH:** — Appends a new directory to the existing
   PATH, so the shell can find executables in that folder too — without
   this, you'd have to type a script's full path every time to run it.

10. **cat /etc/environment** — Displays the contents of the
    system-wide environment configuration file, which sets default
    variables for all users on the system, not just the current shell.
