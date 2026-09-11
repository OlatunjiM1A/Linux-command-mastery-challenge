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
Real cloud setups threw a lot more at me than the plain drill instructions suggested. First, user@<ip> doesn't work on AWS — cloud AMIs use a specific default username (ubuntu for Ubuntu AMIs), not a generic user. Second, cloud instances disable password authentication by default, so ssh-copy-id failed with Permission denied (publickey) until I authenticated using my existing .pem key instead of a password. Third, storing my private key inside the Windows filesystem mount (/mnt/c/...) gave it 0777 permissions, and SSH refuses to use a private key that's world-readable — I had to move it into WSL's native filesystem and lock it down with chmod 400. Finally, once I'd authenticated with the .pem key, ssh-copy-id assumed my new key was already installed and skipped it — I had to use the -f flag to force it to actually append id_ed25519.pub to the remote's authorized_keys.
## Evidence
Screenshot or terminal transcript of the drill in evidence/.

## Related
Previous day: ../day-26-networking-basics/

Next day: ../day-28-bash-scripting/
