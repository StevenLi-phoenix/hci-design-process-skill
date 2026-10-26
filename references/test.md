# Test: will it work for them?

Testing is "an opportunity to learn about your solution and your user". You collect feedback on your prototypes from users, and get another chance to empathize. Test every fidelity level, not just the final build.

> Course coverage note: the course's evaluation, usability-testing and inspection lectures come late in the semester. Until those are folded in, this file follows *Interaction Design* ch. 15–16 (evaluation studies; inspections, analytics and models) and standard practice.

## What to measure

- **Effectiveness**: can users complete the tasks, and how completely and accurately? Measure completion rate, errors, and the severity of those errors.
- **Efficiency**: what does it cost them? Measure time on task, number of steps, and help requests.
- **Satisfaction**: how do they experience it? Use SUS or other questionnaires, ratings, and quotes.

Also consider learnability (time to first success), memorability (performance after a break), and the experience goals that matter for your product (fun, trust, calm).

## Choosing an evaluation method

| Method | Setting | Users involved | Good for |
|---|---|---|---|
| Usability test | controlled (lab, remote session) | yes | finding where specific tasks break |
| Field study / in-the-wild | natural setting | yes | real context, long-term use, social factors |
| Heuristic evaluation | desk | no (3–5 evaluators) | cheap, early, broad issue sweep |
| Cognitive walkthrough | desk | no | learnability of specific task paths |
| Analytics / A/B tests | live product | yes (at scale) | what happens, at scale, without the why |
| Predictive models (Fitts, KLM) | desk | no | comparing expert-time of alternatives |

Inspection methods are cheap and early but **don't replace users**. Label their output as inspection findings.

## Usability test

**Plan** (template: `../templates/usability-test-plan.md`):
1. **Goals and questions.** Which design questions must the test answer?
2. **Participants.** Use representative users matching the personas, not teammates. About **5 per round** finds most major issues. Run more rounds rather than larger ones.
3. **Tasks.** Make them realistic, drawn from the storyboards, each with a clear success criterion. Phrase them as goals, not instructions, and never with UI words: "You want your Documents folder backed up — do it, and tell us when you're confident it's done", not "Click Start backup".
4. **Setup.** The prototype at the right fidelity, devices, screen or audio recording, a note-taking sheet, and the roles: facilitator, note-taker, observers.
5. **Script.**
   - Welcome, purpose, and "we're testing the design, not you".
   - Consent and recording permission; tell them they can stop at any time.
   - Explain think-aloud and give a practice task.
   - Run the tasks. Don't help: answer questions with questions ("What do you think it does?"). Prompt silence with "What are you thinking?"
   - After each task: ask about ease, ideally with one SEQ-style rating.
   - At the end: SUS plus open questions ("What was most confusing?", "Anything we didn't ask about?").
   - Thank them.
6. **Pilot** the whole session once.
7. **Analyze.** List each issue with the evidence (who, which task, quotes or observations), its frequency across participants, and its severity on Nielsen's 0–4 scale: 0 not a problem, 1 cosmetic, 2 minor, 3 major, 4 catastrophe. Turn the issues into prioritized fixes, then re-test.

**Think-aloud**: participants verbalize what they are looking for, expecting and feeling while they work. It reveals the mental model behind each error.

## SUS (System Usability Scale)

There are ten statements rated on a 5-point scale from strongly disagree to strongly agree. They alternate between positive and negative wording.

**Scoring**
- Odd items score (response − 1).
- Even items score (5 − response).
- Add them up and multiply by 2.5, which gives 0–100.

Around 68 is average. Report the mean and spread, and never treat SUS as a percentage.

## Heuristic evaluation

3–5 evaluators each inspect the interface alone, then merge their findings. Each finding names the heuristic violated, where, why, and its severity (0–4).

Nielsen's 10 heuristics:
1. **Visibility of system status**: timely feedback about what is going on.
2. **Match between system and the real world**: users' language and concepts, in a natural order.
3. **User control and freedom**: clearly marked exits, undo and redo.
4. **Consistency and standards**: follow platform and industry conventions.
5. **Error prevention**: eliminate error-prone conditions; confirm risky actions.
6. **Recognition rather than recall**: make options and information visible.
7. **Flexibility and efficiency of use**: accelerators for experts; allow customization.
8. **Aesthetic and minimalist design**: no irrelevant information competing for attention.
9. **Help users recognize, diagnose and recover from errors**: plain-language messages that suggest a fix.
10. **Help and documentation**: easy to search, task-focused, concise.

Claude can run a heuristic evaluation on wireframes, screenshots or code. State it as an inspection and pair it with a usability test plan.

## Cognitive walkthrough

For each step of a task's correct path, ask:
1. Will the user try to achieve the right effect? Do they know this is what they need to do now?
2. Will the user notice that the correct action is available?
3. Will the user associate the correct action with the effect they want?
4. If the correct action is performed, will the user see that progress is being made?

Any "no" is a learnability problem at that step. Walk through each storyboard's tasks with the primary persona in mind.

## Design critique

A structured critique of your own project, or a peer's, against the problem statement, the personas, and these heuristics:
- What works, and for whom.
- What fails, with evidence.
- What to change next, ranked.

Critique the design, not the designers.

## Iterate

Fix the highest-severity issues, then re-test with new participants. Stop when the core tasks succeed with representative users, or when the remaining issues are known, ranked and scheduled. Return to Define if tests show the problem itself was wrong.
