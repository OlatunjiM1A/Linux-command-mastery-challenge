# Day 06 Commands — Reading & Setting Permissions

1. **ls -l (permission string)** — It is a long list shows a 10-character
   string like `-rwxr-xr-x` at the start of each line. The first
   character shows file type, and the next nine show read/write/execute
   permissions for owner, group, and others, in that order.

2. **chmod (relative +/-)** — Adds or removes a specific permission
   without touching the others (e.g. `chmod +x file` adds execute for
   everyone, `chmod u-w file` removes write from the owner only).

3. **chmod (assignment =)** — Sets a permission to an exact value,
   overwriting whatever was there before (e.g. `chmod u=rwx file` makes
   the owner's permissions exactly read, write, execute — nothing more,
   nothing less).

4. **chmod 755 (octal)** — Sets permissions using a three-digit number,
   one digit each for owner/group/others. 755 means the owner gets full
   rwx, while group and others get read and execute only.

5. **chmod 644 (octal)** — A common file permission: owner gets read and
   write, group and others get read-only. No execute for anyone.

6. **chmod 600 (octal)** — A stricter setting: only the owner can read
   or write the file, and nobody else has any access at all. Common for
   files with sensitive content, like SSH private keys.

7. **chmod -R** — Applies a permission change recursively, affecting a
   directory and everything inside it, not just the top-level folder.

8. **umask** — Sets the default permission mask applied to every new
   file or directory you create, determining what permissions they start
   with before you manually change anything.

9. **umask -S** — Shows the current umask setting in a readable
   symbolic format (like u=rwx,g=rx,o=rx) instead of the default numeric
   output.

10. **stat -c '%A %U %G'** — Uses stat with a custom format string to
    print just the permission string, owner, and group of a file — a
    quick, focused way to check exactly those three things instead of
    the full metadata dump.
