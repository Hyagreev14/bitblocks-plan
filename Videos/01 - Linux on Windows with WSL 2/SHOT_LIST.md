# Video 01 — Shot List

This list describes the visuals to capture for the script. Capture only what is needed; do not record private information or leave sensitive windows visible.

## Capture setup

- Use the actual Windows + WSL 2 + Ubuntu environment for the live demonstration.
- The creator's PC already has WSL installed. Do not uninstall, reset, or reinstall it to manufacture fresh-install footage.
- Prepare a clean installation walkthrough graphic showing the standard fresh-PC steps. Clearly label it as a walkthrough, not a live installation.
- Close unrelated apps, private chats, email, personal browser tabs, and notifications.
- Use a clean terminal with a readable font size.
- Prepare a dedicated demo folder and verify the commands before recording.
- Hide or crop Windows account names, personal folder paths, device names, and unrelated file listings.
- Record at a consistent resolution and frame rate supported by the capture setup.
- Capture separate takes for important commands so mistakes can be removed cleanly.

## Shot list

| ID | Script section | Capture | Notes |
|---|---|---|---|
| S01 | Hook | Windows desktop, open Ubuntu terminal | Begin with a clean, confident transition |
| S02 | Hook | Terminal with a few commands | Fast montage; don't make commands unreadable |
| S03 | Problem | Windows desktop and Linux terminal side by side | Communicate both environments on one PC |
| S04 | What is WSL | Clean title card: Windows Subsystem for Linux | Spell out the name |
| S05 | What is WSL | Simple Windows → WSL → Ubuntu diagram | Avoid implying WSL is a separate full desktop OS |
| S06 | WSL 2 architecture | Diagram of Windows host, managed lightweight VM, Linux kernel, distribution | Label the VM accurately |
| S07 | Before installation | Compatibility card: Windows 11, or Windows 10 version 2004 / build 19041 or later | Show winver as the way to check; don't imply all Windows versions use the same path |
| S08 | Installation walkthrough | Clean PowerShell command graphic showing wsl --install | Label “fresh supported Windows setup”; do not present as live execution |
| S09 | Installation walkthrough | Three-step graphic: Administrator PowerShell → command → restart | Keep text large and simple |
| S10 | First launch | Ubuntu first-launch / account setup illustration | Never show a real password being entered |
| S11 | Verification | PowerShell running wsl --list --verbose | Show the actual creator setup; highlight VERSION 2 |
| S12 | WSL status | PowerShell running wsl --status | Capture actual output |
| S13 | Ubuntu terminal | Open Ubuntu terminal | Keep prompt readable; hide username if visible |
| S14 | Kernel | Run uname -r | Capture actual output |
| S15 | Current directory | Run pwd | Avoid showing personal paths if possible |
| S16 | Demo folder | Run mkdir -p ~/bitblock-wsl-demo and cd | Show command clearly |
| S17 | Demo file | Run the printf command | Show the exact command |
| S18 | Read file | Run cat hello.txt | Hold output long enough to read |
| S19 | Windows integration | Run explorer.exe . and show folder | Crop personal path from Explorer address bar |
| S20 | Benefits | Terminal, code editor, documentation or project view | Only show apps that are actually installed and relevant |
| S21 | Limitations | Clean graphic with 3 short points | Resources, filesystem location, not ideal for every use |
| S22 | Closing | Windows desktop with Ubuntu terminal | Calm final shot |
| S23 | End card | BitBlock logo and tagline | Leave enough time to read |

## Optional B-roll

- A close-up of the Ubuntu app launch.
- A short screen capture switching between a Windows application and Ubuntu.
- A simple animation of a command being entered and output appearing.
- A clean diagram illustrating the managed WSL 2 virtual machine.
- A simple restart/first-launch transition for the installation walkthrough.

Do not use unrelated stock footage just to fill time. Do not show a simulated installer as though it were live footage.

## On-screen text

Use short labels only:
- WINDOWS + LINUX
- WINDOWS SUBSYSTEM FOR LINUX
- WSL 2
- LINUX KERNEL
- UBUNTU
- WINDOWS 11 / WINDOWS 10 2004+
- POWERSHELL AS ADMINISTRATOR
- wsl --install
- RESTART
- CREATE LINUX USER
- VERIFY: VERSION 2

## Capture verification

Before the final recording:
1. Run every command used on the actual creator machine once without recording.
2. Confirm the distribution is WSL 2.
3. Confirm the demo folder is created under the Linux home directory.
4. Confirm the file contents are correct.
5. Confirm Windows Explorer opens the current directory.
6. Rehearse the transition between PowerShell and Ubuntu.
7. Check that no private details are visible.
8. Check that the installation walkthrough graphic matches Microsoft's current instructions.
9. Clearly distinguish the fresh-install walkthrough from the creator's existing WSL setup.
