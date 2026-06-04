# Universal Card Game Resolution Order (UROE v2)

*Original filename: "UNIVERSAL CARD GAME RESOLUTION ORDE.txt"*

```
UNIVERSAL CARD GAME RESOLUTION ORDER ENGINE (UROE v2)

PURPOSE:
Defines deterministic resolution order across all card games.
Works with STRESS-PROOF v2 + Edge Case Library.
Does NOT replace game rules — interprets them consistently.

─────────────────────────────

CORE RESOLUTION CYCLE:

S → N → I → M → V / B / H / C → STATE UPDATE → (NEW S CYCLE IF TRIGGERS OCCUR)

─────────────────────────────

LAYER DEFINITIONS:

S (Sequencing / Timing)
- Controls when effects enter resolution
- Validates timing (If / When / Whenever / Quick / Continuous)
- Orders simultaneous events
- ENTRY GATE ONLY

N (Negation / Pre-Resolution)
- Prevents effects before resolution
- Works only on pending effects
- Cannot affect resolved state

I (Interaction / Multiplier)
- Combines / amplifies effects
- Enables synergy chains
- Cannot negate or finalize effects

M (Resolution / State Change)
- Executes actual game changes
- Includes: summon, destroy, exile, bounce, discard, etc.
- FINAL execution step BEFORE evaluation

V / B / H / C (Post-Resolution Evaluation)
- V = Value / win progression
- B = board state
- H = hand resources
- C = consistency / access
- NO rule changes here

STATE UPDATE
- Locks final game state
- Checks for new triggers
- Begins next cycle if needed

... (trimmed for brevity)
```
