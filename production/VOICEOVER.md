# Voiceover Guide

## Role of narration
The voiceover is the explanation layer for the video. In the ATLAS session series, **every development episode should have narration explaining the work done in that session**. The timelapse alone is not expected to communicate the story, and the voiceover is not an occasional add-on.

Narration should explain intent, decisions, progress, and limitations—not simply read out visible code or describe every mouse movement.

## Prepare after the session
Use the real work session as the source of truth. Before recording, note:
- the goal for the session;
- relevant context from earlier work;
- the main tasks completed;
- important implementation decisions and why they were made;
- bugs, obstacles, and unexpected behaviour;
- tests performed and their actual results;
- what remains incomplete or uncertain;
- the next useful step.

If the session did not achieve its original goal, that is still a valid story. Explain what happened honestly.

## A useful narration structure
- **Opening:** identify the session's goal, result, or interesting problem.
- **Context:** briefly explain what already exists and why this task matters.
- **Work:** explain the main changes in a logical order.
- **Reasoning:** describe important choices and trade-offs.
- **Challenges:** explain bugs, uncertainty, or approaches that did not work.
- **Result:** say what works, what is incomplete, and how the result was checked.
- **Next:** identify a natural next step without promising an unconfirmed release date.

This is a guide, not a compulsory script formula. Reorder or shorten it to fit the session.

## Script versus outline
Use a full script when the subject involves complex technical explanation, precise claims, or wording that needs careful verification. Use an outline when the creator knows the work well and a natural explanation will sound better. A hybrid is often useful: script the opening and technical explanations, then use notes for the session walkthrough.

## Narration style
Speak as if explaining the work to a curious person. Define unfamiliar terms when useful. Avoid forced hype, corporate language, repetitive filler, and claims that make a normal development session sound like a dramatic breakthrough. Do not narrate every keystroke. Group work into meaningful sections and explain why those sections matter.

## Recording
- Record a short test and listen for clipping, noise, and volume.
- Keep a consistent distance from the microphone.
- Speak clearly at a natural pace.
- Leave short pauses between ideas to make editing easier.
- Re-record sections that are difficult to understand.
- Keep a clean copy of the voice track until the edit is final.

## Editing
Remove long pauses, repeated phrases, and unrelated tangents, but preserve a natural cadence. Keep background music below speech and avoid sound effects that distract from technical explanation. Check the final mix on available speakers or headphones.

## Accuracy
Narration must match the actual session and current project state. Distinguish planned, attempted, partially completed, implemented, and tested. Never imply a test passed if it was not run. If a design changed after the session, explain that it changed rather than silently presenting the final plan as if it had always been the original approach.