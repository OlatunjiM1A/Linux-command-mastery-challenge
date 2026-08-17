# Day 07 Commands — Ownership & Special Bits

1. **chown** — Changes the owner of a file or directory. Only root or
   the current owner (in some cases) can hand ownership to someone else.

2. **chown user:group** — Changes both the owner and the group of a file
   in a single command, instead of running chown and chgrp separately.

3. **chown -R** — Applies an ownership change recursively, affecting a
   directory and everything inside it, not just the top-level folder.

4. **chgrp** — Changes only the group associated with a file or
   directory, leaving the owner untouched.

5. **chmod u+s (SUID)** — Sets the Set User ID bit on an executable. When
   run, the program executes with the permissions of the file's owner,
   not the person running it — this is how tools like `passwd` let
   normal users make a change that technically needs root access.

6. **chmod g+s (SGID)** — Sets the Set Group ID bit. On a directory,
   this means any new file created inside automatically inherits the
   directory's group instead of the creating user's default group —
   useful for shared team folders.

7. **chmod +t (sticky bit)** — Restricts deletion inside a shared,
   world-writable directory so that only a file's owner (or root) can
   delete or rename it, even though everyone can create files there.
   `/tmp` uses this by default.

8. **find -perm /4000** — Searches for files that have the SUID bit set
   anywhere on the system. This is a basic but important security audit
   step, since an unexpected SUID binary can be a sign of a
   privilege-escalation risk.

9. **getfacl** — Displays the Access Control List for a file, showing
   more detailed, fine-grained permissions than the standard
   owner/group/other model allows.

10. **setfacl -m** — Modifies a file's ACL, letting you grant specific
    permissions to an individual user or group beyond what standard
    chmod permissions allow.
