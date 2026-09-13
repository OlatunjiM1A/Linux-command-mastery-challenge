# Day 30: Capstone — Full System Command Mastery Review

## Phase 6 - Networking, Scripting & SSH Mastery | Day 30 of 30

## Commands covered today
See commands.md for the 10 capstone tasks, each drawing on commands
learned across all six phases of the challenge.

## What I practiced
CAPSTONE PROJECT. I built one Bash script that connects to a remote
server over SSH, deploys a file with the correct ownership and
permissions, restarts the relevant service, verifies it's healthy using
systemctl and journalctl, and logs the entire run. I then walked a peer
through it end to end, using only commands from this challenge.

## What surprised me
Building the capstone made it obvious how much every earlier day fed
into this one script — SSH from Day 27, chmod/chown from Days 6-7,
systemctl and journalctl from Days 23-24, and scripting fundamentals
from Days 28-29 all had to work together in the right order for the
deployment to actually succeed. Nothing in this script was new; it was
entirely about combining 29 days of separate lessons into one coherent
workflow.

## Evidence
Screenshot or terminal transcript of the drill in evidence/, plus the
health-check.sh script itself.

## Related
Previous day: ../day-29-functions-automation/

Next day: N/A — Day 30 is the final day
