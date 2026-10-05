# Model Advisor

A Claude skill that recommends the right AI model (Haiku, Sonnet, or Opus) for your development tasks.

## Overview

Choosing the right Claude model can be tricky. This skill analyzes your task and automatically recommends:

- **Haiku** — Fast execution, iteration, and known solutions
- **Sonnet** — Moderate complexity with analysis
- **Opus** — Deep reasoning, architecture, and new problems

## Installation

### For Claude.ai / Cowork users

1. Copy the `SKILL.md` file to your Claude skills directory
2. Or use the `.skill` file if your Claude setup supports it
3. The skill will automatically appear in your `/` menu

### For Claude Code users

Place the `SKILL.md` in your configured skills directory and it will be available via `/model-advisor`.

## Usage

Simply describe what you're working on:

```
"I'm trying to figure out why my game's collision detection is sometimes buggy"
```

The skill analyzes your task and responds with:

```
Recommendation: Opus
Why: This is a mysterious, inconsistent bug that needs deep reasoning.
Root cause is unknown, and collision detection involves system thinking.
Use Opus for deep analysis and to find hidden issues.
```

## Quick Decision Framework

Ask yourself these three questions in order:

1. **Have I solved this type of problem before?**
   - Yes → Haiku or Sonnet
   - No → Opus

2. **Do I know what the solution should be?**
   - Yes, clearly → Haiku
   - Yes, roughly → Sonnet
   - No → Opus

3. **Is this execution or exploration?**
   - Execution → Haiku
   - Analysis → Sonnet
   - Exploration → Opus

## Domain Examples

### Web Game Development
- **Haiku:** Add sprite, implement input, tweak animation
- **Sonnet:** Add new game mechanic, optimize rendering
- **Opus:** Design game loop, collision algorithm, debug performance mystery

### SCADA/Industrial
- **Haiku:** Add OPC tag, write familiar script
- **Sonnet:** Migrate query, optimize pipeline, debug slow report
- **Opus:** New OPC architecture, redesign alarm pipeline, debug production mystery

### General Development
- **Haiku:** Fix a known bug you understand
- **Sonnet:** Performance is slow (probably known issue-type)
- **Opus:** Why does it fail in prod? Design a new system.

## When This Skill Triggers

The skill automatically activates when you:
- Ask "which model should I use?"
- Describe debugging, design, or architecture work
- Ask for model selection advice
- Describe any task where choosing the right tool matters

## Testing

The skill was tested on 3 realistic scenarios:

✅ **Debugging collision bug** → Opus (mysterious, needs reasoning)
✅ **Adding game feature** → Haiku (known pattern, execution)
✅ **Performance analysis** → Sonnet (analysis, moderate complexity)

## Contributing

Found edge cases? Want to improve the recommendations? Open an issue or PR!

## License

MIT — Use freely, modify, adapt.

## Built With

- Created using Claude skill-creator
- Tested on real development scenarios
- Optimized for Haiku, Sonnet, and Opus models

---

**Start using it:** Describe any task and ask which Claude model fits best. The skill will guide you.
