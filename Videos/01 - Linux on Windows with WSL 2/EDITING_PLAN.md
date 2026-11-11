# Video 01 — Editing Plan

## Editing objective

Make WSL 2 understandable to someone who has never used it. The edit should feel like a creator showing something useful and explaining it clearly—not a corporate presentation or a command-line speedrun.

**Target duration:** 7–10 minutes, flexible.

## Structure and pacing

| Section | Target | Editing approach |
|---|---:|---|
| Hook | 0:00–0:25 | Quick Windows/Ubuntu contrast; establish the promise immediately |
| Problem | 0:25–1:15 | Calm narration with a simple two-environment visual |
| WSL definition | 1:15–2:30 | Clear title and simple diagram |
| WSL 2 architecture | 2:30–3:30 | One uncluttered diagram; animate the layers |
| Live tour | 3:30–5:00 | Screen capture; zoom only when needed |
| Practical example | 5:00–6:15 | Show commands and output at readable speed |
| Benefits | 6:15–7:00 | Short labels and supporting desktop/terminal shots |
| Limitations | 7:00–8:00 | Balanced list; don't rush the caveats |
| Closing | 8:00–8:30 | Return to desktop/terminal and BitBlock end card |

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

## Screen recording

- Trim pauses while commands are being typed, but retain enough context to follow.
- Avoid speeding up important commands or output.
- Use punch-ins for `wsl --status`, `wsl --list --verbose`, `uname -r`, and the demo file output.
- Blur or crop usernames, personal paths, device names, and unrelated files.
- Keep the same terminal theme and font size across the main demo where possible.
- If the actual output differs from the script, update narration or captions to match.

## Audio

- Voiceover is the primary audio.
- Record narration in short sections if that makes delivery more natural.
- Remove distracting noise and abrupt volume changes.
- Background music is optional. If used, keep it quiet under narration and remove it during command explanations if it reduces clarity.
- Avoid excessive whooshes, glitch sounds, or impacts. The subject is practical technology, not an esports trailer.

## Graphics to create

1. Opening title: "Linux on Windows?"
2. WSL full-name lower third.
3. Simple WSL 2 architecture diagram.
4. Three benefit labels.
5. Three limitation labels.
6. BitBlock end card with "CODE. CREATE. EXPLORE."

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
- Check diagrams for technical accuracy.
- Check that no private information appears in any frame.
- Confirm that the title, thumbnail, description, and actual content agree.
