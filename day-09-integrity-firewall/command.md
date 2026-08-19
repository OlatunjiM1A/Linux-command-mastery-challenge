# Day 09 Commands — Integrity, Encryption & Firewalling

1. **md5sum** — Generates an MD5 checksum for a file, giving it a short
   fingerprint you can compare against a known value to check if the
   file has changed. Considered weak for security purposes now, but
   still common for basic integrity checks.

2. **sha256sum** — Generates a SHA-256 checksum, a stronger and more
   collision-resistant fingerprint than MD5. The standard choice today
   for verifying that a downloaded file hasn't been tampered with.

3. **gpg --gen-key** — Generates a new GPG key pair (public and private),
   used for encrypting files and verifying digital signatures.

4. **gpg --encrypt** — Encrypts a file using GPG, so only someone with
   the matching private key can decrypt and read it.

5. **gpg --decrypt** — Decrypts a file that was previously encrypted
   with GPG, using the matching private key.

6. **chattr +i** — Sets a file as immutable, meaning it cannot be
   modified, deleted, or renamed by anyone — even root — until the flag
   is removed. A strong protection layer beyond normal permissions.

7. **lsattr** — Lists the special file attributes set on a file, such as
   the immutable flag set by chattr, which don't show up in a normal
   ls -l listing.

8. **ufw enable** — Turns on the Uncomplicated Firewall, activating
   whatever rules have been configured and blocking everything not
   explicitly allowed.

9. **ufw allow** — Adds a rule permitting traffic on a specific port or
   service (e.g. `ufw allow 22` opens SSH access).

10. **ufw status** — Shows the firewall's current state and active
    rules, confirming exactly what's open and what's blocked.
