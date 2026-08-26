# Day 15 Commands — Users & Packages Checkpoint

1. **id <user>** — Shows a user's UID, GID, and full group membership.
   A quick way to confirm an account's identity and access setup after
   creating or modifying it.

2. **getent passwd <user>** — Queries the system's user database (which
   may include sources beyond just /etc/passwd) to confirm whether an
   account actually exists and see its details.

3. **useradd -m -G** — Creates a new user with a home directory (-m) and
   immediately adds them to one or more supplementary groups (-G) in
   the same command.

4. **passwd <user>** — Sets or resets a specific user's password,
   typically run by an admin right after creating the account.

5. **apt list --installed** — Lists every package currently installed
   on the system via apt, useful for confirming what's already present
   before installing more.

6. **apt list --upgradable** — Lists installed packages that have a
   newer version available, without actually upgrading anything yet.

7. **apt update && apt install -y** — Chains two commands together:
   refresh the package index, then install a package without a
   confirmation prompt (-y), in one line.

8. **dpkg -l | grep** — Lists all installed packages via dpkg, piped
   through grep to search for one specific package by name.

9. **apt autoremove** — Removes packages that were installed as
   dependencies but are no longer needed by anything currently
   installed, keeping the system clean after installs/removals.

10. **history** — Displays a list of previously run commands in the
    current shell session, useful for reviewing exactly what steps were
    taken during a task like this one.
