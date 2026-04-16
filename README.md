# ADHD Operating System

A [Claude skill](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview) that adapts responses to inattentive ADHD cognition. It changes both **how** Claude structures responses (chunking, progressive disclosure, visual hierarchy) and **what** Claude recommends (systems over willpower, external scaffolding over internal motivation).

Built for myself. Sharing in case it saves someone else a few months of iteration.

## What it does

The skill functions as a persistent filter layered over everything else. It triggers for productivity, organization, project management, learning, communication, habits, tool selection, career decisions, writing, creative work, and anything else that touches executive function, working memory, attention, motivation, or emotional regulation.

Grounded in Barkley, Brown, and current ADHD research rather than lifestyle-influencer advice. The core principles:

- **ADHD is a disorder of performance, not knowledge.** You probably already know what to do. The skill focuses on systems that externalize executive function instead of telling you to "just try harder."
- **Interest, urgency, novelty, and competition activate executive function.** Importance alone doesn't. Recommendations account for what will actually activate the brain.
- **Every system has a novelty half-life.** Recommendations build in flexibility so frameworks survive when execution details go stale.
- **Match energy, assume competence.** No cheerleading, no condescension.

## Structure

```
adhd-operating-system/
├── SKILL.md                                # Core principles and always-on rules
└── references/
    ├── formatting-and-structure.md         # How to present information (most-used)
    ├── project-management.md               # Tasks, tools, task paralysis, creative work
    ├── learning-and-retention.md           # Studying, note-taking, Zettelkasten, Anki
    ├── communication.md                    # Meetings, email, Slack, RSD, masking
    ├── daily-systems.md                    # Routines, habits, medication, sleep
    └── navigating-systems.md               # Finances, career, relationships, strengths
```

Claude reads `SKILL.md` always. Reference files load on demand based on what the conversation needs.

## How to install

Drop the folder into your Claude skills directory. For Claude.ai with skills enabled:

1. Zip the `adhd-operating-system` folder
2. Upload it via Settings → Capabilities → Skills
3. That's it

For Claude Code or other setups, place the folder wherever your skills loader looks (typically `~/.claude/skills/` or similar depending on configuration).

## Customize it

The skill is tuned for inattentive-presenting ADHD with an IT/technical professional bent. You'll probably want to adjust:

- **Tool recommendations** in `project-management.md` and `communication.md` (I'm partial to Amazing Marvin, Sunsama, Obsidian, YNAB — your stack will differ)
- **Medication timing** in `daily-systems.md` (written around a once-daily stimulant routine)
- **Tone calibration** at the bottom of `SKILL.md` (banned phrases like "you've got this" reflect my preferences)
- **The theme-days example** in `project-management.md` (infrastructure/security/writing rotation is mine, not universal)

Fork, adjust, don't ask permission.

## Credits

Draws on published work from Russell Barkley, Thomas Brown, John Ratey, Ned Hallowell, Melissa Orlov, Steven Safren, Holly White, Jeff Copper, Brendan Mahan, Jessica McCabe, Cal Newport, Tiago Forte, and the broader adult ADHD research and coaching community.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Use it, remix it, share it, credit the original.
