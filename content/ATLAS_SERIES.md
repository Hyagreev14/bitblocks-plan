# Building ATLAS — Series Plan

## Concept
A recurring BitBlock Tech series documenting the development of ATLAS session by session. Each episode covers a real work session or a coherent milestone, using a screenshot-based timelapse and a full voiceover.

The series should show the evolution of the project: planning, design decisions, implementation, debugging, revisions, testing, and milestones. It is both a project diary and an understandable explanation of the work. It should remain a genuine record of development rather than a staged demonstration in which every session appears perfect.

## Two connected episode tracks

### 1. Planning and design
These episodes explain why ATLAS is being shaped in a particular way. Suitable subjects include product vision, intended users, Core and Pro boundaries, user journeys, UI concepts, architecture, the ATLAS Action Protocol, tool discovery, consent, AI modes, repository permissions, security design, and trade-offs.

Planning episodes can be made before implementation. They must clearly distinguish ideas, decisions, prototypes, and implemented features.

### 2. Development sessions
These episodes show how the plan becomes real. The creator does not plan to record continuous desktop video. The intended method is a Chronolapse-style tool that captures screenshots periodically—initially around every 5 or 10 seconds—then assembles the images into a timelapse.

**Every development episode should have a voiceover** explaining what happened in that session. The narration is essential because a fast screenshot sequence cannot explain intent by itself.

## Capture-to-video pipeline
1. Choose a meaningful ATLAS work session.
2. Prepare a clean capture workspace and check for private information.
3. Capture screenshots at the selected interval, initially testing 5 seconds and 10 seconds.
4. Work normally; do not change the development process just to create visually busy footage.
5. Review the full image sequence and remove sensitive or irrelevant frames.
6. Assemble the approved frames into a timelapse.
7. Write a narration outline from what actually happened.
8. Record the voiceover explaining the session.
9. Edit the narration and timelapse together; add zooms, pauses, diagrams, or still frames when they materially improve understanding.
10. Review the complete export for accuracy, clarity, audio, and privacy.

## What each development episode should communicate
- The goal of the session and why it matters.
- The relevant state of ATLAS before the session.
- The meaningful work performed.
- Important implementation decisions and their reasoning.
- Bugs, blockers, and unexpected behaviour.
- What was tested and the actual result.
- What is incomplete or still uncertain.
- The most natural next step.

Do not narrate every keystroke or mouse movement. Explain the work in coherent sections.

## Possible episode sequence
1. Introducing ATLAS: the problem, vision, and intended workflow.
2. Planning the initial scope and Core/Pro boundaries.
3. Establishing the project foundation.
4. Designing the initial interface and first-run experience.
5. Planning the action protocol and its safety boundaries.
6. Implementing and validating a first protocol path.
7. A development session focused on a meaningful feature.
8. Reviewing what works, what needs redesign, and what comes next.

This is an idea sequence, not a fixed release plan. The actual project state should determine the order.

## Continuity
Use a consistent series name such as Building ATLAS. Number episodes only if numbering helps viewers follow the journey. Each video should still make sense to a new viewer: provide a short recap of only the context needed, then focus on the current story.

## When a session deserves an episode
A session can stand alone when it contains a clear viewer-friendly story: a feature was developed, a difficult issue was investigated, an important design was implemented, or a meaningful milestone was reached. Combine small routine sessions when they do not support a complete episode. Split a large session when it contains distinct stories.

## Honesty and project accuracy
Do not imply that ATLAS is finished or that a feature works unless it has been tested. Show prototypes as prototypes and plans as plans. If an approach changed, explain why. The live ATLAS repository and actual implementation are the source of truth—not this channel plan.

## Protect the project
Review screenshots, terminal output, editor tabs, browser tabs, and the final export. Keep credentials, tokens, private repositories, personal files, and private notifications out of published material. See the privacy guide.

## Flexibility
The series should support ATLAS development, not slow it down. Do not force every work session into an upload or delay useful project work to manufacture footage.