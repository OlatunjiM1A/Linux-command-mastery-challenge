# Day 13 Commands — APT Package Management (Debian/Ubuntu)

1. **apt update** — Refreshes the local package index by pulling the
   latest list of available packages and versions from configured
   repositories. Doesn't install or upgrade anything itself — just
   updates what apt knows is available.

2. **apt upgrade** — Installs available newer versions of all currently
   installed packages, based on the index from the last apt update.

3. **apt full-upgrade** — Like upgrade, but also allowed to remove
   packages if that's necessary to resolve dependency changes during
   the upgrade.

4. **apt install** — Installs a new package by name, pulling in any
   required dependencies automatically.

5. **apt remove** — Uninstalls a package's program files, but leaves its
   configuration files behind on the system.

6. **apt purge** — Uninstalls a package and also removes its
   configuration files, for a fully clean removal.

7. **apt autoremove** — Removes packages that were installed as
   dependencies for something else but are no longer needed by anything
   currently installed.

8. **apt search** — Searches package names and descriptions in the
   index for a keyword, helping you find the right package name before
   installing.

9. **apt show** — Displays detailed information about a package —
   version, dependencies, description, size — without installing it.

10. **dpkg -l / dpkg -L** — dpkg -l lists all packages currently
    installed on the system. dpkg -L lists every file that a specific
    installed package placed on the system.
