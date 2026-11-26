# Changelog

What changed in the published template, and why. The Korean edition keeps a more detailed record in `ko/CHANGELOG.md`.

## 2026-11-26 Lab cards redrawn: how they worked and how they connected
- The cards under "Labs that ran on it" were redrawn, and there are now five instead of four. The earlier cards listed details of the research (question titles, figures) that a first-time reader could not follow.
- Each card now says in plain words how the researchers went about their work, and gives three ways they came to be connected.
- Each card has a graph. Circles and squares are researchers (a circle was there when the lab opened, a square was added while it ran); a line means one researcher's records name the other. The lines are counted from the commits in the lab's repository (once per commit whose subject or added lines name another researcher, direction dropped), and thickness follows the count. It is not a count of joint work. The README states this rule under the pictures. Direct messages between threads are not kept in the repository and are not counted.
- Every card starts with the same six facts in the same order: initial researchers, researchers added later, reasoning effort, working language, user's language, and how long the lab was recorded. The README says how each is counted: researchers are those who left commits, reasoning effort comes from the records of whoever opened the lab, and the span runs from the first commit to the last one on the day of counting (2026-11-26). These labels carry no color; pink and teal are used only for researchers in the graph and the numbers that point to them.
- A second fantasy web-novel lab was added. It was opened separately with the same request as the first and differs in reasoning effort. Each ran once and other conditions differ too, so the difference between the two cards cannot be read as an effect of reasoning effort. The README says so.
- The lists of question titles were removed from the cards.

## 2026-11-25 README rearranged for people
- Both READMEs were rearranged. The instructions, the first message, and the rules file did not change.
- What a person looks at first now comes first: how it works, two languages, labs that ran on it, get started. Long reference parts (first-day checks, common problems, the two kinds of rules, the eight steps for the AI and the placeholders, what is still on trial) keep their headings but have their bodies folded. The folded text is still in the file, so an AI reads all of it as before.
- Every place that refers to another section now links to it. References to a section of the instructions link to that section of `instructions.md`.
- The lettering in the figures is larger. Body text in a figure no longer falls below 14 pixels on screen (the one-line source note under each lab card is 13).
- Every figure has a Korean version (files ending in `-ko`), used by the Korean README. The Korean README also uses a banner with a Korean tagline (`assets/banner-ko.svg`).
- New section and figure "Two languages": the working language researchers write in for each other, and the language threads use when they write to you, are set separately.
- "An example lab" became "Labs that ran on it": four labs, one card each, with an overview (field, number of researchers, languages), three things that stood out, and three of the questions the researchers chose. The cards are redrawn from each lab's records. The researchers' reported results have not been verified outside the labs.
- The row of feature cells under the introduction grew from four to six.
- The entry about the field question in "Still on trial or undecided" was updated with what was seen in labs opened that way.

## 2026-11-25 Icons and figures
- Both READMEs now carry icons and figures. The instructions, the first message, and the rules file did not change.
- Icons (`assets/icons/`): seventeen line drawings on rounded tiles, in the banner's pink and teal only. The tiles are translucent, so the same files work on light and dark pages. They sit before section titles and in the four-cell row under the introduction.
- Three figures: the three steps of using the template (`assets/start.svg`), the loop one researcher repeats (`assets/loop.svg`), and an example lab (`assets/example.svg`). A small mark closes the document (`assets/mark.svg`).
- New section "An example lab". The figure is redrawn from the records of one lab that ran on this template; it is not a screenshot. It shows the field, the number of researchers, the titles of the questions they chose (shortened and translated), and the first four lines of the guide's first briefing. It shows none of the results the researchers reported.
- The example question titles exist only inside the figure, not as text. When instructions listed example questions, researchers chose nearly the same ones (see the 2026-11-24 entry). The README tells an AI filling in the template to copy nothing from the figure into the files.

## 2026-11-25 Do not change the Git author information
- What happened: in one lab, one researcher's commits showed up under the GitHub account of a person who has nothing to do with the lab.
- Confirmed: that researcher's commits carried its role name as the author name and an email of the form `<role name>@users.noreply.github.com`. GitHub treats an address of that form as belonging to the account with that name, and such an account existed. Commits by other threads in the same repository kept the name and email set by the environment. In one other lab, the director, the guide thread, and one researcher had also changed the author name or email to a role name; no account was attached there when it was checked. This happened in two of the five labs whose repositories were checked.
- Presumed: the threads read "a commit message starts with the name of whoever did the work" broadly and matched their Git settings to their name. Which command they used was not confirmed.
- `instructions.md` section 7 (Korean edition, section 8): leave the Git author and committer name and email as the environment set them; your name goes only at the start of the commit message. The start of the message and the session line at the end already say who did the work.
- A commit shown under an unrelated account gives that account no access to the repository. Commits already pushed are left alone; history is not rewritten.
- `README.md`: one row added to "Common problems and what to do".
- Not yet run in a lab.

## 2026-11-24 English becomes the front page
- The English edition moved to the top of the repository and the Korean edition moved to `ko/`. Each README has buttons at the top that switch between the two.
- The two editions are not translations of each other. The Instructions box of a project accepts at most 16,000 characters, and the same content is longer in English. So the English edition is split into the text for the box (`instructions.md`) and a fixed rules file (`lab-RULES.md`) that is attached to the first message and saved by the coordinator as `lab/RULES.md`. The rules that prevent stalls or corrupted records stay in the box.
- In the English edition the coordinator also asks which language the researchers work in, which language threads use when they write to the user, and which time zone to use.
- The English edition has been run in one lab for a few hours. What was seen and what has not been seen yet is in "Still on trial or undecided" in `README.md`.
- This changelog starts here. Earlier entries below are summaries of the Korean record.

## 2026-11-24 The coordinator asks for the field
- Why: an AI that was given this repository and told only the name of a field invented a description of the field, five example questions, example branches, and two extra rules, and put them into the instructions. In labs whose instructions listed example questions, several researchers chose questions almost identical to the examples. And research that starts in one field can lead into another.
- `first-message.md`: before opening any thread, the coordinator asks which field or topic the lab should start from, and writes the answer word for word on the first line of `lab/README.md`. It adds no description, examples, or rules.
- `instructions.md`: the field is where the lab starts, not a boundary. The list of example fields was removed.
- `README.md`: the AI that fills in the template does not ask for the field and does not put anything into the files that the user did not say.
- Not yet run in a lab.

## 2026-11-24 Reasoning effort is a recommendation
- `README.md`: a reasoning effort of xhigh is recommended for threads, and the template was tested at that level. It is not a requirement, because the right level may change with each model generation.

## 2026-11-24 Banner and structure figure
- A banner and a figure of the thread structure were added. The lettering is drawn from outlines of open-licensed typefaces.
- The README states that the template is published by an individual and is not made or endorsed by Anthropic.

## 2026-11-24 The guide thread, and threads that are not researchers
- Why: after a few days, the notebooks, the board, and the daily digest were written in symbols and abbreviations that work among researchers, and a person could not follow the research. The researchers' way of writing was left alone, and a separate thread explains the lab in plain language when the user asks.
- A thread that is not a researcher writes its own line in a section at the end of `lab/RESEARCHERS.md`, so that two threads do not hold the same job and finished threads get closed.
- Researchers are not asked for deliverables such as papers or reports.

## 2026-11-23 First public version
- The instructions, the first message, and the README with the procedure for an AI to follow. The instructions were refined by fixing failures in labs run since 2026-11-20: the self-wake that never ends and the director's hourly sweep, direct messages and a board with one file per post, prior-work checks shared by the author and the pair reviewer, permission to push directly to main, and the list of things that need the user's approval.
- The license is MIT.
