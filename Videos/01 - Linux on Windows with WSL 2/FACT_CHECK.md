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

## Machine-specific checks before recording

Check these on the actual recording PC:

- [ ] `wsl --status` output.
- [ ] `wsl --list --verbose` shows the expected distribution and version.
- [ ] The Ubuntu terminal opens correctly.
- [ ] `uname -r` output is accurate.
- [ ] `pwd` output does not reveal personal information.
- [ ] The demo commands work exactly as written.
- [ ] `explorer.exe .` opens the current folder if this shot is kept.
- [ ] Any Windows, Ubuntu, WSL, or kernel version shown on screen is current and legible.

## Commands used in the video

PowerShell:

```powershell
wsl --status
wsl --list --verbose
```

Ubuntu:

```bash
uname -r
pwd
ls -la
cd ~
mkdir -p ~/bitblock-wsl-demo
cd ~/bitblock-wsl-demo
printf 'Hello from Linux on Windows!\n' > hello.txt
cat hello.txt
explorer.exe .
```

The demo writes only a new folder and text file under the Linux home directory. Verify that the folder does not already contain anything important before recording. Do not use destructive cleanup commands for this demonstration.

## Claims to avoid

- "WSL 2 is not a virtual machine."
- "WSL is exactly the same as installing Linux on bare metal."
- "WSL is always faster than a traditional VM."
- "WSL works on every Windows version."
- "Every Linux application works perfectly in WSL."
- "You never need a separate Linux machine if you have WSL."
- Any benchmark, resource-use figure, or performance percentage not measured in a reproducible test.

## Source priority

Use official Microsoft documentation for WSL behaviour and installation details. If the documentation changes before recording, re-check the relevant claims and update this file.

Official starting points:
- WSL overview: https://learn.microsoft.com/windows/wsl/about
- Compare WSL 1 and WSL 2: https://learn.microsoft.com/windows/wsl/compare-versions/
- WSL FAQ: https://learn.microsoft.com/windows/wsl/faq
- Install WSL: https://learn.microsoft.com/windows/wsl/install
