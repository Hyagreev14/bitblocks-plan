# Video 01 — How to Install Linux on Windows with WSL 2

<small>BitBlock · CODE. CREATE. EXPLORE.</small>

## Status

**Stage:** Planned — not recorded, edited, or published.

This folder is the working production package for BitBlock's first video. All footage, test results, timings, and final claims must reflect what is actually captured.

## The decision

**Chosen topic:** A beginner-friendly introduction to Windows Subsystem for Linux (WSL 2), a guided installation walkthrough for Ubuntu on a supported Windows PC, and a practical demonstration from the creator's existing Windows + Ubuntu environment.

**Working title:** How to Install Linux on Windows with WSL 2 (Beginner Guide)

**Format:** Explainer + guided installation walkthrough + practical demonstration.

**Target duration:** Approximately 9–11 minutes. This is a planning estimate, not a requirement.

**Audience:** Windows users curious about Linux, beginner developers, students, and people who want to try Linux without replacing Windows.

**Viewer promise:** By the end, viewers should understand what WSL 2 is, know the standard way to install it with Ubuntu on a supported Windows PC, know how to complete first launch and verify WSL 2, and have seen a few useful Linux commands.

## Why this is Video 01

- It introduces BitBlock through a useful, recognisable technology subject.
- It gives viewers a practical outcome, not just an explanation.
- The creator already has a real WSL 2 environment, so the demonstration can be grounded in actual experience.
- It does not depend on ATLAS being ready.
- It introduces Linux without suggesting that viewers must replace Windows.
- The standard installation path is short enough to include without turning the video into a full troubleshooting course.

## Scope

### Include

1. The problem this solves: wanting Linux tools while continuing to use Windows.
2. A plain-language explanation of WSL.
3. The important WSL 2 detail: it uses a real Linux kernel inside a lightweight, Windows-managed virtual machine.
4. A short explanation of how that differs from setting up a traditional VM or dual-booting.
5. The supported Windows versions for the simple installation command.
6. The standard fresh-install walkthrough: open PowerShell as Administrator, run **wsl --install**, and restart when prompted.
7. First launch of Ubuntu and creation of a Linux username and password.
8. Verification with **wsl --list --verbose**, checking that the distribution uses version 2.
9. A tour of the creator's actual Ubuntu terminal.
10. A few safe commands and a tiny file-creation demonstration inside the Linux home directory.
11. A balanced list of useful cases and limitations.
12. A short closing that invites viewers to follow BitBlock's technology experiments.

### Exclude

- Detailed manual installation for older Windows builds. Link to Microsoft's instructions instead.
- A long troubleshooting segment covering every possible installation error.
- A full Linux command-line course.
- Docker, Kubernetes, servers, or ATLAS. They would make the first video unfocused.
- Unsupported performance comparisons or claims that WSL is always better than a VM.
- A claim that WSL 2 is not a VM. It uses a managed lightweight VM; explain that accurately.
- A fixed promise about which future video will be uploaded next.

## Installation walkthrough

For the simple **wsl --install** path, Microsoft currently documents support for Windows 11 or Windows 10 version 2004 (Build 19041) or later.

On a fresh supported Windows PC:

1. Open PowerShell as Administrator.
2. Run **wsl --install**. Ubuntu is installed by default.
3. Restart if prompted.
4. Open Ubuntu from the Start menu and wait for first-time setup.
5. Create a Linux username and password. These are separate from the Windows account. Password characters do not appear while typing; that is normal.
6. In PowerShell, run **wsl --list --verbose** and check that Ubuntu shows version 2.

The command enables the required Windows components, installs the Linux kernel, sets WSL 2 as the default, and installs Ubuntu. The exact setup experience may vary with Windows and WSL versions.

**Recording honesty:** The creator's PC already has WSL installed. Do not uninstall, reset, or alter the working setup just to capture a fresh installation. Present the standard fresh-install steps with a clearly labelled command/step graphic, then show the creator's real existing setup and verification output. Do not present a graphic or recreated screen as a live installation.

For a different distribution, viewers can list available choices with **wsl --list --online** and install one with **wsl --install -d <DistroName>**. Keep this as a brief optional note, not a second tutorial.

## Demonstration environment

Use the creator's real environment, then verify details immediately before recording:
- Windows host.
- WSL 2.
- Ubuntu distribution.
- Current WSL and kernel details as displayed by the machine at recording time.

Do not hard-code versions into the narration until they have been checked on the recording machine. Avoid exposing Windows account names, personal paths, notifications, private tabs, tokens, or unrelated files.

## Demonstration commands

Run these in a prepared terminal and verify the output first:

PowerShell:
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

The demo creates one clearly named folder and one text file in the Linux home directory. It does not modify system configuration. The final command opens the current directory in Windows File Explorer; verify that it works in the recording environment. Do not show personal directory names in the address bar.

## Core story

**WSL gives Windows users a practical way to add a Linux environment without replacing their normal desktop. The video explains what it is, walks through the standard installation path, and then shows what using it looks like.**

Keep the story simple:
- What problem does it solve?
- What is it?
- What does WSL 2 actually run?
- How can a beginner install Ubuntu with it?
- How can they confirm it is working?
- What does it look like in practice?
- When is it useful, and what should viewers know before relying on it?

## Planned structure

See [SCRIPT.md](SCRIPT.md) for narration and [SHOT_LIST.md](SHOT_LIST.md) for capture instructions.

| Section | Approx. time | Purpose |
|---|---:|---|
| Hook | 0:00–0:25 | Promise Linux on Windows and a beginner installation walkthrough |
| The problem | 0:25–1:05 | Explain why someone might want both |
| What WSL is | 1:05–2:10 | Define WSL and WSL 2 |
| How WSL 2 works | 2:10–3:00 | Explain the managed lightweight VM |
| Before installation | 3:00–3:30 | Explain the supported Windows versions |
| Installation walkthrough | 3:30–4:45 | Show the command, restart, and default Ubuntu installation |
| First launch and verification | 4:45–5:45 | Create Linux credentials and confirm version 2 |
| Live demonstration | 5:45–7:45 | Show real terminal commands and a tiny file |
| Benefits and limitations | 7:45–9:20 | Set realistic expectations |
| Closing | 9:20–9:50 | Recap and invite viewers to subscribe |

Timings are placeholders. The final chapter timestamps must be generated from the completed edit.

## Production files

- [Narration script](SCRIPT.md)
- [Shot list](SHOT_LIST.md)
- [Editing plan](EDITING_PLAN.md)
- [Thumbnail brief](THUMBNAIL.md)
- [Publishing package](PUBLISHING.md)
- [Technical fact-check](FACT_CHECK.md)
- [Recording checklist](RECORDING_CHECKLIST.md)

## Production principles

- Use the creator's actual machine and actual results for the live demonstration.
- Be transparent that the installation sequence is a fresh-PC walkthrough, not a live reinstall on the creator's already-configured PC.
- Do not uninstall, reset, or disrupt the existing WSL setup to manufacture installation footage.
- Narration should sound natural, not like a formal lecture.
- Explain technical terms when first introduced.
- Use screen recordings, terminal captures, and simple diagrams; no face camera is required.
- Do not add music or effects that compete with the explanation.
- Keep the video focused. Do not turn it into a WSL troubleshooting marathon.
- If a command or feature behaves differently during recording, update the script to match reality.
- Keep all claims accurate and distinguish personal experience from general facts.

## Completion definition

This video is ready to publish only when:
- the final narration matches the recorded footage;
- all technical claims have been checked;
- the export has been watched from beginning to end;
- the title and thumbnail match the actual video;
- the description, chapters, captions, and links are checked;
- no credentials, private information, or unintended personal details appear;
- final duration and chapter timestamps are updated from the finished export.

**Current state: planning package updated to include installation. No recording or publication is claimed.**
