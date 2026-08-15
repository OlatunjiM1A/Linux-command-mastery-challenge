# Day 5 — Phase 1 Checkpoint Drill

## Task

Create a symbolic link to a configuration file, resolve its real path,
display a two-level tree of `/etc`, and explain the difference between
a hard link and a symbolic link.

## Configuration File Used

`/etc/adduser.conf`

## Commands I Ran

```bash
ln -s `/etc/adduser.conf` ~/day5-practice/config-link
readlink ~/day5-practice/config-link[link]
realpath ~/day5-practice/config-link
tree /etc -L 2  km l;l
