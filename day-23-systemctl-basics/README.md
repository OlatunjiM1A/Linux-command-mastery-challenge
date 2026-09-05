# Day 23: Init Systems & systemctl Basics

## Phase 5 - Process & Service Management | Day 23 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I picked a service, stopped it, confirmed it was inactive, restarted
it, enabled it to auto-start at boot in a single combined command, and
confirmed both its active and enabled state afterward.

## What surprised me
I didn't realize "active" and "enabled" are two completely separate
states in systemd. A service can be running right now (active) but not
set to start automatically at boot (disabled), or the reverse — enabled
to start at boot but not currently running. Checking both separately
with systemctl status made that distinction clear.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-22-process-signals/
Next day: ../day-24-service-logs/
