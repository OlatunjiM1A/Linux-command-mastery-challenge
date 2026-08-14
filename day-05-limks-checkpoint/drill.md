# Day 5 — Phase 1 Checkpoint Drill

## Task

Create a symbolic link to a configuration file, resolve its real path,
display a two-level tree of `/etc`, and explain the difference between
a hard link and a symbolic link.

## Configuration File Used

[Write the config file you actually used.]

## Commands I Ran

```bash
ln -s [config-file] [link]
readlink [link]
realpath [link]
tree /etc -L 2  km l;l
