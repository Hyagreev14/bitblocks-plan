# Video 01 — Recording Checklist

## Before recording

- [ ] Read the latest script and shot list.
- [ ] Decide whether the narration will be recorded before or after the screen capture.
- [ ] Test the microphone and record a short sample.
- [ ] Check screen-capture resolution, frame rate, and audio settings.
- [ ] Close private chats, email, personal browser tabs, and unrelated apps.
- [ ] Enable Do Not Disturb / Focus Assist if appropriate.
- [ ] Hide desktop shortcuts or files that should not appear.
- [ ] Prepare a clean PowerShell window and Ubuntu terminal.
- [ ] Increase terminal font size so commands are readable.
- [ ] Check terminal prompt and paths for personal information.
- [ ] Run every command used on the actual creator machine once before recording.
- [ ] Verify the WSL distribution is actually using WSL 2.
- [ ] Confirm the demo folder and text file are safe to create.
- [ ] Prepare the WSL 2 architecture diagram or a placeholder.
- [ ] Prepare the fresh-install walkthrough graphic: supported Windows versions, Administrator PowerShell, wsl --install, restart, first Ubuntu launch, Linux account, and version verification.
- [ ] Verify the installation graphic against the linked Microsoft documentation.
- [ ] Remember that the creator's machine already has WSL installed. Do not uninstall, reset, or reinstall it for footage.

## During recording

- [ ] Capture each shot separately where possible.
- [ ] Keep command output on screen long enough to read.
- [ ] Do not rush commands to fit a target duration.
- [ ] If a command fails, stop and investigate; do not hide a failure by pretending it worked.
- [ ] Capture actual output, not recreated output presented as live.
- [ ] Clearly label the installation sequence as a fresh-PC walkthrough, not a live install on the creator's machine.
- [ ] Avoid showing personal paths, usernames, machine identifiers, or notifications.
- [ ] Do not show or record any real password entry.
- [ ] Record a clean take of the opening and closing.
- [ ] Save source recordings in the intended project location.

## Voiceover

- [ ] Record in a quiet environment.
- [ ] Keep microphone distance consistent.
- [ ] Speak naturally and explain unfamiliar terms.
- [ ] Leave small pauses between ideas.
- [ ] Re-record unclear sentences rather than relying on heavy editing.
- [ ] Check that background noise does not obscure words.

## After recording

- [ ] Review the captured footage before editing.
- [ ] Remove unusable takes and any frame containing private information.
- [ ] Confirm every shown command and result matches the script.
- [ ] Update the script if the real demonstration differs.
- [ ] Back up the original recordings before deleting or moving anything.
- [ ] Record any technical questions that need another fact-check.

## Privacy review

Never publish:
- passwords, API keys, access tokens, SSH private keys, or recovery codes;
- private messages, email contents, or personal notifications;
- personal file names, account names, or directory paths unless deliberately approved;
- private repository contents or unannounced project details;
- browser tabs or terminal history unrelated to the video.

Review the final export frame by frame around every terminal, settings, and file-manager capture. A blur added in editing is not a substitute for checking the original footage.
