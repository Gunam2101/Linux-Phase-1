# Day 5 - Processes & System Monitoring

## Objective

To understand Linux processes, process IDs, background jobs, signals, and process priority.

## Commands Practiced

- ps
- ps -f
- ps aux
- pgrep
- kill
- jobs
- bg
- fg
- Ctrl+Z
- nice
- renice

## ps

`ps` displays running processes.

`ps -f` displays detailed process information.

`ps aux` displays processes from all users.

## Process Identification

PID means Process ID.

PPID means Parent Process ID.

`pgrep` was used to find process IDs by process name.

## Background Jobs

A background process was created using:

sleep 300 &

The `jobs` command was used to view background jobs.

## Foreground and Background

`fg` brings a background job to the foreground.

`Ctrl+Z` stops a foreground process.

`bg` resumes a stopped process in the background.

## Process Termination

The test processes were safely terminated using:

kill PID

## Nice

A test process was started using:

nice -n 10 sleep 300 &

The initial nice value was:

NI = 10

## Renice

The running process priority was changed using:

renice 15 -p PID

The nice value changed:

10 → 15

## Safety

Only test `sleep` processes created during the practical were terminated.

System processes were not terminated.

## Status

Day 5 - Processes & System Monitoring completed successfully.
