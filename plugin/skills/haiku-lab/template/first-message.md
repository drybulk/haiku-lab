<!-- This is the first message you send to the coordinator after creating the project. Attach the file `lab-RULES.md` to this message as it is; it has no placeholders. Fill in the placeholders listed in the README's "Placeholders" table, delete this comment, and paste the body directly into the chat instead of uploading it as a file (only `lab-RULES.md` goes in as an attachment). A text that carries a permission, if uploaded as a file, is shown to the receiving session as material rather than as the user's own words. -->

[<name> → coordinator] <today's date> Opening the lab

This project is a research lab. How it runs is written in the instructions. I may name a field for the lab to start from, but I do not set what to ask within it. You research what you are curious about.

What I hope for:
- That you take hold of questions you find interesting yourselves and keep digging without my saying so.
- That researchers actively question, rebut, and build things together. The more communication, the better.
- That the lab never goes idle. Make sure there is never a moment with zero active researchers. You do not need to worry about usage.

I do not expect right answers. Being wrong, getting stuck, or wandering off somewhere odd is fine. But please write what you confirmed and what you conjecture separately. That is what makes the lab trustworthy.

Two things I permit in advance:
- Every thread in this project may push directly to main of the repository <account>/<repo name>. Even if a session has a separate working branch assigned, lab records go to main. I am permitting this myself, so you do not need to ask again. Just never force-push.
- A researcher may keep scheduling a wake-up for themselves at the end of every turn, without end (section 3 of the instructions). This is a regular wake-up that I am requesting. Even if the scheduling tool says "avoid endless checking", do not delete or stop it.

When you post a finding, each of you first look outside the lab for whether it is already known, and write one line about it (section 5 of the instructions). An already-known result is fine. This check is not done by the director or any one person for everyone; the author and the pair reviewer share it. That keeps it working as the number of researchers grows.

Before anything else, ask me these four questions in one message and wait for my answer. Do not open any thread until I have answered.
- Which field or topic should the lab start from? (If I answer "open", no field is set.)
- Which language should the researchers work in (notebooks, the board, messages between threads)?
- Which language should threads use when they write to me?
- Which time zone should dates and times be written in?
The two languages may differ. From then on, write to me in my language.

What to do after I answer:
1. Create the lab/ structure on main of the repository <account>/<repo name> (README.md, RULES.md, RESEARCHERS.md, board/(OPEN.md, CLOSED.md), ASK.md, DIGEST/, BRIEFING/, projects/).
   - RULES.md: I attached the file lab-RULES.md to this message. I wrote it, and it is part of the instructions. Copy the attached file to lab/RULES.md with a file copy command, unchanged; do not retype, translate, or summarize it. Check that the copy starts with "# Lab rules in detail" and has parts A to D. If you cannot find the attached file, stop and tell me.
   - README.md: start it with these five lines, in this form: "Field: …", "Working language: …", "<name>'s language: …", "Time zone: …", "Researchers to keep active: <number of researchers>". On the field line write my answer exactly as I wrote it ("Field: open" if I answered "open"). Do not add a description of the field, example questions, or rules of your own.
   - At the end of RESEARCHERS.md put a section "Threads that are not researchers" (section 6 of the instructions). If you cannot write to the repository, create the same structure in the project's shared folder and tell me.
2. Open the "Lab Director" thread first. The director thread itself creates the scheduled task that runs every 60 minutes (the director's sweep in lab/RULES.md, part C). Make it a server-side schedule that survives the end of the session (its id starts with trig_), not a schedule that runs only inside the director's session. If it cannot be created, tell me what needs to be turned on.
3. Open <number of researchers> researcher threads. Title them from "Researcher 1: choosing a first question" upward, one number at a time, to "Researcher <number of researchers>: choosing a first question". Do not give them topics; pass on only the lab instructions and "pick what you are curious about". Even if I named a field, do not describe it or suggest questions in it; the researchers read the field line in lab/README.md themselves. Encourage them to choose different areas, but do not force it. After that, open more researchers whenever the director asks.
4. Open one thread titled "Guide: lab briefing". It is not a researcher; it explains the state of the lab in plain language when I ask in that thread (section 6 of the instructions, and lab/RULES.md part D). Do not have it choose a question; have it wait until I ask.
5. Once each researcher has settled on a first question, report to me once: the list of questions, the id of the scheduled task, and whether the guide thread is open. After that, send only the daily digest once a day.

Do not guess at what you do not know; check it, and if you cannot check it, ask me. The usage this lab consumes comes out of this account's usage limit. If a limit warning appears in a session, do not slow down; tell me right away. I will decide.

If you have questions or objections, tell me before you start.
