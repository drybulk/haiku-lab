# Changelog

What changed in the published template, and why. The Korean edition keeps a more detailed record in `ko/CHANGELOG.md`.

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
