# Day 13: APT Package Management (Debian/Ubuntu)

## Phase 3 - Users, Groups & Package Management | Day 13 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I refreshed the package index, searched for and installed a small
utility, inspected its package details, then purged it completely along
with its configuration files.

## What surprised me
I didn't realize apt remove and apt purge behave differently — remove
uninstalls the software but leaves configuration files behind, while
purge wipes those config files too. If you want a truly clean removal,
remove alone isn't enough.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-12-groups/
Next day: ../day-14-dnf-yum/
