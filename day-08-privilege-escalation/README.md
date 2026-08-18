# Day 08: Privilege Escalation & Identity

## Phase 2 - Permissions, Ownership & Security | Day 8 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does.

## What I practiced
I ran a command that failed due to lack of permission, then instantly
re-ran it with sudo using sudo !! instead of retyping the whole thing.
After that, I checked exactly which commands my account is permitted to
run as another user using sudo -l.

## What surprised me
I didn't realize sudo !! re-runs your last command with sudo prefixed
automatically — no need to retype anything. Also surprising: sudo -l
shows you the exact boundaries of your access before you even try
something, which is a much safer way to check permissions than trial
and error.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-07-ownership/
Next day: ../day-09-integrity-firewall/
