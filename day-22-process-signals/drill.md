# Day 22 Practice Drill

## Task
Start a long-running command in the background, suspend it, resume it
in the background, then start a second one that survives you logging
out, using nohup.

## Commands run, in order

sleep 300 
jobs
fg
# Ctrl+Z pressed here to suspend
bg
jobs
nohup sleep 600 &
disown
jobs

