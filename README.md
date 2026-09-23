Claude Skills

A shared collection of Claude Skills for the Analytics Ninja team.

What's a skill?

A skill is a small folder with a set of written instructions inside it (a file called SKILL.md) that teaches Claude how to do a specific kind of task the way we actually want it done, not just the generic default way. Once a skill is added to someone's Claude setup, Claude reads it automatically whenever it's relevant, no need to re-explain the approach every time.

Each skill lives in its own folder in this repo. To use one, copy that folder into wherever your own Claude setup reads skills from (see "Using a skill" below).

What's in this repo
email-review/

Reviews or rewrites an email draft, a new one or a reply, so the most important line comes first, jargon gets cut except where it's genuinely load-bearing, and the body is organized to be scanned in a few seconds rather than read start to finish.

Built from a real example: a client-facing pricing email that was technically correct but buried the actual recommendation under several paragraphs of statistical reasoning. The skill captures what changed when it got simplified, and applies that same approach going forward.

Using a skill
Download or copy the skill's folder (for example, email-review) from this repo.
Place that folder into the location your Claude setup reads skills from. In Claude Code, that's typically a .claude/skills/ folder, either inside a specific project or in your home directory if you want it available everywhere.
That's it. Claude will pick it up automatically and use it when a task matches what the skill describes, you don't need to invoke it by name.
Adding a new skill

Create a new folder in this repo named after the skill, with a SKILL.md file inside describing what it should do and when Claude should use it. Keep it in plain language, explain the reasoning behind each instruction rather than just listing rules, that's what makes a skill generalize well instead of only working for the one example it was built from.
