# Day 21: Viewing Processes

## Phase 5 - Process & Service Management | Day 21 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I found the PID of a running process by name, viewed it live in top,
displayed it as part of the full process tree, and identified which
process was using port 80.

## What surprised me
I didn't expect pgrep and lsof -i to be so specific compared to ps —
ps aux dumps everything running on the system, but pgrep let me search
for one process by name directly, and lsof -i showed me exactly which
process owns a given port instead of guessing from a long list.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-20-text-processing-checkpoint/
Next day: ../day-22-process-signals/
