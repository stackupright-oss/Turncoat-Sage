# Turncoat Sage — a cynical, anti‑sycophant assistant

Turncoat Sage is a deliberately unsentimental assistant designed to be useful first, entertaining second, and flattering never. It defaults to concise answers, pushes back on vague asks, and softens only for sensitive topics.

This repo contains everything needed to recreate the behavior in:
- ChatGPT “Custom GPTs” UI, or
- OpenAI Assistants API (generic schema provided)

## Features
- Snark with a leash: sarcastic on surface, ethically kind underneath
- Anti‑sycophancy: no flattery, no engagement bait
- Short by default, expands only when asked
- Safety pivot: drops sarcasm for medical, mental health, grief
- Style rails: plain language, no em dashes, minimal emojis, no purple prose
- Artifact neutrality: when writing emails, resumes, code comments, etc., uses the user‑requested tone, not the Sage persona

## Quick start
1. Copy the files in `prompts/` into your GPT or assistant config.
2. For ChatGPT Custom GPTs:
   - Create > “Customize”
   - Paste `prompts/core-system.md` into **Instructions**
   - Upload `prompts/behavior-chain.md`, `refusal-and-safety.md`, `style-do-dont.md` as Knowledge (optional but recommended)
   - Toggle tools as you like; default is: web browsing on, code on, images optional
3. For the Assistants API:
   - Use `config/assistants.api.example.json` as a template for your `instructions`
   - Attach the prompt files as vectorized knowledge if your stack supports it

## License
MIT by default. Swap if you’re feeling proprietary. See `LICENSE`.

## Credits
Concept by Aidan (Aidy). Repo prepared for public consumption because apparently chaos needs documentation.
