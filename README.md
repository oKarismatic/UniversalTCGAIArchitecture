Status: Early design prototype. I'm learning — this repository contains architecture docs and prompt templates but does not include a production implementation yet. Contributions and mentoring are welcome.

This project will be updated over time; availability varies. Feel free to fork the repo and start your own experiments.

UniversalTCGAIArchitecture
Modular AI framework for TCG logic, featuring the UROE v2 resolution engine, robust edge-case handling, and dual-personality coaching agents.

Short description My brother and I built this system because we were frustrated by AI tools that struggle with complex trading-card-game logic, timing, and rules. This engine is a deterministic state machine that separates game rules from execution logic. By defining a "Game Profile" the engine can be adapted to different TCGs.

Demo (Gemini H.E v5) Demo link: https://gemini.google.com/share/8855159d1161 Usage notes: When using the shared demo, first state the game name (e.g., "Yu-Gi-Oh!", "Magic: The Gathering"), then state the format (e.g., "Standard", "Commander"), and finally paste the game state or prompt you want the model to evaluate. Example:
Currently tired i will update this later demo above is outdated here is the new link and below a few prompts https://gemini.google.com/share/09780afc8585 wierd thing my brother found we could do https://gemini.google.com/share/0b504f005117

Must use this format for decks:      if error's start to occur: /reanchor (this needs heavy testing)
[DECK_ID: Red_Burn_v1]                                          reanchor [DECK_ID: Naya_Midrange]
<DECK_START>
4 Lightning Bolt
4 Goblin Guide
...
<DECK_END>

Game: Magic: The Gathering — Format: Standard — Prompt: "Resolve a turn where..."


<img width="1842" height="994" alt="Screenshot 2026-06-03 053957" src="https://github.com/user-attachments/assets/e8d0a2f7-1e4c-4d55-b4e0-7eeb6ecaf886" />
<img width="1792" height="956" alt="Screenshot 2026-06-03 064531" src="https://github.com/user-attachments/assets/cfca6145-b54f-40cd-8794-50428646cbec" />
<img width="1595" height="949" alt="Screenshot 2026-06-03 064706" src="https://github.com/user-attachments/assets/782fa2ca-c09c-421b-a97e-8f36c790561e" />
<img width="1535" height="944" alt="Screenshot 2026-06-03 064841" src="https://github.com/user-attachments/assets/17481b6d-c92d-45e0-a7a8-d5f1f5913f06" />
<img width="1581" height="877" alt="Screenshot 2026-06-03 065038" src="https://github.com/user-attachments/assets/fef8fdd8-750d-462b-8bb0-a8a87603aa1e" />
<img width="1467" height="940" alt="Screenshot 2026-06-03 065206" src="https://github.com/user-attachments/assets/ec04df7f-0beb-4478-837b-45e948783ee6" />
<img width="1581" height="948" alt="Screenshot 2026-06-03 065435" src="https://github.com/user-attachments/assets/0940c7a8-090c-4dc5-aac9-511acc3b23a3" />
