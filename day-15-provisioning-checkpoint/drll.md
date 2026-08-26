# Day 15 Practice Drill

## Task
CHECKPOINT. Provision a complete new team member account (user, groups,
password) and install the three tools they need for their role, in a
single documented sequence.

## Commands run, in order

sudo useradd -m -G sudo,developers -s /bin/bash devopsintern
sudo passwd devopsintern
id devopsintern
sudo apt update && sudo apt install -y git curl tree
dpkg -l | grep -E "git|curl|tree"
history
