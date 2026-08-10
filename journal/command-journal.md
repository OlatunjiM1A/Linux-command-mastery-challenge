## Day 1 — File Navigation & Filesystem Mastery

1. pwd — prints the full path of the directory I'm currently in
2. ls — lists files and folders in the current directory
3. ls -l — long listing: shows permissions, owner, group, size, and last modified date
4. ls -a — shows all files including hidden ones (dotfiles like .bashrc)
5. ls -la — combines long format and hidden files in one view
6. ls -lh — long format but with human-readable sizes (e.g. 4.0K instead of 4096)
7. cd /var/log — moves into /var/log using its absolute path from root
8. cd .. — moves up one level to the parent directory
9. cd ~ — jumps straight back to my home directory regardless of where I am
10. cd - — jumps back to whichever directory I was just in before the last cd

**What surprised me:** I didn't realize that /var/log is also a directory 
`cd -` only remembers the *one* previous 
directory, not a full history — if I run it twice in a row it just toggles 
back and forth between two places instead of going further back.
juujnjub
