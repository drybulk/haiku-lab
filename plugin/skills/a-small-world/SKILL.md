---
name: a-small-world
description: Set up a self-running research lab, a Claude project in which a director thread, a guide thread, and several researcher threads keep doing research on their own and record it in a dedicated GitHub repository. Use when the user asks to open, start, or set up such a lab, asks how to use the bundled lab template, or brings a problem with a lab that was opened from it.
---

# A Small World

A lab is a Claude project, not something that runs inside this conversation. This skill prepares what the user needs to open one and walks them through opening it.

## What you can and cannot do

- You complete two texts from the bundled template: the project instructions and the first message. In the English edition you also hand over one file, `lab-RULES.md`, unchanged.
- You cannot create the project, paste into its Instructions box, send its first message, or open its threads. The user does those. Say this at the start so the user knows what to expect.
- Create a GitHub repository only if the user asks you to and you have a tool for it.

## The template is bundled with this skill

Everything is under `template/` in this skill's folder. Nothing needs to be downloaded, and the user does not need to paste any file.

| Edition | Start from | Files you complete | File you hand over unchanged |
|---|---|---|---|
| English | `template/README.md` | `template/instructions.md`, `template/first-message.md` | `template/lab-RULES.md` |
| Korean | `template/ko/README.md` | `template/ko/instructions.md`, `template/ko/first-message.md` | None |

- The English edition keeps two languages apart: the language the researchers work in, and the language threads use when they write to the user. A lab opened from it can work in English and still write to the user in another language.
- The Korean edition is not a translation. It is organised differently, and everything in a lab opened from it is in Korean.
- Use the English edition unless the user asks for the Korean one. If the user writes to you in Korean, tell them in one sentence that both editions exist and how they differ, and let them choose.
- `template/downstream-variant.md` (and `template/ko/downstream-variant.md`) is for a project that aims at one big question, and for a user who finds it hard to choose a field. `template/CHANGELOG.md` (and `template/ko/CHANGELOG.md`) records why each sentence of the template is there.
- The bundled READMEs are the published ones with their pictures removed. Where a README mentions a picture, there is nothing to open.
- The bundled files call the lab by the template's original name. It is the same thing this skill sets up.

## What to do

1. Read the README of the chosen edition in full, then the other files of that edition.
2. Follow that README's section for the AI ("For the AI" in English, "AI에게" in Korean) step by step. That section is the procedure, and this file does not repeat it. Where it says to ask the user to paste the files, skip that: you already have them.
3. Hand over the completed instructions and the completed first message in a form the user can copy as they are (two files, or two code blocks). For the English edition, also hand over `lab-RULES.md` as a file. Then walk the user through the README's steps to create the project.

## Rules that are easy to break

The README's section for the AI gives these in full. They are repeated here because breaking them damages the lab.

- Put nothing into the texts that the user did not say. Fill in the placeholders listed in the README and change nothing else. If you think something is worth adding, suggest it to the user in a sentence or two; do not write it into the texts.
- Do not ask the user about the field of research, and do not write a field, example questions, or field-specific rules into the texts. The project's coordinator asks the user about the field when the lab opens. The English edition's coordinator also asks about the two languages and the time zone, so do not ask about those either.
- Do not edit the files under `template/`. Write the completed texts as new files or as code blocks.
- The first message must be pasted into the project chat as text. Tell the user not to upload it as a file.
- Write to the user in the user's language.
- The names and positions of product screens change. Say which steps you could not check against current documentation.

## When the user comes back with a problem

Look in the README's section on common problems first ("Common problems and what to do", "자주 생긴 문제와 대처"). If the failure is not there, say so, and propose a change that follows the README's design principles. Do not guess a cause.
