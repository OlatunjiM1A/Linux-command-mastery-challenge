# Day 11: Creating & Managing Users

## Phase 3 - Users, Groups & Package Management | Day 11 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I created a new user with a home directory and Bash shell, set their
password, added them to a secondary group, renamed the account, then
removed it along with its home directory.

## What surprised me
I didn't realize useradd on its own doesn't create a home directory or
set a shell by default — you have to explicitly pass -m and -s, or the
account ends up with no home folder and a non-interactive login shell.
adduser (Debian's friendlier wrapper) handles all of that automatically,
which explains why the two commands feel so different in practice.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-10-security-audit-checkpoint/
Next day: ../day-12-groups/
