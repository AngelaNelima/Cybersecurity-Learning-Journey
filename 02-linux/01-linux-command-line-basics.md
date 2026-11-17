## 1. Introduction

The Linux command-line interface (CLI) allows users to interact with the operating system by entering commands into a terminal.

It provides direct access to filesystem operations, system information, administrative functions and network utilities.

Understanding the command line is important in cybersecurity because many security tools and system administration activities rely on terminal-based operations.

## 2. Understanding Linux Commands

A Linux command is an instruction entered into the terminal to perform a particular operation.

For example:

ls

The command displays files and directories in the current working directory.

Commands can also accept options, commonly called flags, which modify their behaviour.

## 3. Understanding the ls Command

The ls command lists files and directories.

Common options

ls  Lists files and directories

ls -l Displays detailed file information

ls -a Displays hidden files

ls -r Reverses the sorting order

ls -h Displays human-readable sizes when used with -l

ls -k Uses 1024-byte units for size reporting in long format

ls -R Lists contents recursively

ls -t Sorts by modification time

ls -S Sorts by file size

ls -lh Displays detailed information with readable sizes

ls -la Displays hidden files in long format

ls -lah Combines long format, hidden files and readable sizes

## 4. Understanding Command Flags

Flags modify how commands execute.

For example:

ls -lah

This combines:

-l: Long listing format.

-a: Includes hidden files.

-h: Displays file sizes in human-readable units.

Understanding flags makes it possible to use commands more efficiently.

## 5. Understanding Long Listing Output

When executing:

ls -l

The terminal displays information about files, including permissions, ownership, file size and modification date.

Example:

-rwxr-xr-- 1 angie angie 2048 Nov 17 10:30 script.sh

The permission section is:

-rwxr-xr--

It represents:

File type

Owner permissions

Group permissions

Other users' permissions

The permission symbols include:

r - Read

w - Write

x - Execute

- Permission not granted

## 6. Hidden Files

Files beginning with a dot (.) are hidden by default when using the normal ls command.

To display them:

ls -a

Examples include:

.bashrc

.profile

.ssh

Some hidden files contain important user and system configuration information.

## 7. Practical Exercise

I explored the behaviour of different ls options using the following commands:

ls
ls -l
ls -a
ls -lh
ls -lah

The objective was to understand how each option changes the information displayed in the terminal.

## 8. Cybersecurity Relevance

Understanding Linux file listings is useful when:

Inspecting files and directories.

Identifying hidden configuration files.

Reviewing file ownership and permissions.

Conducting basic system enumeration.

Investigating potentially exposed files.

## 9. Key Takeaways

Linux commands instruct the operating system to perform specific operations.

Flags modify command behaviour.

ls displays directory contents.

Hidden files begin with a dot.

Long listing format provides useful information about permissions and ownership.

10. Learning Status

Completed: Linux command-line fundamentals and common ls options.
