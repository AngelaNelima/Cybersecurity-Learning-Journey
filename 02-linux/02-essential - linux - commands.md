## Essential Linux Commands

### 1. Introduction

Linux provides commands for navigating directories, managing files, searching information, controlling permissions, monitoring processes and inspecting network configurations.

These commands are important for everyday Linux usage and provide a foundation for cybersecurity activities.

### 2. Linux Filesystem Structure

Linux uses a hierarchical filesystem that begins at the root directory /.

Important directories include:

/ Root of the filesystem

/home Users' personal directories

/etc System configuration files

/var Variable data, including logs

/tmp Temporary files

/usr Applications and system utilities

/root Root user's home directory

### 3. Directory Navigation

pwd Displays the current working directory.

cd Changes the current directory.

cd Documents
cd ..
cd ~
cd -

cd .. moves one directory up.

cd ~ moves to the home directory.

cd - returns to the previous directory.

mkdir Creates a directory.

tree Displays directories and files in a tree structure.

### 4. File Management

touch Creates an empty file or updates its timestamps.

i.e: touch notes.txt

cat Displays file contents.

i.e cat notes.txt

less Views files page by page.

i.e less notes.txt

Press q to exit.

cp Copies files.

cp notes.txt backup.txt

mv Moves or renames files.

i.e mv notes.txt new-notes.txt

echo Displays or writes text.

i.e echo "Learning Linux" > notes.txt

The > operator overwrites existing content.

The >> operator appends content.

echo "Cybersecurity journey" >> notes.txt

### 5. Searching and Filtering

find Searches for files and directories.

i.e find . -name "*.log"

Finds files ending in .log under the current directory.

find . -mtime -1

Finds files modified within approximately the last 24 hours.

grep Searches for specific text within files.

i.e grep "failed" auth.log

Useful options:

grep -i "failed" auth.log
grep -r "password" .

-i: Ignores case sensitivity.

-r: Searches recursively.

These commands are useful when analysing logs and searching for specific patterns.

### 6. Permissions and Ownership

chmo Changes file permissions.

chmod 755 script.sh
chmod 644 notes.txt
chmod 600 private.txt

Numeric permission values:

7 Read, write and execute

6 Read and write

5 Read and execute

4 Read only

0 No permissions

The three digits represent the owner, group and others respectively.

chown Changes file ownership.

i.e sudo chown angie notes.txt

Changes the owner.

sudo chown angie:angie notes.txt

Changes the owner and group.

### 7. User Identification

whoami Displays the current username.

whoami id

Displays user ID, group ID and group membership information.

id These commands help identify the account executing commands and its group memberships.

### 8. Administrative Privileges

sudo Allows an authorised user to execute commands with elevated privileges.

Example:

sudo apt update

Administrative privileges should be used carefully because they allow changes to important system configurations.

### 9. Process Management

ps Displays information about running processes.

ps aux Search for a process:

ps aux | grep firefox

kill Sends a signal to a process.

kill PID The default signal requests graceful termination.

Always identify the correct process before terminating it.

### 10. Basic Networking Commands

ip addr Displays network interfaces and assigned IP addresses.

ip route Displays the routing table.

ping Tests network reachability.

ss Displays socket information.

curl Requests information from a URL.

i.e curl -I https://example.com

The -I option requests HTTP response headers.

### 11. Cybersecurity Relevance

ls -lah  Inspect files and permissions

find  Locate files during system inspection

grep  Search logs and configuration files

chmod  Manage file permissions

whoami  Identify the current user

id Inspect user and group memberships

ps aux Inspect running processes

ip addr Identify network interfaces

ip route Inspect network routing

ss -tuln  Inspect listening services

curl -I  Inspect HTTP response headers

### 12. Security Considerations

Understand commands before executing them.

Use sudo carefully.

Avoid unnecessary changes to system files.

Avoid overly permissive settings such as chmod 777.

Be cautious with destructive commands such as rm.

Only investigate systems you own or have permission to access.

### 13. Key Takeaways

Linux commands provide tools for filesystem navigation, file management, searching, permissions, process management and networking.

Understanding these commands provides an important foundation for system administration and cybersecurity.

### 14. Learning Status

Completed: Essential Linux commands and introductory system inspection.

Next topic: Linux users, groups, file permissions and privilege management.
