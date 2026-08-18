# Day 08 Commands — Privilege Escalation & Identity

1. **sudo** — Runs a single command with elevated (root) privileges,
   without needing to fully log in as root. The most common way to
   perform admin tasks safely and with an audit trail.

2. **sudo -i** — Starts an interactive root login shell, effectively
   putting you into a full root session instead of running just one
   command with elevated privileges.

3. **sudo -u** — Runs a command as a specific user instead of root
   (e.g. `sudo -u www-data whoami`). Useful for testing what a service
   account can or can't do.

4. **sudo !!** — Re-runs the previous command with sudo automatically
   added in front of it. A fast fix for when a command fails because you
   forgot to elevate it in the first place.

5. **sudo -l** — Lists exactly which commands the current user is
   permitted to run with sudo, and as which users. A safe way to check
   your own boundaries before attempting something.

6. **visudo** — Safely opens the sudoers file for editing, using syntax
   checking to prevent a mistake that could lock every admin out of
   sudo access.

7. **su** — Switches to another user account, most commonly root,
   starting a new shell session as that user.

8. **su -** — Same as su, but also loads that user's full environment
   (like their home directory and PATH), simulating a real fresh login
   instead of just changing identity mid-session.

9. **whoami** — Prints the username of whoever is currently running the
   shell. A quick sanity check, especially after switching users.

10. **id** — Shows a fuller identity picture than whoami: the user's UID,
    GID, and every group they belong to.
