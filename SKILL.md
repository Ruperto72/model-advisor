---
name: model-advisor
description: Choose the right Claude model (Haiku, Sonnet, or Opus) for a task. Use when the user asks which model to use, in English or Swedish — e.g. "which model for this?", "Haiku or Opus?", "is Sonnet enough?", "vilken modell ska jag använda?", "vilken modell för det här?", "Haiku eller Opus?", "räcker Sonnet?", "behöver jag Opus till det här?" — or when they describe upcoming work and are unsure how much reasoning power it needs. Recommends Haiku for execution and iteration, Sonnet for moderate complexity, and Opus for architecture, design, and new problem-solving. Do not trigger on ordinary development requests where model choice isn't in question. Answer in the user's language.
---

# Model Advisor

Choosing between Haiku, Sonnet, and Opus depends on *what kind of thinking* your task needs and how familiar the problem is.

## Haiku — Execution & iteration
Use when:
- You **know what you want** — just need to code it
- Implementing features, fixing bugs in code you understand
- Refactoring, adding tests, writing docs
- You're in flow and shipping code

**Cost/Speed:** Fastest, cheapest. Perfect for executing a clear plan.

## Sonnet — Moderate complexity
Use when:
- You need **more thinking than Haiku, but not full Opus**
- Adding new features to existing systems (new but scoped)
- Debugging familiar problem types (needs analysis, likely a known issue-type)
- Code review, architectural tweaks
- Performance tuning in domains you know

**Cost/Speed:** Fast with more reasoning power than Haiku.

## Opus — Deep reasoning & design
Use when:
- You're **solving something for the first time** — new architecture, unfamiliar domain
- Designing system architecture, data models, abstractions
- Debugging mysterious failures (root cause unknown)
- Optimizing performance in unfamiliar systems
- Evaluating trade-offs, security design, complex refactoring

**Cost/Speed:** Most capable. Best at complex reasoning and system thinking.

## Decision framework

Ask yourself in order:

1. **Have I solved this type of problem before?**
   - Yes → Haiku (if straightforward) or Sonnet (if moderate complexity)
   - No → Opus

2. **Do I know what the solution should be?**
   - Yes, clearly → Haiku
   - Yes, roughly → Sonnet
   - No → Opus

3. **Is this execution or exploration?**
   - Pure execution → Haiku
   - Some analysis → Sonnet
   - Exploration/design → Opus

## Examples by domain

### Web game development
- **Haiku:** Add sprite, implement input handling, tweak animation, write shader
- **Sonnet:** Add new game mechanic (new but scoped), optimize rendering in known engine
- **Opus:** Design game loop architecture, collision detection algorithm, debug mysterious performance bottleneck

### SCADA/Industrial
- **Haiku:** Add OPC UA tag, write familiar gateway script, add alarm rule
- **Sonnet:** Migrate a historian query, optimize existing data pipeline, debug slow report
- **Opus:** New OPC integration architecture, redesign alarm pipeline, debug production mystery no one understands

### General development
- **Haiku:** "Fix this known bug in code I wrote"
- **Sonnet:** "Performance is slow — probably cache related"
- **Opus:** "Why does this fail in production but not dev?" or "Design cache strategy for this system"

## How to use this skill

Describe what you're building, what's stuck, or what you're unsure about. This skill will recommend Haiku, Sonnet, or Opus and explain why.

If it's genuinely a border case (e.g., "probably Sonnet, but could be Haiku if you just want speed"), the explanation will help you choose based on your priorities.
