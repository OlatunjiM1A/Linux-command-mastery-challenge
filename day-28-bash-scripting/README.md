# Day 28: Bash Scripting Foundations

## Phase 6 - Networking, Scripting & SSH Mastery | Day 28 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I wrote and executed a script that reads the user's name, checks
whether a config file exists using an if statement, and loops through
three server names pinging each one.

## What surprised me
I didn't expect the shebang line (#!/bin/bash) to matter as much as it
does — without it, the system tries to figure out which interpreter to
use on its own, which isn't reliable. That one line at the top of the
file is what guarantees the script actually runs as a bash script every
time, regardless of what shell someone happens to be using.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-27-ssh-file-transfer/

Next day: ../day-29-functions-automation/
