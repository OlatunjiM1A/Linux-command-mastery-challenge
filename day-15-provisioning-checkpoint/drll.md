# Day 15 Practice Drill

## Task
CHECKPOINT. Provision a complete new team member account (user, groups,
password) and install the three tools they need for their role, in a
single documented sequence.

## Commands run, in order

sudo useradd -m -G sudo,developers -s /bin/bash newmember
sudo passwd newmember
id newmember
sudo apt update && sudo apt install -y git curl tree
dpkg -l | grep -E "git|curl|tree"
history

## Notes
Creating the account with groups already attached (-G) meant I didn't
need a separate usermod step afterward. Checking with id confirmed
group membership before moving on to installs, which felt like the
right order — get the account fully set up first, then give it tools.
history at the end gave me a clean record of the whole sequence, which
doubled as documentation for the drill itself.
