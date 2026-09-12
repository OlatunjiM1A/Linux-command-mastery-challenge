# Day 29 Commands — Functions, Arguments & Automation

1. **function_name() { }** — Defines a reusable block of code that can
   be called by name later in the script, avoiding repetition when the
   same logic is needed more than once.

2. **$1 / $2 positional args** — Refers to the first, second, etc.
   arguments passed to a script or function, letting it behave
   differently based on what's supplied when it's called.

3. **$# / $* / $@** — $# gives the number of arguments passed; $* and
   $@ both represent all arguments, though $@ handles arguments
   containing spaces more reliably when quoted.

4. **$0** — Refers to the name of the script itself, as it was invoked
   — useful for error messages or logging that reference the script by
   name.

5. **exit codes ($?)** — $? holds the exit status of the last command
   that ran; 0 means success, any non-zero value indicates some kind of
   failure, letting scripts check whether a previous step worked.

6. **crontab syntax** — The five-field time format cron uses to
   schedule jobs: minute, hour, day of month, month, day of week —
   each field can be a specific value, a range, or an asterisk for
   "every."

7. **cron scheduling (0 * * * *)** — A specific example of crontab
   syntax meaning "run at minute 0 of every hour" — i.e., once every
   hour, on the hour.

8. **nohup script.sh &** — Runs a script in the background in a way
   that survives the terminal session closing, combining nohup and &
   together in one line.

9. **trap** — Catches a signal (like Ctrl+C or a script exit) and runs
   a specified command in response — useful for cleanup tasks before a
   script actually terminates.

10. **logger** — Sends a message directly into the system log
    (accessible via journalctl or /var/log/syslog), letting scripts
    record their own activity into the standard logging system.
