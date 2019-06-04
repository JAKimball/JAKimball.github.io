# Read 02: The Coder's Computer (The Text Editor, Files, and the Command Line Interface)

## The Text Editor

At its core a text editor is a program for editing editing plain text files.  It may be installed on your computer or accessed online through a web browser.

### Features to look for in a text editor

- Code completion
- Syntax highlighting
- A variety of color themes to reduce eye fatigue
- A good selection of extensions

Code completion allows you to start typing and will display suggestions base on what was typed in order to save time and reduce typos.

Emmet is a feature of many editors (built in, or by extension) that allows HTML and CSS to be written mre efficiently by allowing typing in a shorthand in order to produce the HTML and CSS code.

Syntax highlighting colorizes the text according to the syntax of the programming language of the text file making it much easier to read.

### Text Editors Included With the OS

- Mac - Text Edit
- Windows - Notepad
- Linus - Depends on the Linux distribution...
  - Gedit

These are very basic editors and don't include many features that would help you code more efficiently.

### Third-Party Options

- NotePad++ - Free - For Windows only
- TextWrangler/BB Edit - Mac only
- Visual Studio Code - Windows, Mac, and Linux - Made by Microsoft - Very popular among web developers.
- Atom - Windows, Mac, and Linux - Made by GitHub
- Brackets - Windows, Mac, and Linux - Made by Adobe
- Sublime Text - Premium software ($70)

### The Difference Between Text Editors and IDEs

IDE stands for Integrated Development Environment.  An IDE is a suite of software combined and includes a text editor, file manager, and debugger all in one package.

The following are my notes from the excellent [Linux Tutorial](https://ryanstutorials.net/linuxtutorial/) by Ryan Chadwick of [Ryan's Tutorials](https://ryanstutorials.net).

## The Command Line

Simply stated, a Unix shell or Command Line Interface (CLI) works like a Read-Evaluate-Print-Loop or **REPL**.

### How to open a terminal

- Mac - Find the Terminal program under Applications -> Utilities.  Entering `command + space` and typing "Terminal" will get it quickly.
- Linux - Usually in Applications -> System or Applications -> Utilities.  You may also be able to *right-click* on the desktop and select the option "Open in terminal".  This will depend on your Linux distribution.
- Windows - To connect remotely to another machine you will need an SSH client such as Putty.  Alternatively you can use the Windows Subsystem for Linux (WSL).  This can be invoked a number of different ways.  After the linux distribution is installed from the Windows Store, the terminal can be launched by finding it in the Windows start menu, or by hitting the windows start key and entering the name of the distribution.

## Key Commands for Navigating the File System

`pwd` stands for Print Working Directory.  It outputs the current working directory.

`ls` is short for list.  It lists the files in the current directory.  It can also take optional arguments indicating options and the relative or absolute location to list.

### Absolute and Relative Paths

When specifying a directory or a file, there are two types of paths we can use, absolute and relative.  The linux file system is a hierarchical structure with the root of the structure, the **root** directory, denoted by a single slash (`/`).

Absolute paths specify locations relative to the root directory.  They always begin with a forward slash (`/`).

Relative paths specify locations relative to the current working directory.  They do not begin with a slash.

`~` - The tilde is a shortcut for the users home directory.

`.` - The period refers to the current directory.

`..` - A pair of periods refer to the parent directory.  This can be used several times to step up the hierarchy. For example `../../` refers to the parent of the parent of the current directory.

`cd` - Stands for change directory.  This changes the current working directory of the shell to the directory indicated in the command argument.  Running `cd` without and argument will take you back to you home directory.

## More About Files

In linux everything is a file.

Linux does not use filename extensions to indicate the type of file.  The command `file [path]` can be used to determine the type of a file by looking into the content to determine the type.

Linux file names are case sensitive.

Spaces in file and directory names are valid, but quotes or escape characters must be used so that the names are interpreted correctly.

```bash
> cd 'Holiday Photos'
```

or

```bash
> cd Holiday\ Photos
```

## Hidden Files and Directories

If a file or directory name begins with a period then it is considered to be hidden and will not show in a directory listing unless the `-a` option to the `ls` command is used.

[Return Home](/)


