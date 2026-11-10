# Static variations

A Claude Code skill that plans, then builds, an automation to turn the photos a client has already sent you into new static ad images with Gemini.

From one photo you get new backgrounds, new scenes and every ad size, using real reference photos from Pexels so the scenes look real. A person approves every image before it's used.

## What it does

1. Looks at one example client's photos in Google Drive and sorts them by type.
2. Asks you about the client's look, what's off limits and your budget.
3. Agrees the right variations for each kind of photo, and how references are found.
4. Tests a small batch (it tells you the cost first) and learns from what you keep and reject.
5. Sets it up to run on a schedule, dropping new images into a `To review` folder.

Nothing is generated or spent until you've agreed the plan.

## What you need

- [Claude Code](https://claude.com/claude-code)
- Google Drive tools in Claude, such as the Google Drive connector
- A Gemini API key from [Google AI Studio](https://aistudio.google.com) (images cost a few US cents each)
- A free [Pexels API key](https://www.pexels.com/api/)

## Install

1. Make the folder `~/.claude/skills/static-variations/`.
2. Download [`SKILL.md`](SKILL.md) into it.
3. Open Claude Code and say "plan static variations". Claude walks you through the rest.

Your API keys go in a local `.env` file that you fill in yourself. Never paste them into the chat.

---

Made by [Minimise](https://minimise.co.nz).
