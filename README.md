# BitBlock — Channel Plan & Agent Handoff

> **CODE. CREATE. EXPLORE.**

BitBlock is a faceless, creator-led channel about technology, software development, gaming, and the curiosity that connects them. This repository is the durable source of truth for the channel's direction. It exists so the creator—or a future AI agent, collaborator, or tool—can continue the work without reconstructing decisions from old conversations.

The creator owns the channel and makes final decisions. This plan is detailed enough to support continuity, but flexible enough to evolve as the channel develops.

## Start here

1. **[Channel overview](docs/CHANNEL_OVERVIEW.md)** — purpose, identity, channel promise, and scope.
2. **[Content strategy](docs/CONTENT_STRATEGY.md)** — how the Tech and Gaming worlds fit under one channel.
3. **[Editorial principles](docs/EDITORIAL_PRINCIPLES.md)** — accuracy, tone, safety, and creative freedom.
4. **[Agent handoff](planning/AGENT_HANDOFF.md)** — instructions for a future assistant taking over the project.
5. **[Current priorities](planning/NOW_NEXT_LATER.md)** — what is active, upcoming, and deliberately deferred.
6. **[Production workflow](production/WORKFLOW.md)** — the flexible path from idea to published video.

## Repository map

### docs/ — Durable channel foundations
- [Channel overview](docs/CHANNEL_OVERVIEW.md) — what BitBlock is and how it should feel.
- [Content strategy](docs/CONTENT_STRATEGY.md) — broad Tech and Gaming coverage without prematurely splitting channels.
- [Audience](docs/AUDIENCE.md) — intended viewers and the value each video should provide.
- [Editorial principles](docs/EDITORIAL_PRINCIPLES.md) — tone, honesty, technical depth, pacing, and creative freedom.
- [Brand identity](docs/BRAND_IDENTITY.md) — name, tagline, visual direction, and identity rules.
- [Channel architecture](docs/CHANNEL_ARCHITECTURE.md) — one channel now, possible sub-channels later.
- [Success signals](docs/SUCCESS_SIGNALS.md) — evaluating progress without obsessing over metrics.

### content/ — What BitBlock can publish
- [Content pillars](content/CONTENT_PILLARS.md) — recurring subject areas and how to classify overlapping videos.
- [BitBlock Tech](content/BITBLOCK_TECH.md) — broad technology coverage, not only Minecraft-adjacent technology.
- [BitBlock Gaming](content/BITBLOCK_GAMING.md) — Minecraft and other gaming content.
- [ATLAS series](content/ATLAS_SERIES.md) — the session-by-session development journey.
- [Planning videos](content/PLANNING_VIDEOS.md) — design, architecture, trade-offs, and decisions.
- [Video formats](content/VIDEO_FORMATS.md) — practical formats for a faceless, narrated channel.
- [Idea backlog](content/IDEA_BACKLOG.md) — possible videos, not promises or a fixed schedule.

### production/ — How videos are made
- [Production workflow](production/WORKFLOW.md) — idea to finished upload.
- [Timelapse capture](production/TIMELAPSE_CAPTURE.md) — periodic screenshot capture for ATLAS sessions.
- [Voiceover](production/VOICEOVER.md) — narration planning, recording, and editing.
- [Editing](production/EDITING.md) — pacing, visuals, sound, and export review.
- [Privacy and safety](production/PRIVACY_AND_SAFETY.md) — protecting credentials, personal information, and systems.
- [Publishing](production/PUBLISHING.md) — titles, thumbnails, descriptions, settings, and final checks.

### planning/ — Keeping the project manageable
- [Current priorities](planning/NOW_NEXT_LATER.md) — a flexible snapshot, not a deadline calendar.
- [Launch plan](planning/CHANNEL_LAUNCH.md) — a simple and achievable first phase.
- [Episode planning](planning/EPISODE_PLANNING.md) — scoping individual videos.
- [Review and iteration](planning/REVIEW_AND_ITERATION.md) — learning from uploads and improving deliberately.
- [Agent handoff](planning/AGENT_HANDOFF.md) — continuity instructions for future AI agents.

## Important decisions and direction

- **One umbrella channel first:** publish under BitBlock rather than splitting into BitBlock Gaming and BitBlock Tech immediately.
- **Two broad content worlds:** Tech includes general technology and development; Gaming includes Minecraft and other games.
- **Tech is not Minecraft-dependent:** Linux, WSL, Docker, programming, software development, AI tools, automation, servers, self-hosting, networking, cybersecurity education, Windows/developer tools, hardware, and homelabs are all valid subjects.
- **ATLAS is a flagship Tech series candidate:** document its real development journey, including planning, implementation, debugging, testing, and milestones.
- **Planning videos belong in the ATLAS journey:** planning and development can be separate episode types within one series.
- **Timelapse method:** capture periodic screenshots, initially testing intervals around 5–10 seconds, assemble them into a timelapse, and add a voiceover explaining the work in that session.
- **Every ATLAS development episode gets narration:** the voiceover is the explanation layer, not an occasional extra.
- **Faceless does not mean personality-free:** narration, opinions, decisions, experiments, mistakes, and explanations provide the human perspective.
- **Sustainability beats arbitrary frequency:** the workflow should fit real life, school, and project work. Do not invent a fixed upload schedule.

## How to interpret this repository

This is a living plan, not an unchangeable contract and not proof that every idea is implemented. A plan is not a completed feature; an idea is not a scheduled upload; a draft is not a published video. Mark uncertain or untested decisions clearly.

When updating the repository:
- Inspect the existing files and preserve useful decisions.
- Keep one clear source of truth for each topic.
- Update links when files move.
- Prefer focused documents over one enormous document.
- Do not add files just to increase the file count.
- Do not silently turn suggestions into confirmed decisions.
- Use meaningful commit messages and focused commits.
- Keep this README's navigation accurate.

## For future agents

Start with this README, then read [Agent Handoff](planning/AGENT_HANDOFF.md). Treat the creator as the decision-maker. Help with strategy, research, scripts, technical verification, production planning, titles, descriptions, and iteration. Be practical, direct, and collaborative. Avoid rigid corporate-style rules, unnecessary questionnaires, and overengineering.