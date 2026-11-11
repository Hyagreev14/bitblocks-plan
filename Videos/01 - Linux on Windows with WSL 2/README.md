# Video 01 — Linux on Windows: What Is WSL 2 and Why Use It?

<small>BitBlock · CODE. CREATE. EXPLORE.</small>

## Status

**Stage:** Planned — not recorded, edited, or published.

This folder is the working production package for BitBlock's first video. The creator should review and approve the plan before recording. All footage, test results, timings, and final claims must reflect what is actually captured.

## The decision

**Chosen topic:** A beginner-friendly introduction to Windows Subsystem for Linux (WSL 2), supported by a real demonstration from the creator's Windows + Ubuntu environment.

**Working title:** Linux on Windows? What Is WSL 2 and Why Use It?

**Format:** Explainer + practical demonstration + small hands-on experiment.

**Target duration:** Approximately 7–10 minutes. This is a planning estimate, not a requirement.

**Audience:** Windows users curious about Linux, beginner developers, students, and people who want to understand why developers use WSL.

**Viewer promise:** By the end, viewers should understand what WSL 2 is, how it fits between Windows and Linux, what it is useful for, and what a simple Linux workflow inside Windows looks like.

## Why this is Video 01

- It introduces BitBlock through a useful, recognisable technology subject.
- It gives the channel an opportunity to explain and demonstrate rather than only announce itself.
- The creator already has a real WSL 2 environment, so the video can be grounded in actual experience.
- It does not depend on ATLAS being ready.
- It introduces Linux without suggesting that viewers must replace Windows.
- It can combine an accessible explanation with an authentic, small experiment.

## Scope

### Include

1. The problem this solves: wanting Linux tools while continuing to use Windows.
2. A plain-language explanation of WSL.
3. The important WSL 2 detail: it uses a real Linux kernel inside a lightweight, Windows-managed virtual machine.
4. A short explanation of how that differs from installing a separate traditional VM or dual-booting.
5. A tour of the creator's actual Ubuntu terminal.
6. A few safe commands that show this is a real Linux environment.
7. A tiny file-creation demonstration inside the Linux home directory.
8. A balanced list of useful cases and limitations.
9. A short closing that invites viewers to follow BitBlock's technology experiments.

### Exclude

- A complete installation tutorial. This video explains and demonstrates WSL; a separate setup guide can be made if useful.
- A full Linux command-line course.
- Docker, Kubernetes, servers, or ATLAS. They would make the first video unfocused.
- Unsupported performance comparisons or claims that WSL is always better than a VM.
- A claim that WSL 2 is not a VM. It uses a managed lightweight VM; explain that accurately.
- A fixed promise about which future video will be uploaded next.

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

The demo creates one clearly named folder and one text file in the Linux home directory. It does not modify system configuration. The final command opens the current directory in Windows File Explorer; verify that it works in the recording environment. Do not show personal directory names in the address bar.

## Core story

**Windows is the desktop the viewer already knows. WSL lets them add a Linux environment and Linux command-line tools without having to leave Windows or manage a separate traditional VM themselves.**

Keep the story simple:
- What problem does it solve?
- What is it?
- What does WSL 2 actually run?
- What does it look like in practice?
- When is it useful, and what should viewers know before relying on it?

## Planned structure

See [SCRIPT.md](SCRIPT.md) for narration and [SHOT_LIST.md](SHOT_LIST.md) for capture instructions.

| Section | Approx. time | Purpose |
|---|---:|---|
| Hook | 0:00–0:25 | Show Linux running alongside Windows |
| The problem | 0:25–1:15 | Explain why someone might want both |
| What WSL is | 1:15–2:30 | Define WSL and WSL 2 |
| How WSL 2 works | 2:30–3:30 | Explain the managed lightweight VM |
| Live demonstration | 3:30–6:30 | Show real terminal commands and a tiny file |
| Benefits and limitations | 6:30–8:00 | Set realistic expectations |
| Closing | 8:00–8:30 | Recap and invite viewers to subscribe |

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

- Use the creator's actual machine and actual results.
- Narration should sound natural, not like a formal lecture.
- Explain technical terms when first introduced.
- Use screen recordings, terminal captures, and simple diagrams; no face camera is required.
- Do not add music or effects that compete with the explanation.
- Keep the video focused. Do not turn it into a WSL installation marathon.
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

**Current state: planning package created. No recording or publication is claimed.**
