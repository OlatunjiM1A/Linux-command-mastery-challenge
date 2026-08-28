# Day 17 Practice Drill

## Task
Add a permanent environment variable and a custom alias to your
.bashrc, reload it without opening a new terminal, and confirm both
persist in a fresh session.

## Commands run, in order

nano ~/.bashrc
# Added: export MYPROJECT="/home/user/projects"
# Added: alias ll='ls -la'
source ~/.bashrc
echo $MYPROJECT
ll
exit
# reopened terminal
echo $MYPROJECT
ll

