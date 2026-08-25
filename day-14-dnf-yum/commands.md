# Day 14 Commands — DNF/YUM & Alternative Installs

1. **dnf update** — Refreshes package metadata and upgrades installed
   packages to their latest available versions, similar in role to
   apt update combined with apt upgrade.

2. **dnf install** — Installs a new package by name, pulling in
   required dependencies automatically. The RHEL/Fedora/Amazon Linux
   equivalent of apt install.

3. **dnf remove** — Uninstalls a package from the system, along with
   dependencies that are no longer needed by anything else.

4. **dnf search** — Searches package names and descriptions for a
   keyword, helping locate the correct package name before installing.

5. **yum install** — The older package manager that dnf replaced on
   most RHEL-based systems. Functionally very similar to dnf install,
   and yum still works as an alias on many modern systems.

6. **rpm -qa** — Queries and lists all packages currently installed on
   the system, using the RPM package database directly rather than
   going through dnf.

7. **snap install** — Installs a package using Snap, a
   distribution-independent package format that bundles its own
   dependencies, working across many different Linux distros.

8. **add-apt-repository** — Adds a new external repository to apt's
   sources list on Debian/Ubuntu systems, so apt can install packages
   not available in the default repositories.

9. **dpkg -i** — Installs a package directly from a local .deb file,
   bypassing the repository system entirely. Useful for software
   distributed as a standalone file rather than through a repo.

10. **pip / npm install** — Language-specific package managers: pip
    installs Python packages, npm installs Node.js packages. Separate
    from the OS-level package manager, since these operate at the
    application/language level instead of the system level.
