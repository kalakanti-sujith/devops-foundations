# Linux Navigation – Why it matters in real systems

When logging into a Linux server, the first step is always to confirm the current working directory.

*Command:
pwd

Reason:
In production environments, deleting or modifying files from the wrong directory can cause application outage or data loss.

Example scenario:
Suppose logs are stored inside:
/var/log/app/

If an engineer mistakenly runs a delete command from the root or wrong folder, it can remove critical system files instead of logs.

To avoid this:
1. Always run "pwd" to confirm location
2. Use "ls" to verify files in the directory
3. Then perform operations

Commands used:
- pwd → shows current directory
- ls → lists files and folders
- cd → used to move safely between directories

Learning outcome:
Linux navigation is not just basic knowledge.  
It is a safety practice to prevent production incidents.

