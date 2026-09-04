# Day 22: Controlling Processes with Signals

## Phase 5 - Process & Service Management | Day 22 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I started a long-running command in the background, suspended it,
resumed it in the background, then started a second one using nohup so
it would keep running even after I logged out.

## What surprised me
I didn't realize Ctrl+Z doesn't stop a process — it just pauses it.
The process is still there, just frozen, until you either bring it back
with fg/bg or kill it outright. That distinction between "paused" and
"terminated" wasn't obvious to me before actually testing it.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-21-viewing-processes/
Next day: ../day-23-systemctl-basics/
