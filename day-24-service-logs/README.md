# Day 24: Deeper Service Management & Logs

## Phase 5 - Process & Service Management | Day 24 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I listed every failed service on the system, then pulled today's logs
for one specific service, filtered down to errors only, and followed
that service's log output live for a minute.

## What surprised me
I didn't expect journalctl to be this granular — being able to filter
by a specific service, a time range, and a severity level (errors only)
all at once meant I could go straight to what mattered instead of
scrolling through an entire day's worth of unrelated log noise.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-23-systemctl-basics/
Next day: ../day-25-operational-snapshot-checkpoint/
