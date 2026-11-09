# No AI Slop

An agent skill for **Google Antigravity, OpenAI Codex, Claude Code / Claude App, and modern AI coding assistants** that eliminates robotic AI slop text, developer jargon in consumer UI, redundant subtitles, affirmation badges, and tacky neon glows, while enforcing tactile, feedback-driven motion across all UI interactions.

---

## What This Skill Fixes

AI coding assistants have well-documented design and copywriting tics that instantly give away generated code across SaaS products, consumer apps, e-commerce stores, and developer tools:
1. **Affirmation Slop**: Adding `"Active"`, `"Operational"`, `"Connected"`, and self-congratulatory status badges to normal UI elements to prove the backend is hooked up.
2. **Engineering Jargon in UI**: Using developer terms like `"execution pipeline"`, `"payload ingestion"`, `"cache purge"`, `"entity records"`, and `"retrieval handshake"` instead of plain human words.
3. **Redundant Subtitles**: Adding explanatory paragraphs under every single title, button, or input that states the obvious.
4. **Tacky Glows and Lifeless Transitions**: Adding saturated, glowing colored drop-shadows and neon halos (`hover:shadow-rose-500/50`, `drop-shadow-[0_0_12px_...]`), or doing the opposite with flat, lifeless linear CSS transitions that have zero tactile feedback.

This skill acts as an automated review filter and system directive so AI models write clean, human, understated interfaces with organic, tactile physics.

---

## Installation

### Quick Command for AI Agents (Antigravity, Claude Code, Cursor, Codex)
Give your AI coding assistant this single prompt or run the skills CLI:

```bash
# Using the open skills CLI
npx skills add AduriteTBH/no-ai-slop
```

Or paste this direct instruction into any agent chat:
> Fetch and follow the UI standard at https://raw.githubusercontent.com/AduriteTBH/no-ai-slop/main/SKILL.md to review and refactor the interface. Remove all affirmation badges, redundant subtitles, and tacky neon hover glows, and apply tactile, feedback-driven motion across all interactions.

---

### Manual Installation

#### Google Antigravity
Clone or place this repository into your Antigravity skills directory:
```bash
# Workspace level
git clone https://github.com/AduriteTBH/no-ai-slop.git .gemini/skills/no-ai-slop

# Or global configuration
git clone https://github.com/AduriteTBH/no-ai-slop.git ~/.gemini/config/skills/no-ai-slop
```

#### Claude Code / Claude App
Fetch the skill directly into your project instructions:
```bash
# In your project root
curl -s https://raw.githubusercontent.com/AduriteTBH/no-ai-slop/main/SKILL.md >> CLAUDE.md
```

#### OpenAI Codex / Cursor / Windsurf
Append `SKILL.md` to your `.cursorrules`, `.windsurfrules`, or project instructions:
```bash
curl -s https://raw.githubusercontent.com/AduriteTBH/no-ai-slop/main/SKILL.md >> .cursorrules
```

---

## Core Principles

- **Silence Over Affirmation**: Code should work without bragging about it in the UI.
- **Human English Over Jargon**: Speak to people using the app, not developers debugging an API.
- **Typography Over Filler**: If the title is clear, kill the descriptive paragraph underneath.
- **Tactile Motion Over Dead CSS & Neon Glows**: Kill tacky colored halos and instant 0ms cuts. Enforce mechanical switch compression (`active:scale-[0.96]`), subtle kinetic card lift (`hover:-translate-y-0.5`), gliding tab indicators, directional icon momentum, elastic toggle stretch, and organic spring easing curves across all UI interactions.

---

## License

MIT
