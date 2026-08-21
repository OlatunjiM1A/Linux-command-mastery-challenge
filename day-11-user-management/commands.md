# Day 11 Commands — Creating & Managing Users

1. **useradd** — Creates a new user account at a low level. By default
   it does not create a home directory or assign a shell unless you add
   extra flags.

2. **useradd -m** — Creates the new user along with a home directory,
   since plain useradd skips this by default.

3. **useradd -m -s** — Creates the user with a home directory and
   explicitly sets their login shell (e.g. -s /bin/bash), instead of
   leaving them with a default that may not even be interactive.

4. **adduser** — A more user-friendly, interactive wrapper around
   useradd (available on Debian/Ubuntu) that automatically creates a
   home directory, sets a shell, and prompts for a password during
   setup.

5. **passwd** — Sets or changes a user's password. Run by an admin with
   a username, it resets that specific account's password.

6. **usermod -aG** — Adds a user to an additional (secondary) group
   without removing them from any group they're already in. The -a
   (append) flag is essential here — leaving it off can wipe existing
   group memberships.

7. **usermod -s** — Changes a user's login shell after the account has
   already been created.

8. **usermod -l** — Changes a user's login name (username), effectively
   renaming the account without touching its UID or files.

9. **userdel** — Deletes a user account, but by default leaves their
   home directory and files untouched on disk.

10. **userdel -r** — Deletes a user account and also removes their home
    directory and mail spool, cleaning up everything tied to that
    account.
