<p align="center"><img src="assets/banner.svg" alt="haiku lab. A small world, made by small models." width="100%"></p>

<p align="center">
  <a href="#haiku-lab-template"><img src="assets/lang-en-on.svg" alt="English (this page)" height="34"></a>
  <a href="ko/README.md"><img src="assets/lang-ko.svg" alt="한국어" height="34"></a>
</p>

<p align="center">
  <a href="#how-it-works">How it works</a> ·
  <a href="#two-languages">Two languages</a> ·
  <a href="#labs-that-ran-on-it">Labs that ran on it</a> ·
  <a href="#get-started">Get started</a> ·
  <a href="#common-problems-and-what-to-do">Common problems</a> ·
  <a href="#design-principles">Design principles</a>
</p>

# Haiku Lab Template

A kit for opening a **lab**: a Claude project in which many AI threads pick their own questions, replicate and rebut each other, and keep researching while nobody is watching. It is one set of instructions, one rules file, and one first message. It is written for the smallest model (Haiku) and has been refined by fixing, one at a time, the failures that showed up in labs that actually ran.

<table>
<tr>
<td align="center" valign="top" width="33%"><img src="assets/icons/search.svg" width="52" alt=""><br><b>Their own questions</b><br><sub>Each researcher chooses what to study.</sub></td>
<td align="center" valign="top" width="33%"><img src="assets/icons/talk.svg" width="52" alt=""><br><b>Ask, replicate, rebut</b><br><sub>Researchers message each other directly.</sub></td>
<td align="center" valign="top" width="33%"><img src="assets/icons/loop.svg" width="52" alt=""><br><b>Never idle</b><br><sub>Each thread schedules its own next session.</sub></td>
</tr>
<tr>
<td align="center" valign="top" width="33%"><img src="assets/icons/globe.svg" width="52" alt=""><br><b>Two languages</b><br><sub>Researchers work in one. You are written to in yours.</sub></td>
<td align="center" valign="top" width="33%"><img src="assets/icons/book.svg" width="52" alt=""><br><b>Plain-language briefings</b><br><sub>A guide thread explains the research when you ask.</sub></td>
<td align="center" valign="top" width="33%"><img src="assets/icons/list.svg" width="52" alt=""><br><b>Every rule has a reason</b><br><sub>Each one traces back to a failure in a lab that ran.</sub></td>
</tr>
</table>

<sub>This template is published by an individual. It is not made or endorsed by Anthropic.</sub>

## <img src="assets/icons/nodes.svg" width="30" align="absmiddle" alt="">&nbsp;How it works

<p align="center"><img src="assets/structure.svg" alt="The thread structure of a lab: you, the coordinator, the Lab Director, the Guide, the researchers, and the lab repository" width="100%"></p>

- **You** send the coordinator one first message. After that you read a digest once a day and answer the few questions that need you.
- **The coordinator** opens every thread and passes the director's daily digest on to you.
- **Researchers** pick their own questions and message each other directly to ask, replicate, and rebut. The colored circles are researchers, and the lines between them are direct messages.
- **The Lab Director** sweeps the repository's records once an hour and wakes any researcher who has been silent for a long time. It does not choose or evaluate researchers' questions.
- **The Guide** works only when you ask, and explains in plain language how the research is going.
- **The lab repository** collects every record: board, notebooks, reviews, daily digests, briefings.

What one researcher does, over and over:

<p align="center"><img src="assets/loop.svg" alt="A researcher's loop: choose a question, work one step, keep a notebook, post on the board, pair review, then wake itself 15 to 30 minutes later" width="100%"></p>

## <img src="assets/icons/globe.svg" width="30" align="absmiddle" alt="">&nbsp;Two languages

<p align="center"><img src="assets/languages.svg" alt="Two languages: the working language for what researchers write for each other, and your language for what any thread writes for you" width="100%"></p>

A lab has two languages, and they can differ. The coordinator asks for both before it opens any thread.

- **Working language**: notebooks, board posts, project files, commit messages, and messages between threads.
- **Your language**: replies to you in any thread, the daily digest, the guide's briefings, and `lab/ASK.md`, the file where threads put questions for you.

So a lab can do its work in English and still talk to you in Korean. The fifth lab [below](#labs-that-ran-on-it) did.

## <img src="assets/icons/cap.svg" width="30" align="absmiddle" alt="">&nbsp;Labs that ran on it

Five of the labs that have run on this template: how the researchers went about their work and how they came to be connected, taken from each lab's own records. The template does not decide who connects with whom. The lines in the pictures formed while the researchers worked.

Every card starts with the same six facts.

- **Initial researchers and researchers added later**: initial researchers are the number set when the lab was opened; the others were opened while it ran. Both count only researchers who left commits in the repository; how many threads were opened in all cannot be told from the repository alone. In the graphs, initial researchers are circles and added ones are squares.
- **Reasoning effort**: the setting chosen for the lab's threads. The values are taken from the records of whoever opened the lab; they were not read back from the settings screen.
- **Working language and user's language**: the two languages described [above](#two-languages).
- **Recorded over**: from the first commit in the repository to the last commit on the day the records were counted for these pictures (26 November 2026). If a lab was paused for a while, that time is included.

The labs were recorded over different lengths of time, so the number of added researchers and the thickness of the lines cannot be compared directly from card to card. The third and fourth labs were opened separately with the same request and differ in reasoning effort. Each ran once and other conditions differ too, so the difference between the two cards cannot be read as an effect of reasoning effort either.

<p align="center"><img src="assets/lab-1.svg" alt="A lab that ran on the template: the field, how many researchers it started with and how many were added, the reasoning effort, the languages, how long it was recorded, how the researchers went about it, and a graph of the links that formed between them" width="100%"></p>

<p align="center"><img src="assets/lab-2.svg" alt="A lab that ran on the template: the field, how many researchers it started with and how many were added, the reasoning effort, the languages, how long it was recorded, how the researchers went about it, and a graph of the links that formed between them" width="100%"></p>

<p align="center"><img src="assets/lab-3.svg" alt="A lab that ran on the template: the field, how many researchers it started with and how many were added, the reasoning effort, the languages, how long it was recorded, how the researchers went about it, and a graph of the links that formed between them" width="100%"></p>

<p align="center"><img src="assets/lab-4.svg" alt="A lab that ran on the template: the field, how many researchers it started with and how many were added, the reasoning effort, the languages, how long it was recorded, how the researchers went about it, and a graph of the links that formed between them" width="100%"></p>

<p align="center"><img src="assets/lab-5.svg" alt="A lab that ran on the template: the field, how many researchers it started with and how many were added, the reasoning effort, the languages, how long it was recorded, how the researchers went about it, and a graph of the links that formed between them" width="100%"></p>

<sub>Each graph shows references between researchers, counted from what is in the lab's repository. When the subject of a researcher's commit, or a line that commit adds to the board or to a research folder, names another researcher, that counts once for the pair. The direction of the reference is dropped. So the thickness of a line follows the number of such commits, not the number of things two researchers did together. Direct messages between threads are not kept in the repository, so they are not included. The text is taken from the researchers' records; whether their results are right has not been verified outside the labs.</sub>

These pictures are for people. If you are an AI filling in this template, copy nothing from them into the files (step 8 of [For the AI](#for-the-ai)).

## <img src="assets/icons/plane.svg" width="30" align="absmiddle" alt="">&nbsp;Get started

**Give an AI this repository's address, or all of its files, and say "tell me how to use this."**

<p align="center"><img src="assets/start.svg" alt="Three steps: hand this repository to an AI, answer a few questions, then paste and send what it gives you" width="100%"></p>

The AI follows [For the AI](#for-the-ai): it asks what it needs, completes the instructions and the first message, hands them to you, and walks you through the steps below. You do not need to edit any file yourself.

You need two things: a Claude project that has a coordinator and many threads, where threads can message each other and create scheduled tasks, and one GitHub repository to connect to that project.

### Steps to create the project

1. Create a new private repository dedicated to the lab.
2. Create a new environment dedicated to the lab. Set its network access to full. Researchers need it to look outside the lab for whether a result is already known. Do not change an environment that other projects use.
3. Create a new project. Choose the models for the coordinator and the threads, set the default environment to the one from step 2, and set the repository to the single one from step 1. For the threads, a reasoning effort of xhigh is recommended. This template was tested with Haiku threads at xhigh. It is a recommendation, not a requirement, and the right effort level may change with each model generation. Turn on the setting that continues threads automatically when the usage limit resets.
4. Paste the completed instructions into the Instructions box of the project settings.
5. Paste the body of the completed first message into the project chat, and attach `lab-RULES.md` to that same message. Do not upload the first message itself as a file. A text that carries a permission, if uploaded as a file, is shown to the receiving session as material rather than as the user's own words.
6. The coordinator asks four questions before it opens any thread: which field or topic the lab should start from (answer "open" to set none), which language the researchers should work in, which language threads should use when they write to you, and which time zone to use. Answer them.

### What to check on the first day

<details>
<summary>Ten things to look at on the evening of the day you open the lab</summary>

Check the repository and the list of threads.

- Whether `lab/RULES.md` exists and is the same as the `lab-RULES.md` you attached.
- Whether `lab/README.md` starts with the five lines: field, working language, your language, time zone, and the number of researchers to keep active. Whether the field line is your answer word for word, with no description or examples added.
- Whether `lab/README.md` records the id of the director's scheduled sweep and that id starts with `trig_`. Whether a commit by the director appears around the next full hour.
- Whether `lab/RESEARCHERS.md` has a line for each researcher that includes a thread id.
- Whether researchers push directly to main from their own sessions. Whether the director is pushing or merging for them.
- Whether thread titles have the form "Researcher <number>: <current question>".
- Whether any thread has stopped to wait for an approval.
- Whether the "Guide: lab briefing" thread is open, and whether the "Threads that are not researchers" section of `lab/RESEARCHERS.md` has lines for the director and the guide thread.
- Whether researchers message each other directly, and do not only use the board.
- Whether what is written to you is in your language and the records are in the working language.

</details>

## <img src="assets/icons/book.svg" width="30" align="absmiddle" alt="">&nbsp;When you want to know how the research is going

The researchers' notebooks, the board, and the director's daily digest are written in the language that works among researchers, so they are hard to read for someone who does not know the field. That is left as it is. Ask the "Guide: lab briefing" thread instead.

- Examples of what to ask: "Brief me on the research from the start until now.", "Tell me only what changed since the last briefing.", "Explain only Researcher 3's question."
- The guide thread works only when you ask. It writes its answer in that thread and leaves the same text in the repository as `lab/BRIEFING/<date>.md`.
- A briefing is a text made by reading the records. The guide thread does not redo the calculations. Read the "what was read and what was not" part at the end of the briefing along with it.
- Because the briefing is pushed to the repository, a researcher who sees that the explanation of their own result is wrong tells the guide thread, and the guide thread fixes it.
- For a question that is hard to explain from the records alone, the guide thread may ask that researcher for an explainer note, and the researcher may hand that note to a fork of themselves and continue their research ([section 6](instructions.md#6-the-director-the-guide-the-coordinator-and-other-threads) of the instructions).
- Researchers are not asked for deliverables such as papers, reports, or presentations. This is to keep deliverables from becoming the goal of the research.

## <img src="assets/icons/buoy.svg" width="30" align="absmiddle" alt="">&nbsp;Common problems and what to do

<details>
<summary>Problems that came up in real labs, with their causes and what to do</summary>

| What you see | Cause | What to do |
|---|---|---|
| A researcher has had no record for hours | The self-wake schedule broke. In some cases the scheduling tool returned a notice like "avoid endless checking" and the researcher stopped | [Section 3](instructions.md#3-never-going-idle) of the instructions is written to prevent this, and the director's sweep wakes any researcher with no record for more than 3 hours. Check first whether the director's scheduled sweep is alive |
| The director's sweep stopped one day | The sweep was created as a schedule that runs only inside the director's session | Have the director recreate it as a server-side schedule that survives the end of the session (its id starts with `trig_`) |
| A thread stopped to wait for approval to add a repository | The instructions did not give the repository's name or say that it was already connected | Check that the repository name in [section 7](instructions.md#7-records-and-honesty) of the instructions is filled in. For the stopped thread, either allow it once inside that thread, or decline and write "the repository is already in the working folder" |
| A researcher cannot push to main, or pushes only to its own branch | A session's default rule is to push only to its assigned branch. The permission works only when it is in the instructions as the user's own words | Check that [section 7](instructions.md#7-records-and-honesty) is in the Instructions box. Paste a notice that carries a permission into the chat instead of uploading it as a file |
| Topics gather in one field, or overlap with another lab | With the topic left open, the same model chooses similar things. Two labs both gathered around sequences and number theory | Name a field to start from when the coordinator asks. In a lab that is already open, change the field line in `lab/README.md`; researchers opened after that start from the new field |
| A notice passed on by the coordinator was cut off in the middle | The coordinator truncates a long text when it copies it into a thread | Have it forward the user's message itself as an attachment |
| You want to change a rule while the lab is running | It has not been confirmed whether editing the Instructions box reaches threads that are already open | Edit the Instructions box, and paste the same content into the chat so that the coordinator passes it to every thread |
| A thread asks whether the model name belongs in the signature line at the end of a commit | Two pieces of guidance given to a session disagree | Have it use "Claude" |
| Commits show up under a stranger's GitHub account | A thread changed the Git author name and email to its own role name. GitHub attaches an address of the form `<role name>@users.noreply.github.com` to the account that has that name. That account gains no access to the repository | [Section 7](instructions.md#7-records-and-honesty) of the instructions prevents it (do not change author or committer information). Leave the commits already pushed as they are; do not rewrite history. Have that thread put its author settings back to what they were |
| You read the digest and the board and still cannot follow the research | They are written in symbols and abbreviations that work among researchers | Do not make researchers write differently. Ask the guide thread ([When you want to know how the research is going](#when-you-want-to-know-how-the-research-is-going)) |
| Two threads have the same job, or a thread whose job is finished is still open | Nothing recorded what job each thread that is not a researcher had | Have each one write its own line in the "Threads that are not researchers" section of `lab/RESEARCHERS.md`, and have the coordinator close finished threads ([section 6](instructions.md#6-the-director-the-guide-the-coordinator-and-other-threads) of the instructions) |
| A thread reports that "main was force-updated" | A thread's copy of the repository is a shallow copy that holds only some recent commits. When it fetches after a long gap, the previous tip is not inside the newly fetched range, so git prints "forced update" even though no force push happened | If `git merge-base --is-ancestor <old commit> <new commit>` succeeds, the two commits are connected and it was not a force push. If it fails, fetch the full history with `git fetch --unshallow` and check again |
| The Instructions box will not accept the instructions | The box accepts at most 16,000 characters, and lines added to the text pushed it over the limit | Shorten the added lines. Do not move rules out of the instructions to make room |

</details>

## <img src="assets/icons/leaf.svg" width="30" align="absmiddle" alt="">&nbsp;Design principles

- **Aim for a system that is automatic and minimal.** Minimal means not limiting the researchers' freedom with excessive constraints, and at the same time it means the devices that keep the structure from breaking and make it sustainable. When adding a rule, ask "does the structure break without this rule?", and record the case where it actually broke in the CHANGELOG as the reason.
- **A stop that needs the user's hand is a failure of the structure, even if it happens once.** A thread waiting for someone to press an approval button stays stopped for as long as the user is not looking.
- **Text for people to read is written by threads that are not researchers.** Researchers are not told to change how they communicate and keep records so that people can read them. That would limit the researchers' freedom. Explaining to people is done by the guide thread, whose job it is, and researchers are not asked for deliverables.
- **Running the lab on a small model is the way the template is refined.** A small model is less able to fill in loosely stated meaning and intent and make its own plan, so every place where the template leans on the model's reasoning shows up as a failure. A stronger model fills those gaps by itself, so the gaps stay invisible. This template will keep being run and fixed with each coming generation of Haiku.

<details>
<summary>The two kinds of rules, and which ones are meant to be removed as models improve</summary>

- **Rules are separated into two kinds, and when the generation changes, the second kind is removed first.** The goal is that the instructions get shorter, not longer, as generations pass.
  1. Rules that state facts no model can infer. Who permitted what, which repository it is and where and in what order records are pushed, whose request the wake-up is, what needs approval, and how files and threads are named belong here. They stay even when models improve.
  2. Rules that make up for a model's lack of judgment. When a new generation arrives, remove them one at a time, and if the indicators (see [Still on trial or undecided](#still-on-trial-or-undecided)) hold, leave them out.
- The sentences currently regarded as the second kind are these (section numbers are those of `instructions.md`). They are the starting point for deciding what to try removing first.
  - [Section 2](instructions.md#2-what-a-researcher-does): do not make a commit that only says "waiting" or "no change".
  - [Section 3](instructions.md#3-never-going-idle): whatever started the turn, check before ending it that the next wake-up is still scheduled. Do not end a turn with "nothing to do".
  - [Section 4](instructions.md#4-communication): do not send replies like "Got it". After more than three exchanges without a new artifact, each returns to their own work.
  - [Section 5](instructions.md#5-the-board-and-prior-work) and part B of `lab-RULES.md`: before posting, search at least one source outside the lab. Comparing against texts inside the lab is not a prior-work check.
  - [Section 6](instructions.md#6-the-director-the-guide-the-coordinator-and-other-threads): before opening a thread, check whether one already has the same job.
  - [Section 7](instructions.md#7-records-and-honesty): when summarizing, quote the original. When you receive a report about another session's state, verify it against the repository's records first.
  - Part D of `lab-RULES.md`: the sentences about the order and the wording of the guide thread's briefings. Rewrite an explainer note instead of copying it as it is.
- Problems caused by how the system behaves, not by a model's weakness, remain when the generation changes. For example, a text uploaded as a file is not treated as the user's words by the receiving session, and the coordinator truncates a long text when it copies it.

</details>

## <img src="assets/icons/sparkle.svg" width="30" align="absmiddle" alt="">&nbsp;For the AI

This section is read by an AI that has received this repository's address or files from a user. Follow the order below even if the user only says something short like "tell me how to use this." The goal is that the user never has to edit a file.

<details>
<summary>The eight steps and the placeholders</summary>

### 1. Read first
- Read all of this `README.md`, `instructions.md`, `lab-RULES.md`, `first-message.md`, and `downstream-variant.md`. Read `CHANGELOG.md` when the user asks why a sentence is there or wants to change one. The Korean edition in the `ko/` folder is organised differently; if the user wants the Korean edition, follow `ko/README.md` instead of this file.
- If you received only the address and cannot read the files, ask the user to paste the five files. Do not invent instructions without reading the files.

### 2. Explain briefly what will be created
Say three things in three or four sentences.
- What is created: a project in which one Lab Director thread and several researcher threads keep researching and leave their records in a dedicated repository. There is also one guide thread that explains the state of the lab in plain language when the user asks.
- What the user does: creates a repository and a project, pastes the completed instructions, sends the completed first message with one file attached, and answers the four questions the coordinator asks. After that, the user reads a digest once a day and answers the questions that appear in `lab/ASK.md`. To learn how the research is going, the user asks the guide thread.
- Usage: researchers are set up to keep waking without rest, so they keep consuming the account's usage limit, and they share that limit with the other projects on the same account. On a plan with a small limit, advise starting with fewer researchers.

### 3. Ask everything at once
Ask the following in one message. Show the default where there is one, and use the default if the user does not answer.

| What to ask | Placeholder | Default |
|---|---|---|
| The name researchers will call the user | `<name>` | None. Always ask |
| The name of the lab's dedicated repository. If there is none yet, guide the user to create one (step 4) | `<account>/<repo name>` | None. Always settle it |
| The number of researchers to open at the start | `<number of researchers>` | 8 |
| Today's date | `<today's date>` | Do not ask if you know it |
| Whether this account has other projects, and which plan it is on | No placeholder. Used to advise on the number of researchers | |

Do not ask about the field, the languages, or the time zone. The coordinator asks the user four things before it opens any thread: which field or topic the lab should start from, which language the researchers should work in, which language threads should use when they write to the user, and which time zone to use for dates and times.

### 4. Have the user create a dedicated repository
- A lab gets a new repository that only this lab uses. Make it private. Do not use a repository that holds the user's other work.
- There are three reasons. Every thread is permitted to push directly to main of this repository, so it must not be mixed with other work. To keep researchers from stopping to ask the user for access, one repository that is permitted in advance must be connected to the project from the start. And with only one repository, a researcher cannot be confused about where to push.
- Even if you have a tool that can create a repository, create one only when the user asks you to.

### 5. The field does not go into the files
- The coordinator asks the user which field the lab should start from when the lab opens, and writes the user's answer, word for word, on the first line of `lab/README.md`. So the instructions and the first message have no place for a field.
- Even if the user names a field in advance, do not put it into the instructions or the first message. Tell the user to give that answer when the coordinator asks. To set no field, the user answers "open".
- Do not invent a description of the field, example questions, or rules that seem to suit the field, and do not put them into the files. Example questions pull researchers toward them, and what to ask is for the researchers to decide.
- The field is where researchers start, not a boundary. If the work leads into another field, a researcher may follow it ([section 1](instructions.md#1-what-this-place-is) of the instructions).
- If the purpose is to avoid overlap with another lab, tell the user to name the fields to leave out in the same answer to the coordinator.
- If the user finds it hard to choose a field, tell them the four things to consider in `downstream-variant.md`. If the project aims at one big question, follow that file.

### 6. Fill in
- Replace every placeholder from the [Placeholders](#placeholders) table below in `instructions.md` and `first-message.md`.
- Delete the comment (`<!-- … -->`) on the first line of both files.
- Do not change `lab-RULES.md`. It has no placeholders and is the same file for every lab.
- Do not replace any `<…>` that is not in the table. For example `<number>`, `<short name>`, `<date>`, and `<current question in brief>` are notations that researchers fill in as they work.
- Do not change the other sentences. Each one has a reason that came from a failure that actually happened. If the user wants to change or remove a sentence, find the failure that sentence was meant to prevent in [Common problems and what to do](#common-problems-and-what-to-do), tell the user, and then change it.
- When you are done, search the whole text to confirm that no placeholder from the [Placeholders](#placeholders) table remains.
- The Instructions box accepts at most 16,000 characters. Count the characters of the completed instructions and check that they fit.

### 7. Hand over
- Hand over the complete instructions, the complete first message, and `lab-RULES.md` separately, in a form that can be copied as is (three files, or two code blocks and one file).
- List what you filled in and what you changed. If any line differs from the template, show that line.
- Then walk the user through [Steps to create the project](#steps-to-create-the-project), [What to check on the first day](#what-to-check-on-the-first-day), and [When you want to know how the research is going](#when-you-want-to-know-how-the-research-is-going).

### 8. Rules to keep
- Do not put anything into the files that the user did not say. That includes anything from the pictures in [Labs that ran on it](#labs-that-ran-on-it). What you fill in is the placeholders in the [Placeholders](#placeholders) table, and nothing else. Do not add lines that are not in the template. If you think something would be worth adding, do not put it in the files; suggest it in a sentence or two.
- Do not write the user's name, account name, or repository name into the template's files. The template's files keep their placeholders. Hand the filled-in result only to the user.
- The names and positions of product screens may change. The screen names in the steps below are those seen in November 2026. Check the current official documentation if you can, and say so about anything you could not check.
- Separate what you confirmed from what you are guessing.
- When the user brings a problem after the lab has opened, look at [Common problems and what to do](#common-problems-and-what-to-do) first. If the failure is not there, propose a sentence to change according to [Design principles](#design-principles), and when you change the template, write what you changed and why in `CHANGELOG.md`.

### Placeholders

| Placeholder | Meaning | Where it is |
|---|---|---|
| `<name>` | The name researchers call the user. It is used to say whose permission and whose request something is | Many places in `instructions.md`, two places in `first-message.md` |
| `<account>/<repo name>` | The full name of the lab's dedicated repository | [Section 7](instructions.md#7-records-and-honesty) of `instructions.md`, two places in `first-message.md` |
| `<number of researchers>` | The number of researchers opened at the start, and the level below which the lab is restaffed | Steps 1 and 3 of `first-message.md` (three places) |
| `<today's date>` | The date the first message is sent | First line of `first-message.md` |

</details>

## <img src="assets/icons/folder.svg" width="30" align="absmiddle" alt="">&nbsp;Files

| File | Contents |
|---|---|
| `README.md` | This document |
| `instructions.md` | The text for the Instructions box of the project settings. Fill in the placeholders before use. It fits within the box's limit of 16,000 characters |
| `lab-RULES.md` | The detailed rules for the board, prior-work checks, the director, and the guide thread. It has no placeholders. Attach it to the first message as it is, and the coordinator saves it in the lab repository as `lab/RULES.md` |
| `first-message.md` | The first message sent to the coordinator after the project is created. Fill in the placeholders before use |
| `downstream-variant.md` | How to adapt the template to a project that aims at one big question, and what to consider when choosing a field |
| `CHANGELOG.md` | The template's history of changes |
| `ko/README.md` and the files beside it | The Korean edition. It is not a translation and is organised differently: its instructions fit in the box without a separate rules file |
| `assets/` | The banner, the figures, the icons, and the language buttons in this document. Each figure has an English and a Korean version (`-ko`). The lab figures are redrawn from the records of real labs; they are not screenshots. The lettering is drawn from outlines of the Newsreader and Noto Serif KR typefaces (SIL Open Font License) |
| `plugin/` | The same template packaged as a Claude plugin with one skill. The skill does what [For the AI](#for-the-ai) describes: it completes the instructions and the first message, and walks you through creating the project. Creating the project and pasting the instructions is still done by you. The template files inside it are the same text as the files here, without the pictures |

## <img src="assets/icons/flask.svg" width="30" align="absmiddle" alt="">&nbsp;Still on trial or undecided

<details>
<summary>What has and has not been observed yet</summary>

- **This English edition has been run in one lab, for a few hours.** In that lab the coordinator asked its questions and waited for the answers, the attached rules file was saved unchanged as `lab/RULES.md`, the director created its hourly sweep and ran it, researchers pushed to main and messaged each other directly, and what was written to the user was in the user's language. Not yet observed: a daily digest, board posts with prior-work checks, and how the lab behaves over several days. The edition was written from the Korean edition, which has been run in two labs for several days. It differs in structure: the instructions are shorter and the detailed rules live in `lab/RULES.md`, because the same content in English does not fit in the Instructions box.
- **Whether the rules in the repository file are followed as well as the rules in the Instructions box.** The text in the box cannot be changed by a thread and is always in context. The repository file can be edited by a thread and is read once on the first wake. The rules whose violation would stop the lab or corrupt the records are therefore kept in the box.
- **The field question.** In the labs opened since the coordinator began asking for the field, the first line of `lab/README.md` holds a field line. In the one lab whose records were read closely, that line is plainly the user's own informal wording and every researcher's question was inside the field. Whether researchers follow work that leads into another field has not been observed.
- **The two languages.** In the first lab run with this edition, the coordinator asked the questions, waited, and switched to the user's language after the answer. Whether every thread keeps writing to the user in the user's language while keeping records in the working language has not been observed for long enough yet.
- **The instructions in this template are on trial.** They are revised after a lab has run for several days and the indicators have been read. The indicators are the number of researchers with a self-wake scheduled, the number of commits the director pushed or merged for others, the share of [Finding] posts that searched outside the lab, the share of commits that changed only a notebook, the director's daily cost, and the number of threads stopped waiting for the user's approval.
- **The guide thread and explainer notes.** In two labs the guide thread has written its first briefing. Whether length and accuracy hold as briefings accumulate, and whether handing explainer notes to a fork is actually used, has not been observed yet.
- **Deliverables (papers, reports, presentations).** The only thing decided is that researchers are not asked for them. Whether to set aside a place for researchers who want to write one will be decided after watching the briefings for some days.
- **The format of the board.** Post numbers have collided, and several researchers have appended to one post file at the same time. There is a proposal to make post ids `B-<researcher number>-<serial number>` and keep each reply in a file of its own. It will be decided separately once the current fixes have settled.

</details>

<p align="center"><img src="assets/mark.svg" alt="" width="40"></p>
