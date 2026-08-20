# Day 10 Commands — Security Checkpoint & Audit

1. **find / -perm /4000 (SUID audit)** — Searches the entire filesystem
   for files with the SUID bit set. A core part of any security audit,
   since an unexpected SUID binary can be a privilege-escalation risk.

2. **last** — Shows a history of successful logins on the system,
   including who logged in, from where, and for how long.

3. **lastlog** — Shows the most recent login time for every user account
   on the system, including accounts that have never logged in at all.

4. **w** — Shows who is currently logged in, what they're doing, and how
   long their session has been idle — a live snapshot rather than a
   history.

5. **who** — A simpler version of w, showing just who is currently
   logged in and from where, without the extra activity detail.

6. **groups** — Lists which groups the current (or a specified) user
   belongs to.

7. **passwd** — Used to change a user's password. Run without a
   username, it changes your own; with one, an admin can reset another
   user's password.

8. **chage -l** — Lists password aging information for a user — when it
   was last changed, when it expires, and any account expiration date.

9. **lastb** — Shows a history of failed login attempts, separate from
   last's successful-login history. Useful for spotting brute-force
   attempts.

10. **history | grep sudo** — Searches the command history for every
    line containing sudo, giving a quick view of every privileged
    command run in the current session.
