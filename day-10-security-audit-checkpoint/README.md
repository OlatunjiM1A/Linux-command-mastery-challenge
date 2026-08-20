# Day 10: Security Checkpoint & Audit

## Phase 2 - Permissions, Ownership & Security | Day 10 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
CHECKPOINT. I produced a one-page mini security audit of a server:
checking who logged in recently, who's currently logged in, which
accounts have never logged in, and reviewing every sudo command run in
the current session.

## What surprised me
I didn't expect lastb to specifically track failed login attempts —
it's separate from last, which only shows successful ones. Seeing both
side by side made it obvious how you'd spot a brute-force attempt: a
pile of failed logins in lastb with no matching success in last.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-09-integrity-firewall/
Next day: ../day-11-user-management/
