# Video 01 — Technical Fact-Check

This document separates verified general facts from details that must be checked on the creator's own machine.

## Core claims

### 1. What WSL does

**Claim:** Windows Subsystem for Linux lets users run a Linux environment on Windows, including Linux distributions and command-line tools.

**Status:** Supported by official Microsoft documentation.

**Source:** https://learn.microsoft.com/windows/wsl/about

### 2. What WSL 2 uses

**Claim:** WSL 2 uses virtualization technology to run a Linux kernel inside a lightweight utility virtual machine managed by WSL.

**Status:** Supported by official Microsoft documentation.

**Source:** https://learn.microsoft.com/windows/wsl/about

**Wording caution:** Do not say "WSL 2 does not use a VM." It does use a virtual machine; Windows manages it, so the user does not have to manage a traditional VM in the usual way.

### 3. WSL 1 and WSL 2 differ

**Claim:** WSL 1 and WSL 2 have different architectures. WSL 2 includes a Linux kernel in a managed VM, while WSL 1 uses a different translation approach.

**Status:** Supported by official Microsoft documentation.

**Source:** https://learn.microsoft.com/windows/wsl/compare-versions/

**Wording caution:** Avoid saying one version is always faster or better. The best choice depends on the workflow, and filesystem performance differs between WSL 1 and WSL 2.

### 4. Windows and Linux integration

**Claim:** WSL allows users to work with Windows applications and Linux command-line tools on the same machine, and access Windows files from Linux.

**Status:** Supported by Microsoft's WSL overview and FAQ.

**Sources:**
- https://learn.microsoft.com/windows/wsl/about
- https://learn.microsoft.com/windows/wsl/faq

### 5. WSL is useful for development

**Claim:** WSL can be useful when tools or workflows expect Linux behaviour, such as Linux command-line utilities and development tools.

**Status:** Supported by Microsoft's FAQ and overview.

**Sources:**
- https://learn.microsoft.com/windows/wsl/faq
- https://learn.microsoft.com/windows/wsl/about

### 6. Project file location can affect performance

**Claim:** Performance can differ depending on whether Linux tools work with files stored in the Linux filesystem or the Windows filesystem.

**Status:** Supported by Microsoft's WSL version comparison guidance.

**Source:** https://learn.microsoft.com/windows/wsl/compare-versions/

**Wording caution:** Keep this short in the first video. Do not invent a benchmark or quote a speed multiplier.

### 7. Installing WSL with the standard command

**Claim:** The simple **wsl --install** path is documented for Windows 11 and Windows 10 version 2004 (Build 19041) or later.

**Status:** Supported by official Microsoft installation documentation.

**Source:** https://learn.microsoft.com/windows/wsl/install

**Important details to state accurately:**
- Open PowerShell or Windows Command Prompt as Administrator for the standard install instructions.
- On a fresh supported system, **wsl --install** enables the required WSL and Virtual Machine Platform components, installs the latest Linux kernel, sets WSL 2 as the default, and installs Ubuntu by default.
- A restart may be required; tell viewers to restart when prompted.
- On first launch, Ubuntu completes initial setup and asks the user to create a Linux username and password.
- The Linux account is separate from the Windows account.
- Password characters do not appear while typing in the terminal. This is expected behaviour, not a broken input field.
- **wsl --list --verbose** lists installed distributions and their WSL versions. Use it to verify that the Ubuntu entry shows version 2.
- **wsl --list --online** lists available distributions. **wsl --install -d <DistroName>** can install a named distribution.

**Wording cautions:**
- Do not imply that **wsl --install** works on every Windows version.
- Do not promise that every machine will have an identical setup experience.
- Microsoft notes that if WSL is already installed and **wsl --install** only displays help, viewers may need to list available distributions and install a distribution separately. Keep this as a brief note rather than a full troubleshooting section.
- Older Windows builds may require the manual installation procedure. Link to Microsoft's manual guide rather than improvising outdated steps.

## Machine-specific checks before recording

Check these on the actual recording PC:

- [ ] **wsl --status** output.
- [ ] **wsl --list --verbose** shows the expected distribution and version.
- [ ] The Ubuntu terminal opens correctly.
- [ ] **uname -r** output is accurate.
- [ ] **pwd** output does not reveal personal information.
- [ ] The demo commands work exactly as written.
- [ ] **explorer.exe .** opens the current folder if this shot is kept.
- [ ] Any Windows, Ubuntu, WSL, or kernel version shown on screen is current and legible.
- [ ] The fresh-install walkthrough graphic matches Microsoft's current installation instructions.

## Commands used in the video

Fresh supported Windows installation walkthrough:

~~~powershell
wsl --install
~~~

PowerShell verification on the creator's existing setup:

~~~powershell
wsl --status
wsl --list --verbose
~~~

Ubuntu:

~~~bash
uname -r
pwd
ls -la
cd ~
mkdir -p ~/bitblock-wsl-demo
cd ~/bitblock-wsl-demo
printf 'Hello from Linux on Windows!\n' > hello.txt
cat hello.txt
explorer.exe .
~~~

The demo writes only a new folder and text file under the Linux home directory. Verify that the folder does not already contain anything important before recording. Do not use destructive cleanup commands for this demonstration.

**Recording note:** The creator's computer already has WSL installed. Do not uninstall, reset, or reinstall it for footage. Show the fresh-install steps as a labelled walkthrough graphic, then show real output from the existing setup. Never present recreated output as live installer output.

## Claims to avoid

- "WSL 2 is not a virtual machine."
- "WSL is exactly the same as installing Linux on bare metal."
- "WSL is always faster than a traditional VM."
- "WSL works on every Windows version."
- "Every Linux application works perfectly in WSL."
- "You never need a separate Linux machine if you have WSL."
- Any benchmark, resource-use figure, or performance percentage not measured in a reproducible test.
- Any claim that the creator performed a fresh installation on camera when the footage is a graphic walkthrough.

## Source priority

Use official Microsoft documentation for WSL behaviour and installation details. If the documentation changes before recording, re-check the relevant claims and update this file.

Official starting points:
- Install WSL: https://learn.microsoft.com/windows/wsl/install
- Set up a WSL development environment: https://learn.microsoft.com/windows/wsl/setup/environment
- Basic WSL commands: https://learn.microsoft.com/windows/wsl/basic-commands
- WSL overview: https://learn.microsoft.com/windows/wsl/about
- Compare WSL 1 and WSL 2: https://learn.microsoft.com/windows/wsl/compare-versions/
- WSL FAQ: https://learn.microsoft.com/windows/wsl/faq
- Manual installation for older Windows versions: https://learn.microsoft.com/windows/wsl/install-manual
