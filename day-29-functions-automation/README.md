# Day 29: Functions, Arguments & Automation

## Phase 6 - Networking, Scripting & SSH Mastery | Day 29 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I turned yesterday's script into a reusable function that accepts a
service name as an argument, checks its status, restarts it if
stopped, and scheduled it to run hourly using cron.

## What surprised me
I didn't realize positional arguments ($1, $2) work exactly the same
way inside a function as they do for the whole script — a function
called with its own arguments gets its own $1, separate from whatever
was passed to the script overall. That made functions feel like
genuinely self-contained mini-scripts rather than just named blocks of
code.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-28-bash-scripting/

Next day: ../day-30-capstone/
