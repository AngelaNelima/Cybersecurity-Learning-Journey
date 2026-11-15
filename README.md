# Cybersecurity-Learning-Journey
# Learning Roadmap

01-Networking/
## theory
- got to learn networking from Cisco Academy
## Practical  
- Cisco Packettracer
## Understanding Linux Commands
- Common ls Linux Flags

ls	List files and directories
ls -l	Long listing / detailed information
ls -a	Include hidden files
ls -r	Reverse the sorting order
ls -h	Human-readable sizes, usually with -l
ls -k	Display sizes in 1024-byte blocks, when using -l
ls -R	Recursively list subdirectories
ls -t	Sort by modification time
ls -s Sort by file size

You can combine compatible short options. ie: ls -lah is equivalent to ls -l -a -h

### Permissions Breakdown
- (-)Type, (rwx)Owner, (r-x)Group, (r--)Others
- r=read, w=write, x=execute, -=permission not granted
     #### Why Permission Management Matters in Cybersecurity
  These commands become useful when:
   - Investigating suspicious files
   - Checking executable scripts
   - I dentifying files accessible to other users
   - Auditing permissions
   - Inspecting directories during incident response
   - Understanding Linux Previledge escalation vulnerabilities
