# Day 09 Practice Drill

## Task
Generate a SHA-256 checksum for a downloaded file to verify its
integrity, make a file immutable with chattr, then open only port 22
and port 443 on the firewall.

## Commands run, in order

sha256sum somefile.txt
chattr +i somefile.txt
lsattr somefile.txt
sudo ufw allow 22
sudo ufw allow 443
sudo ufw enable
sudo ufw status

## Notes
The checksum gave me a fingerprint I could compare later to confirm the
file hadn't changed. Once I set the immutable flag, even trying to
delete the file as its owner failed until I ran chattr -i to remove the
protection. Enabling ufw with only 22 and 443 allowed meant every other
port got blocked by default, which is exactly the "deny by default,
allow explicitly" approach you want on a real server.
