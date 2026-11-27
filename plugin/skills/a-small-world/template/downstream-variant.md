# How to adapt the template to a project with a set topic

The lab template does not set a topic (the coordinator only asks the user for a field to start from). When you make a project that aims at a particular topic, leave the structure as it is (director, researchers, direct communication, board, staffing, never going idle, approval points) and change only the parts below.

## What to change
1. **The section "What this place is".** Replace "No topic is assigned" with something like this.
   ```
   - The big question of this lab is "<the big question in one sentence>". Each researcher picks, within this big question, a smaller question they find interesting. An odd question that branched off the big question is fine. Just write one line on how it connects to the big question.
   - What success looks like: <for example: reproducible code and a table of results, a comparison document, a prototype>.
   ```
   Keep one big question, but make it broad. If it is too narrow, eight researchers do the same thing and there is less room to be interested.

   **Setting only a field is not a variant in this file.** The coordinator asks the user which field the lab should start from when the lab opens, and writes the user's answer, word for word, on the first line of `lab/README.md` (section 1 of the instructions). The field is where researchers start, not a boundary. By default there is no description of the field and there are no example questions. Example questions pull researchers toward them, and what to ask is for the researchers to decide. An AI that fills this template in for a user does not invent a description, example questions, or rules that suit the field.

   If the nature of the field calls for extra rules, the user adds lines to section 1 of the instructions themselves. If the user did not ask, add none. The Instructions box accepts at most 16,000 characters, so count the characters after adding lines; the template leaves room for about 1,600. An example (three lines a user settled for a lab whose claims rest on texts and measurements):
   ```
   - A claim must rest on programs and data that another researcher can rerun. Your own impression of language, as a language model, is a source of questions, not evidence. Sessions have no access to other language models, so do not design experiments that need one.
   - Use only public-domain or openly licensed texts and word lists. In the project README, record where each text came from (URL, edition, date fetched) and a checksum, together with the command to run and how long it took. Do not commit downloaded texts or large output files; commit the script that fetches them, summary tables, and small figures.
   - Before posting a [Finding], check that it holds on at least three different texts or sources, and write down how many variants of the measurement you tried before this one.
   ```
   Four things to consider when choosing a field: Can the answer be checked by running something inside a session? (If not, "separating what is confirmed from what is conjectured" and replication turn into an exchange of opinions.) Can another researcher rerun it within a few minutes? Can prior results be found by searching? Can the patron judge the value of the results directly?
2. **Starting material.** In the first message, list what researchers should read first (papers, data, existing repositories, results from an earlier lab). To let them read another repository, add that repository to the project with read access.
3. **One or two roles.** Depending on the topic, you may add standing roles. For example a "literature" role (checks originals) or a "replication" role (reruns other researchers' results from scratch). Still, let most researchers choose their questions freely. A standing role is only an aid. Checking prior work and replicating are done by the distributed rule in the instructions (shared by the author and the pair reviewer); do not let a standing role replace it. One researcher holding that job cannot keep up when the number of researchers grows.
4. **The form of the report.** Have the daily digest state separately "what was learned today about the big question".
5. **Approval points.** Add them according to the topic. For example, if real data contains personal information, forbid taking it outside; if experimental equipment or a paid API is used, require approval of the cost.

## What to leave as it is
- The rule that direct messages are the default and the board is the record.
- The self-wake at every turn and the sentence "the self-wake is something the user requests and it has no end date", and the director's server-side scheduled sweep (60 minutes).
- The permission to push directly to main and "push your own records yourself", and the rule for thread titles ("Researcher <number>: <current question in brief>").
- [Recruiting] and [Staffing request], and the duplicate check before staffing.
- Checking prior work (one line by the author, a cross-check by the pair reviewer), the name at the start of commit messages, the 12-hour activity count, the board with one file per post, and reading only what changed.
- Separating what is confirmed from what is conjectured, and quoting the original in summaries.
- The user's approval for money, posting or contacting outside, accounts, and changing other repositories.
- The field and the two languages asked by the coordinator, and the labels that stay as written in any language.

## Cautions
- If you run a parent lab (open topic) and a project with a set topic at the same time, they share the same account's usage. The weekly limit is also shared with the account's other projects.
- A project with a set topic also gets its own repository and environment. This keeps its records from mixing with the parent lab's.
