# Video 01 — Editing Plan

## Editing objective

Make WSL 2 understandable to someone who has never used it, and leave the viewer knowing how to install Ubuntu through WSL on a supported Windows PC. The edit should feel like a creator showing something useful and explaining it clearly—not a corporate presentation or a command-line speedrun.

**Target duration:** 9–11 minutes, flexible.

## Structure and pacing

| Section | Target | Editing approach |
|---|---:|---|
| Hook | 0:00–0:25 | Quick Windows/Ubuntu contrast; promise an installation walkthrough |
| Problem | 0:25–1:05 | Calm narration with a simple two-environment visual |
| WSL definition | 1:05–2:10 | Clear title and simple diagram |
| WSL 2 architecture | 2:10–3:00 | One uncluttered diagram; animate the layers |
| Compatibility | 3:00–3:30 | Short Windows version requirement card |
| Installation walkthrough | 3:30–4:45 | Admin PowerShell, wsl --install, restart; label as a fresh-PC walkthrough |
| First launch and verification | 4:45–5:45 | Ubuntu setup, Linux account, wsl --list --verbose |
| Live tour | 5:45–6:45 | Actual creator terminal and WSL status |
| Practical example | 6:45–7:45 | Show commands and output at readable speed |
| Benefits | 7:45–8:30 | Short labels and supporting desktop/terminal shots |
| Limitations | 8:30–9:20 | Balanced list; don't rush the caveats |
| Closing | 9:20–9:50 | Return to desktop/terminal and BitBlock end card |

These are rough edit targets. Use the final narration and captured material to determine actual timings.

## Visual language

- Dark charcoal / near-black panels for diagrams.
- Electric cyan or icy blue for the WSL path and key labels.
- Restrained green for successful command output.
- Use a consistent modern sans-serif font.
- Keep diagrams simple: Windows host → WSL 2 managed VM → Linux kernel → Ubuntu distribution.
- Do not imply that WSL 2 avoids virtualization; explain that Windows manages the lightweight VM.
- Keep terminal text large enough to read on a phone.
- Use cursor highlights or subtle zooms to direct attention, not constant motion.
- Make installation steps readable: administrator PowerShell → wsl --install → restart → open Ubuntu → create Linux account → verify version 2.
- Clearly label the installation sequence as a fresh-PC walkthrough because the creator's machine already has WSL installed.

## Screen recording

- Trim pauses while commands are being typed, but retain enough context to follow.
- Avoid speeding up important commands or output.
- Use punch-ins for wsl --status, wsl --list --verbose, uname -r, and the demo file output.
- Blur or crop usernames, personal paths, device names, and unrelated files.
- Keep the same terminal theme and font size across the main demo where possible.
- If the actual output differs from the script, update narration or captions to match.
- Do not run wsl --install on the creator's already-configured machine just for footage. Use a labelled command graphic for the fresh-install sequence; never fake live installer output.

## Audio

- Voiceover is the primary audio.
- Record narration in short sections if that makes delivery more natural.
- Remove distracting noise and abrupt volume changes.
- Background music is optional. If used, keep it quiet under narration and remove it during command explanations if it reduces clarity.
- Avoid excessive whooshes, glitch sounds, or impacts. The subject is practical technology, not an esports trailer.

## Graphics to create

1. Opening title: "How to Install Linux on Windows with WSL 2".
2. WSL full-name lower third.
3. Simple WSL 2 architecture diagram.
4. Compatibility card: Windows 11 or Windows 10 version 2004 / build 19041 or later.
5. Installation walkthrough: PowerShell as Administrator → wsl --install → restart.
6. First-launch card: open Ubuntu → create Linux username and password.
7. Verification card: wsl --list --verbose → VERSION 2.
8. Three benefit labels.
9. Three limitation labels.
10. BitBlock end card with "CODE. CREATE. EXPLORE."

## Suggested benefit labels

- Use Linux tools on Windows
- Keep Windows apps in your workflow
- Useful for Linux-oriented development

## Suggested limitation labels

- Uses system resources
- File location can affect performance
- Not a replacement for every Linux setup

## Export and review

- Export at the same resolution and frame rate as the main recording timeline, unless there is a deliberate reason to change.
- Use a standard YouTube-friendly MP4 export.
- Watch the entire export, not just the beginning.
- Check terminal text at phone-size playback.
- Check narration clarity and music level.
- Check diagrams and installation steps for technical accuracy.
- Check that the installation graphic is presented as a walkthrough, not as footage of a live install.
- Check that no private information appears in any frame.
- Confirm that the title, thumbnail, description, and actual content agree.
