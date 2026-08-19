# Day 09: Integrity, Encryption & Firewalling

## Phase 2 - Permissions, Ownership & Security | Day 9 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I generated a SHA-256 checksum for a file to verify its integrity, made
a file immutable using chattr so it couldn't be modified or deleted even
by the owner, then configured ufw to open only port 22 and port 443,
leaving everything else closed.

## What surprised me
I didn't expect chattr +i to override normal permissions entirely —
even as the file's owner with full rwx permissions, I still couldn't
delete or edit it until I removed the immutable flag. It's a stronger
lock than chmod alone.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-08-privilege-escalation/
Next day: ../day-10-security-audit-checkpoint/
