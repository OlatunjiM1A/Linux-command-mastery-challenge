# Day 27: Remote Access & File Transfer

## Phase 6 - Networking, Scripting & SSH Mastery | Day 27 of 30

## Commands covered today
See commands.md for all 10 commands with syntax and my own explanation
of what each one does and when I would reach for it.

## What I practiced
I generated an SSH key pair, copied the public key to a remote host,
connected to that host without being prompted for a password, then
securely copied a file to and from that server.

## What surprised me
I didn't realize ssh-copy-id does all the manual work for you — without
it, setting up key-based login means manually appending your public
key into the remote's ~/.ssh/authorized_keys file yourself. One command
replaced what would otherwise be several fiddly manual steps.

## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-26-networking-basics/

Next day: ../day-28-bash-scripting/
