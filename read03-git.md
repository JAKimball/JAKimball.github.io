# Lab 03: Revisions and the Cloud

## Version Control

A Version Control System (VCS) is a system that manages multiple versions of files in a project and allows tracking of modifications and the possibility to revert to previous versions of files or projects.

### Local Version Control

Years ago programmers created Local Version Control Systems.  These entailed a single local database for verion control.

### Centralized Version Control

Centralized Version Control Systems (CVCS) allowed for collaboration within a developer team on individual files or sets off files.  The CVCS involved a central server storing all changes and file versions.

### Distributed Version Control

Distributed version control systems (DVCS) address the issue of the server as a single point of failure in a CVCS.  To prevent catastrophic loss. a DVCS allows clients to create mirror repositories.

## What is Git?

Git is...

### Snapshots

... A DVCS that stores data in a file system made up of snapshots.  Each *commit* operation creates a snapshot of the changed files for that version as well as references to unchanged versions.

### Local Operations

For expediency Git mostly relies on local operations.  Because a project's history resides on the local system, the need to fetch history information from the central server is eliminated, allowing for work to continue on a project even when offline.

### Tracking Changes

All file and directory changes are tracked by Git, and Git will always detect file corruption or data loss.

### Loss of Data

Git is designed to minimize the possibility of irreversible data loss.  It makes it extremely difficult for committed snapshots to be lost.

### States

The three main states of files in Git.

- Committed - Securely stored in a local database
- Modified - File changed but not committed
- Staged - File's changed version is flagged to be committed in the next snapshot

## Getting Help

Three ways to get help on Git commands (where `command` is the command):

```bash
git help command
git command --help
man git-command
```

## Setting up a Git Repository

### Importing

```bash
$ git init
```

```bash
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”
```

### Cloning

```bash
$ git clone https://github.com/test
```

```bash
$ git clone https://github.com/test mydirectory
```


## Workflow

### The Life Cycle of File Status

![The Life Cycle of File Status
](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)

### Check File Status

```bash
$ git status
```

### Tracking and Staging a New File

```bash
$ git add filename
```

```bash
$ git add *
```

### Committing a File

```bash
$ git commit -m “made change x,y,z”
```

### Committing All Changes

```bash
$ git commit -a
```

### Pushing Changes

```bash
$ git push -u origin master
```

## Remote Repositories

```bash
$ cd example
$ git remote -v
remote1 https://github.com/remote1/example (fetch)
remote1 https://github.com/remote1/example (push)
remote2 https://github.com/remote2/example (fetch)
remote2 https://github.com/remote2/example (push)
remote3 https://github.com/remote3/example (fetch)
remote3 https://github.com/remote3/example (push)
```

[Return Home](/)