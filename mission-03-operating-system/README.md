# Mission 3 - Understand the operating system

## 1. Task / objective
To explore my operating system, look at running processes, understand paths and file permissions, and describe what an operating system is responsible for.

## 2. Work completed
I checked my macOS version, account, storage and a snapshot of system activity. I looked at running processes, compared absolute and relative paths, read file permissions, and explained the main responsibilities of an operating system.

## 3. Commands / tools used
sw_vers, whoami, df -h, top, ps aux, pwd, cd, ls -l. I used the Terminal in VS Code.

## Task 3.1 - Explore my operating system

| Information explored | What it tells you | Your observation (privacy-safe) |
|---|---|---|
| Operating system / system details (sw_vers) | The name and version of the operating system I am running | macOS, version 27.2.1 (build 26B131) |
| Current account identity (whoami) | Which user account is currently active | The account name, which I have redacted: [redacted] |
| Available and used storage (df -h) | How much disk space exists, how much is used and how much is free | About 926Gi total, 87Gi used and 814Gi available, so around 10% of the disk is used |
| System activity snapshot (top -l 1 \| head -n 12) | What the computer is doing right now, like memory use and disk and network activity | The snapshot showed memory use of about 15G used and about 528M unused, plus totals for network packets and disk reads and writes. I did not copy the process list because it can show my username. |

## Task 3.2 - Understand processes
- A process is a program that is currently running on the computer.
- The PID column is the process ID, a unique number the operating system gives each running process so it can keep track of it.
- Two processes I saw running:  Brave Browser and Visual Studio Code. These are applications running on my computer, and each has its own process ID (PID).

## Task 3.3 - Paths and permissions
- Absolute vs relative path: an absolute path starts from the top of the file system, like /Users/[redacted]/digital-detective-8030/mission-03-operating-system. A relative path starts from where I am now, like ../mission-02-terminal. When I used cd .., the location shown by pwd changed to the parent folder.
- Permissions: The permission string rw-r--r-- means that the owner has read and write permissions, while the group and other users have only read permission. The owner can modify the file, but the others cannot.

## Task 3.4 - Operating system responsibilities

| OS responsibility | Your explanation | Example |
|---|---|---|
| Process management | It decides which programs get to use the CPU and when, so many programs can run together. | Brave, VS Code and Terminal were all running at the same time on my laptop. |
| Memory management | It gives each running program some memory to work in and takes it back when the program closes. | The top command showed how much of my memory was used and how much was unused. |
| Device management | It controls hardware like the keyboard, screen, speakers and storage so programs can use them. | When I type, the OS passes the key presses from the keyboard to the app I am using. |
| File management | It keeps track of files and folders, where they are stored, and lets me create, copy, move and delete them. | In Mission 2 I used mkdir, cp and mv to create, copy and rename files. |
| User interface / shell | It gives me a way to give instructions to the computer, using the desktop or the Terminal. | Typing ls in the Terminal to list the files in a folder. |
| Security and permissions | It controls who can read, change or run files and protects user accounts. | The permission string rw-r--r-- showed that only the owner can change the file. |

## 4. My understanding
An operating system manages the computer's hardware and software and allows different applications to work together. Through this mission, I learned how to check system information, monitor running processes, navigate directories and understand file permissions using Terminal commands.

## 5. Difficulties faced
No major difficulties faced.

## 6. How I resolved them
Not applicable

## 7. Evidence / files
- mission-03-operating-system/README.md – Contains the completed tasks, command explanations, observations and OS responsibilities table.

## 8. Commit details
- Commit message: "Document operating system and file management"
- The completed Mission 3 README was committed and pushed to GitHub. The updated file and commit are visible in the repository.