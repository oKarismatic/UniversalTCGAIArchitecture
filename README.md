# UniversalTCGAIArchitecture
Modular AI framework for TCG logic, featuring UROE v2 resolution engine, stress-proof edge-case handling, and dual-personality coaching agents.

My brother and I built this system because we were tired of AI tools that struggled with complex card game logic, timing, and rules. We wanted something that could actually "think" through a game's state deterministically and explain its reasoning.

This system is a deterministic state machine that separates game rules from execution logic. It is designed to be highly adaptable; by defining a new "Game Profile," this engine can be applied to different trading card games. It is meant to be modified or specialized to specific games to create different tools without the need to start from scratch.


Screenshots: H.E v5 and Gemini

Below are screenshots that demonstrate H.E v5 and how it affected the Gemini demos. Replace the image files in the `images/` folder with your actual screenshots (see instructions below) and the images will render here.

- ![H.E v5 — before applying changes](images/HE_v5_before.png)
  - Caption: Gemini output / behavior before H.E v5
- ![H.E v5 — after applying changes](images/HE_v5_after.png)
  - Caption: Gemini output / behavior after H.E v5
- ![H.E v5 — effect visualization](images/HE_v5_effect.png)
  - Caption: Key differences and notes (timing/resolution highlights)

How to add your screenshots (two simple options):

1) Using GitHub web UI (easiest — no coding required):
   - Go to the repository on GitHub and click "Add file" → "Upload files".
   - Create a new folder called `images/` (or navigate into it) and drag-and-drop your screenshot files.
   - Name them exactly `HE_v5_before.png`, `HE_v5_after.png`, and `HE_v5_effect.png` (or update the names in this README to match the files you upload).
   - Commit the change. The README will automatically show the images.

2) If you want me to upload them for you:
   - Reply here with the three screenshot image files (or share links to them). I can add them to the `images/` folder and update the README for you.

Notes and alt text

- Use PNG or JPG screenshots with at least 800px width for clear rendering on GitHub.
- Include short captions or annotations in the images (highlight the parts where H.E v5 changed Gemini's behavior — e.g., resolution order, log lines, or output text differences).

Core docs in this repo

- `UNIVERSAL CARD GAME RESOLUTION ORDE.txt` — UROE v2 / resolution order and timing rules.
- `UNIVERSAL CARD GAME THINKING MODEL.txt` — how the AI should reason about game states and actions.
- `STRESS-PROOF EDGE CASE LIBRARY v5.txt` — catalog of tricky edge cases and how the engine handles them.
- `dual personality framework for AI.txt` — design for dual-personality coaching/assistant agents.
- `prompt for AI chat bot v1.txt` and `prompt for AI chat bot v2.txt` — prompt templates used in demos.

License: MIT (see LICENSE file)
