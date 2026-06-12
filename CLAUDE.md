# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Type

This is a **documentation and content project** for a college extension course, not a software project. There are no build commands, test suites, or package managers. The repository contains text documents, PDFs, and Markdown files that support completing a project on the DreamShaper platform.

## Context and Purpose

The user is completing the college extension course **"Atividades de Extensão: Integração de Competências em Inteligência Artificial I"** (Cruzeiro do Sul Virtual / EAD, 2026/1º semestre, Prof. Douglas Almendro). The project must be developed entirely on the **DreamShaper** platform (cds-extensao-ea-desenvolvimento.dreamshaper.com), which requires answering questions **one at a time** in a sequential, interactive format.

The chosen project theme is a workshop called **"Desenvolver Software com IA e SDD"** about practical, beginner-friendly software development with AI-assisted workflows and structured delivery. The workshop focuses on:

1. **LLMs e contexto** — entender como essas ferramentas ajudam a gerar e revisar ideias
2. **SDD básico** — criar PRD, fases e tasks atômicos com clareza
3. **Execução passo a passo** — planejar, implementar, testar e validar cada tarefa

The goal is to replace the old community-mural framing with an educational workshop that shows how to build software with AI and SDD in a continuous, practical way.

## Repository Structure

All content lives under `docs/`:

- **`docs/`** — Current workshop notes, support material, and DreamShaper status for the new project
  - `docs/dreamshaper-status.md` — Record of confirmed answers and progress for the extension submission
  - `docs/Carta_de_Apresentacao_Extensao.docx` — Presentation letter for the extension project
  - `docs/Como Criar Projeto.pdf` — DreamShaper tutorial used to structure the submission

- **`docs/skills/explorar-planejar-executar/SKILL.md`** — Methodological skill framework (EPE: Explorar → Planejar → Executar). This is the formal definition of the "Itere" superpower as a 3-phase workflow with explicit commands (`/explorar`, `/planejar`, `/executar`).

- **`docs/Atividades de Extensão Integração de Competências em Inteligência Artificial I.pdf`** — Official course syllabus (Plano de Ensino 2026/1º semestre)

- **`docs/Carta_de_Apresentacao_Extensao.docx`** — Presentation letter for the extension project

- **`docs/Como Criar Projeto.pdf`** — DreamShaper platform tutorial showing how to create a project step by step

## Working Method

The user must answer DreamShaper questions **one by one**, copying each question from the platform and pasting it here. Claude assists in crafting the response, and the user copies it back into DreamShaper. This is an interactive, sequential workflow — the platform does not allow batch submission.

### Metodologia DreamShaper

For each DreamShaper question/request:
1. The user pastes the platform question/request. When copying from DreamShaper is difficult, the user may paste the page HTML instead.
2. If HTML is pasted, Claude must extract and distinguish the relevant DreamShaper content: topic/stage, question/request, selectable options, text fields, character limits, and any already saved answer. Ignore irrelevant markup/navigation whenever possible.
3. Claude identifies the topic/stage and drafts a response in **Portuguese (pt-BR)**, ready to copy into DreamShaper.
4. Before drafting the final answer, Claude should ask concise clarifying questions whenever real-world details are missing or would improve veracity (e.g. who attended, what happened, what reactions were observed, names, dates, locations, concrete examples). Do not over-question when enough context is already available; ask only what can materially improve the answer.
5. Claude should usually respond in this format: `Tópico identificado: ...`, `Perguntas rápidas:` when needed, `Resposta sugerida: ...`, and, when useful, `Observação: ...`.
6. If the platform shows a character limit, Claude must respect it and warn when the answer is close to the limit.
7. If the question has selectable options plus a text field, Claude must separate clearly: `Selecione:` and `Campo de texto:`.
8. The user may ask for refinements or respond positively (e.g. “sim”, “ok”, “boa”, “pode”, “confirmado”, “salva”, “é isso”, “fechou”). Any clear positive response counts as confirmation.
9. Only after confirmation, update `docs/dreamshaper-status.md` with a concise record.
10. The status file must contain: topic + short question, concise status, and concise final answer. Do not save rejected drafts.
11. The status must reflect what the user actually submitted or confirmed, not necessarily Claude’s first suggestion.
12. Before presenting final text for DreamShaper, use the local `.codex/skills/humanizer-br/SKILL.md` editorial guidance when available. The goal is to make answers sound natural in pt-BR, concise, concrete, and consistent with the user's voice, avoiding generic or mechanical phrasing.

When helping answer a DreamShaper question:
- First consult `docs/dreamshaper-status.md` if it exists, to preserve continuity with previous confirmed answers
- Read the current project notes in `docs/`, especially `docs/dreamshaper-status.md`, to extract facts that are already confirmed
- Read `docs/skills/explorar-planejar-executar/SKILL.md` when the answer involves the SDD workflow, the planning phases, or the way the workshop showed AI as an execution tool
- Treat the EPE flow (`/explorar` → `/planejar` → `/executar`) as the core educational method used in the workshop, with emphasis on practical delivery and testing
- Keep the tone realistic, concrete, and aligned with the new educational focus on software development with AI and SDD
- The target audience is beginners with no prior AI experience, in a small-city Brazilian context
- The primary case study is **Empório Princesa** in **Campanha, MG**, where the workshop was presented in a community setting
- All outputs should be in **Portuguese (pt-BR)**
- The workshop format was: in-person, around 1 hour, public audience, beginner level
- The presentation material is built with HTML + Reveal.js and should be described as part of the current project repository, without relying on old branding

## Key Reference Points

- **Workshop date:** January 22, 2026
- **Workshop location:** Empório Princesa, Campanha, MG
- **Workshop title:** "Desenvolver Software com IA e SDD"
- **Theme:** AI-assisted software development, PRD, phases, atomic tasks, tests, and a live to-do list demo
- **Format:** in-person workshop for beginners, around 1 hour
- **Main demonstration:** modern to-do list with search, dark mode, and cookie persistence

## Workshop Execution Result

The workshop was presented on January 22, 2026 at Empório Princesa, with a practical focus on LLM concepts, the three basic SDD files, and a step-by-step execution flow using tests. The live demo showed how a modern to-do list can be built and iterated with AI support.

When writing project deliverables for DreamShaper, reference the workshop as an educational extension activity focused on software development with AI and SDD, not as a donation or assistentialist action.

## Repository Metadata

- **Current repository:** this workspace, used to support the DreamShaper submission
- **Repo language:** Markdown and supporting documentation
- **Project focus:** educational workshop on AI + SDD for software development

## Language

All interactions and generated content must be in **Portuguese (pt-BR)**.
