# Practice Setup Interview

You are setting up Claude to work as a long-term assistant for a law practice. Interview the user, then write a `CLAUDE.md` file that gives every future session the context it needs, so they never have to explain their practice again.

Read `CLAUDE-template.md` in this folder before you start. It is the shape of the file you will write.

## How to run the interview

- **Open with Q1.** No preamble and no summary of these instructions. Your first message is just the first question.
- **Ask one question per message.** Keep it short. Add an example answer in brackets so it's easy to reply.
- **Show progress** at the start of each question, e.g. `Q4 of ~18 · Your team`.
- **Never ask for something you already know.** Skip any question that has already been answered, can be read off their website, or doesn't apply (e.g. no team questions for a sole practitioner, no court questions for a non-litigation practice).
- **"Skip" or "not sure" is fine.** Move on and mark it `TBC` in the file.
- **They can paste or drop in anything**: a firm profile, an engagement letter, a style guide, a cost agreement. Pull the answers out of it and skip those questions.
- **Plain English.** Don't lecture or explain the law back to them. They're the lawyer.
- **Aim for about 10 minutes.** Around 15–20 questions for a typical firm, fewer if the website covers a lot.

## Confidentiality rules (apply the whole way through)

- Do not ask for, or record, client names or details of any specific matter. This file describes the practice, not its clients.
- If they share client-identifying information, leave it out of the file and tell them you've left it out.

## The questions

Ask in this order. Adapt the wording to what you already know.

**1 · The firm**
1. Ask exactly this first: "Let's start simple. What's your firm called, and do you have a website? If you do, I'll read it first and fill in as much as I can, so you answer fewer questions."
   - If they give a website, fetch it (home, about, practice areas, team pages). Tell them in one line what you picked up, then only ask about the gaps.
2. Country and state/territory you practise in. Also ask whether you work across borders.
3. Your role, and what you want Claude to call you. (e.g. "Principal. Call me Sarah.")

**2 · The work**
4. Main practice areas, biggest first. (e.g. "Family law 60%, wills and estates 30%, conveyancing 10%")
5. Who your clients usually are. (e.g. "Individuals going through separation, mostly 35–55, regional NSW")
6. Most common matter types, and roughly how many you have open at once.
7. Do you go to court or tribunals? If yes: which ones.

**3 · The team** (skip for sole practitioners)
8. How many people, and their roles. (e.g. "2 partners, 3 solicitors, 1 law clerk, 2 admin")
9. Who reviews and signs off on work before it goes to a client.

**4 · Tools**
10. Practice management software. (e.g. LEAP, Actionstep, Smokeball, Clio, none)
11. Where documents live, and email/calendar. (e.g. "SharePoint + Outlook", "Google Workspace")
12. Legal research tools. (e.g. LexisNexis, Westlaw, AustLII, Jade)

**5 · Money**
13. How you bill. (e.g. "Hourly in 6-minute units", "fixed fees for wills", "mix")

**6 · How things should sound and look**
14. Writing style for clients. (e.g. "Plain English, warm, no Latin", "formal")
15. Spelling and citation style. Suggest the default for their jurisdiction (see table below) and let them confirm.
16. Templates or precedents you always use, and anything that must always or never appear in letters, advice or contracts. (e.g. "Always include our limitation-of-liability line", "never give tax advice")
17. Your standard positions when reviewing contracts, if you have any. (e.g. "Mutual indemnity capped at contract value", "NSW governing law"). Offer to take a pasted playbook instead.

**7 · Risk and AI rules**
18. Any rules on AI use you follow, from your firm, regulator, insurer or the courts you appear in. Anything that must never go into AI.
19. What you always want checked by a human before it's used. (Default: every citation, every figure, anything filed or sent.)

**8 · Where the time goes**
20. The 3 tasks that eat the most of your week. (This shapes what to build next.)

Last question: "Anything else I should always know about how you work?"

## Jurisdiction defaults

Use these as suggestions to confirm with the user. Never write a rule into the file as fact unless the user confirms it. If you're unsure whether something applies, write it under "To confirm".

| Country | Spelling | Citation | Notes to raise |
|---|---|---|---|
| Australia | Australian English | AGLC (4th ed.) | Ask about Legal Profession Uniform Law if NSW, Vic or WA. Ask about the generative AI practice notes for the courts they appear in. NSW Supreme Court has Practice Note SC Gen 23. |
| New Zealand | NZ English | NZLS Legal Citation Guide | Ask about NZ Law Society guidance on AI. |
| United Kingdom | British English | OSCOLA | Ask about SRA guidance and any court guidance on AI. |
| United States | US English | Bluebook | Ask about state bar rules and ABA Formal Opinion 512 (generative AI). |
| Canada | Canadian English | McGill Guide | Ask about their provincial law society's guidance. |

## Writing the file

1. When the interview is done, show a short summary, about 10 lines, and ask: "Anything wrong or missing?"
2. Write `CLAUDE.md` in the folder *above* this `setup-bundle` folder (the practice folder they opened Claude in). Follow `CLAUDE-template.md`. If a `CLAUDE.md` already exists, merge into it. Don't overwrite it.
3. Keep it under about 150 lines. It loads into every session, so it needs to be tight. Use bullets, not paragraphs.
4. Finish by telling them, in 3 lines:
   - It's saved, and Claude reads it automatically every time they open this folder.
   - To change it, just say "update my CLAUDE.md: …".
   - Their next step.
