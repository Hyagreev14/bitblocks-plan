# Video 01 — Shot List

This list describes the visuals to capture for the script. Capture only what is needed; do not record private information or leave sensitive windows visible.

## Capture setup

- Use the actual Windows + WSL 2 + Ubuntu environment.
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
| S07 | WSL status | PowerShell running `wsl --status` | Capture actual output |
| S08 | Installed distributions | PowerShell running `wsl --list --verbose` | Show actual distro and WSL version; redact personal details |
| S09 | Ubuntu terminal | Open Ubuntu terminal | Keep prompt readable; hide username if visible |
| S10 | Kernel | Run `uname -r` | Capture actual output |
| S11 | Current directory | Run `pwd` | Avoid showing personal paths if possible |
| S12 | Demo folder | Run `mkdir -p ~/bitblock-wsl-demo` and `cd` | Show command clearly |
| S13 | Demo file | Run the `printf` command | Show the exact command |
| S14 | Read file | Run `cat hello.txt` | Hold output long enough to read |
| S15 | Windows integration | Run `explorer.exe .` and show folder | Crop personal path from Explorer address bar |
| S16 | Benefits | Terminal, code editor, documentation or project view | Only show apps that are actually installed and relevant |
| S17 | Limitations | Clean graphic with 3 short points | Resources, filesystem location, not ideal for every use |
| S18 | Closing | Windows desktop with Ubuntu terminal | Calm final shot |
| S19 | End card | BitBlock logo and tagline | Leave enough time to read |

## Optional B-roll

- A close-up of the Ubuntu app launch.
- A short screen capture switching between a Windows application and Ubuntu.
- A simple animation of a command being entered and output appearing.
- A clean diagram illustrating the managed WSL 2 virtual machine.

Do not use unrelated stock footage just to fill time.

## On-screen text

Use short labels only:
- WINDOWS + LINUX
- WINDOWS SUBSYSTEM FOR LINUX
- WSL 2
- LINUX KERNEL
- UBUNTU
- ONE PC, TWO ENVIRONMENTS

## Capture verification

Before the final recording:
1. Run every command once without recording.
2. Confirm the distribution is WSL 2.
3. Confirm the demo folder is created under the Linux home directory.
4. Confirm the file contents are correct.
5. Confirm Windows Explorer opens the current directory.
6. Rehearse the transition between PowerShell and Ubuntu.
7. Check that no private details are visible.
