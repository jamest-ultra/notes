---
tags:
  - How_to_guide
---
# Description

ncdu (NCurses Disk Usage) is a disk utility for Unix systems. Its name refers to its similar purpose to the du utility, but ncdu uses a text-based user interface under the curses programming library. Users can navigate the list using the arrow keys and delete files that are taking up too much space by pressing the 'd' key. Version 1.09 and later can export the file listing in JSON format.

--- 
# How to run ncdu scoped to just Linux.

```bash
sudo ncdu / --exclude /mnt
```

