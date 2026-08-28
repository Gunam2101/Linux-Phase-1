# Day 2 - Filesystem & Navigation

## Objective

To understand the Linux filesystem hierarchy and practice navigation commands.

## Commands Practiced

### 1. pwd
Displays the current working directory.

Output:
`/home/gunam`

### 2. ls
Lists files and directories in the current directory.

### 3. ls -la
Displays visible and hidden files with detailed information.

### 4. cd /
Changes the current directory to the Linux root directory.

### 5. cd /home
Moves to the `/home` directory.

### 6. cd gunam
Moves to `/home/gunam`.

### 7. cd ..
Moves to the parent directory.

### 8. tree
Displays directories and files in a tree structure.

### 9. find
Used to search for files.

Command used:
`find /home/gunam -type f -name "*.log"`

Found:
`/home/gunam/.cache/ubuntu-pro/ubuntu-pro.log`

### 10. Find Top 5 Largest Files

Command used:
`find /home/gunam -type f -printf '%s %p\n' | sort -nr | head -5`

## Filesystem Map

/
├── bin
├── boot
├── dev
├── etc
├── home
│   ├── alice
│   ├── bob
│   ├── charlie
│   └── gunam
│       ├── bin
│       └── snap
├── lib
├── media
├── mnt
├── opt
├── proc
├── root
├── run
├── sbin
├── snap
├── srv
├── sys
├── tmp
├── usr
└── var

## Status

Day 2 - Filesystem & Navigation completed successfully.
