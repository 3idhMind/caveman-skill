# 🪨 caveman-skill

> why use many word when few word do trick

**The only caveman skill built for [claude.ai](https://claude.ai) — web and desktop.**

Not Claude Code. Not a terminal plugin. The actual chat interface you use every day.

---

## The Gap

[JuliusBrussee's caveman](https://github.com/JuliusBrussee/caveman) is brilliant — 26k+ stars, viral on HN, ThePrimeagen covered it. But it only works in **Claude Code** (the CLI tool developers run on their machines).

**Nobody built this for claude.ai.** Until now.

---

## What It Does

Activates caveman mode inside claude.ai chat. Three intensity levels. Slashes output verbosity by up to 87% while keeping 100% technical accuracy.

| Mode | Command | Token Reduction | Style |
|------|---------|----------------|-------|
| LITE | `/caveman-lite` | ~30% | Cut fluff, keep grammar |
| NORMAL | `/caveman` | ~75% | Full caveman grammar |
| ULTRA | `/caveman-ultra` | ~87% | Brutal minimum. Grunts. |

---

## Before / After

**Normal Claude (72 tokens):**
> Sure! I'd be happy to help you with that. The issue you're experiencing is most likely caused by your authentication middleware not properly validating the token expiry. Let me take a look and suggest a fix. Hope that helps!

**LITE (38 tokens):**
> The issue is in your authentication middleware — token expiry isn't being validated correctly. Fix:

**NORMAL (11 tokens):**
> Auth middleware. Token expiry check wrong. Fix:

**ULTRA (6 tokens):**
> `auth middleware. expiry < not <=.`

---

## Install

### Step 1 — Download the skill

Download [`caveman-skill.zip`](https://github.com/devvaham/caveman-skill/releases/download/v1.0.0/caveman-skill.skill) from Releases.

### Step 2 — Upload to claude.ai

1. Go to [claude.ai](https://claude.ai)
2. Settings → **Capabilities** → **Skills**
3. Click **"Upload skill"**
4. Select the `.zip` file

### Step 3 — Use it

In any conversation, type:

```
/caveman
```

Claude confirms: `🪨 caveman mode on.`

To deactivate: `/normal`

---

## All Commands

```
/caveman-lite    → lite mode (~30% reduction)
/caveman         → normal caveman (~75% reduction)
/caveman-ultra   → ultra mode (~87% reduction)
/normal          → back to normal
```

Also works with plain English:
- "caveman mode", "talk like caveman", "be brief", "less words"
- "stop caveman", "normal mode", "talk normally"

---

## Mode Details

### 🪨 LITE
Removes pleasantries, meta-commentary, hedging, sign-offs. Grammar stays intact. Good for people who want clean answers without going full cave.

### 🪨🪨 NORMAL
Full caveman grammar. Drops articles, filler, padding. Fragments fine. Short synonyms. Maximum signal.

### 🪨🪨🪨 ULTRA
Absolute minimum. Symbols over words (`→`, `=`, `+`). Every word must earn its place. One fragment per point. Brutal.

**Code blocks are NEVER affected.** All modes write clean, full, correct code. Caveman speak only in the English wrapper.

---

## Why It Works

A [March 2026 arXiv paper](https://arxiv.org/abs/2502.04463) — *"Brevity Constraints Reverse Performance Hierarchies in Language Models"* — found that constraining LLMs to brief responses improved accuracy by **26 percentage points** on certain benchmarks.

Less verbose ≠ less intelligent. Often the opposite.

> Caveman not dumb. Caveman efficient.

---

## Compatibility

| Platform | Works? |
|---------|--------|
| claude.ai (web) | ✅ |
| Claude Desktop (macOS/Windows) | ✅ |
| Claude Code | ❌ use [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) |
| Claude API | ❌ just add rules to system prompt |

---

## Credits

Inspired by [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) — the original Claude Code skill that started the caveman movement.

This repo fills the gap: **claude.ai and Claude Desktop** users who want the same power without touching a terminal.

Built by [@Dev Vaham](https://github.com/devvaham)

---

## License

MIT — use it, fork it, make it better.

---

*🪨 caveman save token. token save money. money good.*
