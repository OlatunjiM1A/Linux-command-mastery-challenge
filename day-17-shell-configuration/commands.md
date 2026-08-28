# Day 17 Commands — Persisting Configuration

1. **nano ~/.bashrc** — Opens the personal shell startup file for
   editing. This file runs automatically every time a new interactive
   Bash session starts, making it the place to put anything you want
   to persist.

2. **source ~/.bashrc** — Re-runs the .bashrc file in the current shell
   session, applying any new changes immediately instead of waiting for
   the next fresh terminal.

3. **cat ~/.bash_profile** — Displays the contents of the bash_profile
   file, which runs for login shells specifically — different from
   .bashrc, which runs for interactive non-login shells.

4. **sudo nano /etc/environment** — Opens the system-wide environment
   file for editing, which sets default variables for every user on the
   machine, not just the current one.

5. **sudo nano /etc/bash.bashrc** — Opens the system-wide Bash
   configuration file, which applies to every user's interactive shell
   by default, before their personal .bashrc runs on top of it.

6. **alias** — Creates a shortcut name for a longer command (e.g.
   `alias ll='ls -la'`), saving typing for commands used often.

7. **unalias** — Removes a previously created alias, restoring the
   original command name to its normal, un-shortened behavior.

8. **type** — Shows how the shell would interpret a given command name —
   whether it's an alias, a built-in, or an actual file on disk.

9. **which** — Shows the full path to the executable that would run when
   you type a given command name, searching through PATH.

10. **whereis** — Similar to which, but broader — it can show the
    binary, source, and manual page locations for a command, not just
    the executable path.
