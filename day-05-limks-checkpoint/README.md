# Day 5 — Paths, Links & Tree Structures

## Phase 1 — File Navigation & Filesystem Mastery | Day 5 of 30

## Checkpoint

Today is the Phase 1 checkpoint.

I practiced filesystem paths, directory trees, hard links, symbolic links, path manipulation, directory stacks, and sorting files by modification time.

## Commands Covered

See [commands.md](commands.md) for the complete list and my explanations.

## Checkpoint Drill

I created a symbolic link to a configuration file, resolved its real path, displayed a two-level tree of `/etc`, and practiced explaining the difference between hard links and symbolic links.

## What I Learned

I learned that hard links and symbolic links are not the same. A hard link directly references the same underlying file through the inode, while a symbolic link points to the path of another file.


## What Surprised Me

What surprised me was that the hard link and the original file had exactly the same inode number, while the symbolic link had a different inode and clearly showed what file it was pointing to. I also initially got an error when creating the configuration-file link because I had not created the `day5-practice` directory yet.

## Evidence

See the screenshots in the `evidence/` folder.

## LinkedIn Article

[Day 5 — Phase 1 Checkpoint][(MY-LINKEDIN-ARTICLE-LINK)
](./(https://lnkd.in/p/eVfksTg4)/.)

## Related

Previous day: [Day 4](../day-04-filesystem-search/)

Next day: [Day 6](../day-06-permissions/)
