# Model Advisor — Test Cases

These are real-world scenarios the skill has been tested on.

## Test 1: Debugging Game Collision Bug

**Scenario:**
> "I'm building a Wizball-remake web game and I just realized the collision detection is wrong — sometimes the player ball clips through walls but not other times. It's inconsistent and I can't figure out why."

**Recommendation:** Opus
**Why:** Mysterious, inconsistent bug; root cause unknown; unfamiliar domain (first collision system)

---

## Test 2: Adding Game Enemy Type

**Scenario:**
> "I need to add a new enemy type to my game that shoots projectiles. I already have the enemy base class and weapon system working. Just need to inherit from enemy, override the shoot method, and add sprite assets."

**Recommendation:** Haiku
**Why:** Straightforward execution; knows exactly what to do; familiar pattern (already did other enemies)

---

## Test 3: SCADA Performance Analysis

**Scenario:**
> "Our Plant SCADA system is getting slow when generating end-of-month reports — they take 5-10 minutes now but used to be fast. The queries look fine to me but something feels off. I'm not sure if it's the database, the OPC UA connection, or the reporting engine."

**Recommendation:** Sonnet (escalate to Opus if root cause remains unknown)
**Why:** Needs analysis; could be familiar issue-type (disk, query, pool); moderate-to-high complexity; familiar domain but this specific problem feels new

---

## Test 4: Swedish — Simple Ignition Change

**Scenario:**
> "Räcker Haiku för att lägga till ett par nya taggar i en befintlig UDT och koppla dem till larm? Jag har gjort likadant många gånger."

**Recommendation:** Haiku
**Why:** Familiar, repetitive task; the solution is clear; pure execution. The answer should be in Swedish.

---

## Test 5: Swedish — Unclear Production Error

**Scenario:**
> "Vilken modell ska jag köra? Min PWA visar gammal data på vissa mobiler men inte på datorn, trots att jag har bumpat CACHE_NAME. Jag fattar inte varför."

**Recommendation:** Opus
**Why:** Root cause unknown; inconsistent behaviour across devices; needs real exploration. The answer should be in Swedish.

---

## Test 6: Should NOT Trigger

**Scenario:**
> "Kan du lägga till en knapp för mörkt läge i inställningsvyn?"

**Recommendation:** — (skill should not activate)
**Why:** An ordinary development request; the user isn't asking about model choice.

---

## Adding Your Own Test Cases

Did you find an edge case? Submit it as a PR with:

1. **Scenario** — Real task description
2. **Recommendation** — What the skill recommended
3. **Your feedback** — Was it right? Why or why not?

Use these to help improve the skill for everyone!
