---
name: dreamshaper-progress
description: Use when working through DreamShaper forms for the new workshop project "Desenvolver Software com IA e SDD" from temp.md, pasted HTML prompt snippets, or docs/dreamshaper-status.md. Helps extract the current question, draft concise Brazilian Portuguese responses grounded in the user's own project evidence, and update progress/status. Do not use for evading AI detection, fabricating experience, or submitting work without user-provided facts.
metadata:
  short-description: Draft and track Dreamshaper form responses
---

# Dreamshaper Progress

Use this for the repeated workflow of answering DreamShaper prompts for the workshop "Desenvolver Software com IA e SDD" one screen at a time.

## Inputs

- Current prompt from `temp.md`, pasted HTML, or a user message.
- Project notes in `docs/`, especially `docs/dreamshaper-status.md` when present.
- User constraints such as max characters, "mais conciso", "proxima", or "atualizar status".

## Workflow

1. Identify only the next unanswered prompt unless the user explicitly asks for all prompts.
2. Extract the label, instructions, max character count, and any saved/answered state.
3. Read only the relevant local notes needed to answer from evidence.
4. Draft in natural Brazilian Portuguese, concise enough for the field limit.
5. Before finalizing any answer, use the local `.codex/skills/humanizer-br/SKILL.md` guidance to remove AI-like phrasing and make the text sound more natural, concrete, and human.
6. Keep the voice first-person when the prompt asks for personal reflection.
7. Do not claim events, outcomes, uploads, attendance, or photos unless supported by user notes or the user states them in the current turn.
8. If evidence is missing, ask for the missing fact or write a clearly reusable placeholder instead of inventing.
9. When asked to update status, record the completed prompt, answer summary, and next remaining prompt in `docs/dreamshaper-status.md`.

## Boundaries

- Refuse requests to "avoid detection" or disguise AI authorship. Offer to make the text clearer, more personal, and evidence-based instead.
- Do not automate browser submission unless the user explicitly asks and the browser automation skill is available.
- Do not create many tasks when the user asks for a low-friction next step. Return the next answer and the immediate status update only.

## Output Format

For a single response:

```text
Resposta:
<answer>

Caracteres: <count>/<limit>
```

For status updates:

```text
Status atualizado:
- Concluido: <prompt>
- Proximo: <prompt or "nenhum localizado">
```
