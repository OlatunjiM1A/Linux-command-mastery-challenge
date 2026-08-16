# Day 6 — Permissions Drill

## Objective

Create a script file and set it to rwxr-xr-x using all three chmod methods (relative, assignment, octal) in turn, confirming the result with ls -l after each change.

## commds I ran

```bash
touch script.sh
chmod u+rwx,g+rx,o+rx script.sh
ls -l script.sh
chmod u=rwx,g=rx,o=rx script.sh
ls -l script.sh
chmod 755 script.sh
ls -l script.sh

