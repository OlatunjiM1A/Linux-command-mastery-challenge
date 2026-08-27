# Day 16: Environment Variables

## Phase 4 - Environment, Vim & Text Processing | Day 16 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I set a temporary environment variable, confirmed it existed, then
unset it. After that, I added a directory to my PATH for the current
session only, and proved the shell could find a script inside it
without me typing the full path.

## What surprised me
I didn't realize environment variables set with export only last for
the current shell session by default — closing the terminal wipes them
completely. Nothing persists unless it's written into a config file
like .bashrc, which is a different topic from just setting a variable.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-15-provisioning-checkpoint/
Next day: ../day-17-shell-configuration/
