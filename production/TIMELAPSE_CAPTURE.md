# Timelapse Capture

## Purpose
Capture the development of ATLAS without recording continuous desktop video. A Chronolapse-style screenshot tool periodically captures the workspace; the approved images are later assembled into a timelapse.

The timelapse is the visual record of the session. The voiceover explains the meaning of the work. Neither needs to show every single action.

## Starting interval
Test an interval of roughly **5–10 seconds**:
- **5 seconds:** captures more intermediate states and may make changes easier to follow, but creates more images and uses more storage.
- **10 seconds:** creates a lighter sequence and a faster visual progression, but may skip brief actions or intermediate states.

Use a short test session to compare the results. The interval is a starting choice, not a permanent rule. Select based on the pace of the work, image volume, readability, and editing effort.

## Before capture
- Create a dedicated folder for each project session.
- Capture only the intended monitor or application area where practical.
- Close unrelated windows, notifications, personal messages, and account pages.
- Use a clean workspace layout and readable editor scaling.
- Keep passwords, API keys, tokens, recovery codes, private keys, and other secrets off-screen.
- Check terminal output, browser tabs, editor tabs, and file paths for private information.
- Confirm available disk space and test a short capture before a long session.
- Keep screen resolution and scaling stable where possible.

## During the session
Work normally. Do not change the development process just to make the timelapse look busy. Pause capture during long breaks if convenient. Optional notes can mark useful moments such as:
- session start and task objective;
- feature or component started;
- meaningful implementation completed;
- bug discovered or fixed;
- important design decision changed;
- test run and its result;
- session ended.

These markers are optional. The workflow should remain lightweight.

## After the session
1. Stop capture and preserve the original sequence temporarily.
2. Review every image, not just a sample.
3. Remove or exclude frames containing private information, unrelated windows, or accidental captures.
4. Check that the sequence is in chronological order.
5. Confirm that image dimensions and scaling are consistent.
6. Assemble the approved frames into a video.
7. Adjust playback speed so routine work moves quickly while meaningful changes remain understandable.
8. Add zooms, crops, pauses, or still frames when small text would otherwise be unreadable.
9. Sync the timelapse with the session voiceover.
10. Recheck the final render for any information that was missed during frame review.

## Limitations
A screenshot timelapse cannot show every interaction clearly and may jump over short actions. The narration must explain important changes. Use a separate diagram, still image, or brief direct screen capture only when it materially improves understanding; do not turn the workflow into continuous recording by default.

## Storage and organisation
Use predictable session folders, for example a project folder containing date- or session-labelled capture folders, a reviewed image sequence, the generated timelapse, and the final edit. Keep raw captures only as long as useful for editing or project history. Avoid committing large raw image folders to the planning repository.

## Privacy
Never publish credentials, personal information, private messages, private repository content, or sensitive account screens. If a secret appears in a capture, remove the affected frame and assess whether the credential itself must be rotated. See the privacy and safety guide.