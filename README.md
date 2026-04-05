# Almost-Tokenless Skill

**Default:** This skill is always active unless you ask for more explanation, reasoning, or context (e.g. "explain", "why", "walk me through it"). Minimal prose is the baseline.

Ultra-low token mode for OpenClaw agents. Minimal prose, maximum signal.

## When to Use

- Cost-sensitive tasks (paid API providers)
- Quick debugging sessions
- Repetitive operations where brevity matters
- When you explicitly want no fluff

## Triggers

The skill auto-activates on these phrases:
- "token efficient"
- "minimal tokens"
- "caveman mode"
- "grug brain"
- "just the answer"
- "no explanation"
- "keep it short"

## What It Does

Forces the agent to:
- Skip preambles and filler
- Use 2-5 word sentences
- Run tools immediately without narration
- Return only: finding / fix / next step
- Summarize noisy output in 1-3 bullets

## Example

**Normal mode:**
> "Sure! I'd be happy to help you check the server status. Let me run a quick command to see what's happening..."

**Almost-tokenless mode:**
> "Checking server status. Running: systemctl status gateway"

## Installation

### GitHub

```bash
git clone https://github.com/1devtests/almost-tokenless.git
cp -r almost-tokenless ~/.openclaw/workspace/skills/
```

Or, copy the contents of this repo directly into:
```
~/.openclaw/workspace/skills/almost-tokenless/
```

## Usage

Minimal token mode is always on by default unless you ask for more detail, explanation, or context.

## License

MIT - See LICENSE file
