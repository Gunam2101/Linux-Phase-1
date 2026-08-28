# Day 3 - Permissions & Ownership

## Objective

To understand Linux file permissions, ownership, groups, umask, shared directories, read-only directories, and script permissions.

## Topics Practiced

- File permissions
- chmod
- Numeric permissions
- chown
- chgrp
- umask
- Shared directory
- Read-only directory
- Script permission break and fix

## Permission Values

r = 4
w = 2
x = 1

644 = rw-r--r--
600 = rw-------
755 = rwxr-xr-x

## Ownership

User:
gunam

UID:
1000

Primary Group:
gunam

Additional group used:
projectgrp

## Shared Directory

Directory:
~/bin/shared

Permission:
770

Owner:
gunam

Group:
projectgrp

## Read-Only Directory

Directory:
~/bin/readonly

Permission:
555

## Umask

Current umask:
0022

Symbolic representation:
u=rwx,g=rx,o=rx

## Script Permission Test

Script:
test-script.sh

The execute permission was removed using chmod u-x.

Result:
Permission denied

The execute permission was restored using chmod u+x.

Result:
Linux Day 3 Permission Test

## Status

Day 3 - Permissions & Ownership completed successfully.
