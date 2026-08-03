## taskwarrior

A task manager for the command line.

taskwarrior keeps a to-do list in a local database with priorities, projects, due dates, and dependencies. No server, no GUI, no web app.

### Your tasks as data

```
task add "write report" project:wiki due:tomorrow
task list project:wiki
task 12 done
```

The whole system is commands that read and write one local file. Export to JSON or JSONLines for scripts and backups.

### Filtering is a query language

taskwarrior filters are flexible:

```
task overdue
task project:work due.before:today
task +urgent
```

Reports are plain text, and any filter can become a standing report.

### The Unix fit

taskwarrior is a single binary with no daemon by default, and it composes with cron, notify-send, and shell hooks.

A task list should live where you work, not in an app that demands your attention.

### Scriptable to the core

Everything is a command, so everything scripts.

It is the task manager for a terminal-centric workflow, and it stores its data in formats you can read.
