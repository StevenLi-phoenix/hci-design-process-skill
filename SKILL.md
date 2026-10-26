---
name: hci-design-process
description: Run a user-centered design process (Empathize → Define → Ideate → Prototype → Test) for anything a human will use — mobile/web apps, desktop software, onboarding and setup flows, forms, dashboards, CLIs' human-facing output, chat or voice flows, devices, services. Use when starting a new product or feature, when deciding who the users are or what problem to solve, or when asked to write a problem statement, plan user research, write or critique an interview guide or survey, analyze interview notes/transcripts (coding, themes, affinity diagram), create personas, user profiles, storyboards or scenarios, brainstorm, sketch or wireframe, plan a usability test, or run a heuristic evaluation or cognitive walkthrough. Trigger even when the user only says "design X", "how should I start building this app", "what should this app do", "redesign this flow", or "users are confused by Y". Not for cosmetic tweaks or pure coding tasks, and not for interfaces whose user is an AI agent (MCP tools, CLIs for agents, skills, prompts) — use aci-design-process for those.
---

# HCI Design Process

A user-centered design process for anything a person will use. Spine: design thinking — **Empathize → Define → Ideate → Prototype → Test**, iterated — with the concrete methods, quality gates and failure modes from a university HCI course built on *Interaction Design: Beyond Human-Computer Interaction* (Preece, Rogers & Sharp, 6th ed.).

The reflex this skill replaces: hearing "build an app that does X" and jumping to features and screens. "A wonderful interface to the wrong features will fail" (Nielsen). Most of the leverage is in the first two stages, which decide *whose* problem and *which* problem.

## First principles

- **You are not the user.** Designers — and Claude — know the system too well and carry their own assumptions. Every design claim traces back to evidence about real users, or is labeled as an assumption to test.
- **Usability only exists in context.** It is the extent to which *specified users* achieve *specified goals* with **effectiveness, efficiency and satisfaction** in a *specified context of use* (ISO 9241-11). Until you can say who, for what, and where, no design can be judged.
- **Look for needs, not solutions.** People can't reliably say what they'd want or what's possible (DVD-by-mail subscribers asked for faster shipping, not streaming). Study what they do, how, and why; the solution is the designer's job.
- **Iterate.** Any stage can send you back. An interview that contradicts the problem statement means rewriting the statement, not ignoring the interview.

## Scale the process to the decision

| Situation | Run |
|---|---|
| New product, new major flow, "what should we build?" | All five stages |
| New feature or screen in an existing product | Problem statement → evidence check → primary persona + storyboard → ≥2 alternatives → wireframe → heuristic review + usability test plan |
| Confusion or complaint report ("users can't tell if X worked") | Problem statement → evidence (tickets, recordings) → walkthrough of the current flow → redesign → usability test plan |
| Cosmetic tweak, copy fix, fully specified change | Skip the process; just do it |

## Where the evidence comes from

Claude usually cannot meet users. Rank evidence and label every artifact with what it rests on:

1. **Primary research** run by the human team — Claude prepares the guide or plan, the team runs it, Claude analyzes the transcripts and notes.
2. **Existing traces** — support tickets, issues, app reviews, forum posts, analytics, session recordings, earlier research.
3. **The requester's own account** — interview them by the same rules as any participant (specific past incidents, not wishes).
4. **Assumptions** — allowed only as labeled hypotheses, `[assumption — validate by …]`, each paired with how to check it.

Never present an assumption-based persona or finding as research-based.

## The stages

Each stage lists its goal, steps, artifact and exit gate. Methods, examples and pitfalls are in `references/`; fill-in skeletons are in `templates/`.

### 1. Empathize — understand users, tasks and context
Read `references/empathize.md`.
- Map users and stakeholders: primary (use it directly), secondary (affected, or influence it), and the indirect ones — people who manage users, receive outputs, pay, or use competitors.
- Profile them: age, abilities and impairments, education, tech experience, motivation, attitude, physical and social environment.
- Pick methods and triangulate: semi-structured interviews (default), observation and contextual inquiry (go to their environment and look at their artifacts), surveys only for breadth and in combination.
- Build the interview guide (`templates/interview-guide.md`): 3–4 themes derived from the problem statement; intro → warm-up → themed main body (specific past incidents first, speculative last) → wrap-up that always ends with "Is there anything we didn't talk about?" Before handing it over, lint every question and probe: rewrite any that opens with Do/Did/Is/Was/Have/Would… into What/How/Tell me about/Walk me through.
- Run interviews: informed consent, recording permission, anonymity; rapport; "why?", "tell me more"; follow the participant but cover every theme. Record and also take notes; verify AI transcripts against the audio.
- **Gate:** you can state, with evidence, the users' goals, the steps they take now, where it breaks, and how context and people differ.

### 2. Define — turn data into a sharp problem
Read `references/define.md`.
- Write the problem statement (`templates/problem-statement.md`): who, what (current state, desired state, unmet need), when, where, why it matters (magnitude, who loses what). No solution in it — not "our app will…".
- Analyze qualitatively: emergent coding from the participant's perspective; never count mentions across semi-structured interviews.
- Build the affinity diagram (`templates/affinity-diagram.md`): one insight per note, one color per participant, problem statement on top, clusters by underlying concept, then headers and super-headers, then relations.
- Revisit and rewrite the problem statement based on what the data actually says.
- **Gate:** the headers alone tell every insight; no cluster is an interview question; no "design suggestions" cluster; the problem statement still contains no solution.

### 3. Ideate — represent users, then generate options
Read `references/ideate.md`.
- Personas (`templates/persona.md`): one primary persona plus 2+ secondary, built from clusters — name, goals, motivations, frustrations, behaviors, and the technologies around the problem. Each persona is a **composite** of a pattern seen across several participants, never one persona per interviewee. Validate each against the data: "could this be one of the people we talked to?"
- Storyboard or scenario (`templates/storyboard.md`): the primary persona in a concrete scene, a trigger, the problem, the decisions, the solution, an ending, and emotions frame by frame. It tells the user's story, not the screens' story.
- Brainstorm broadly first (quantity, no judging), then converge on fit to the persona and problem, then on feasibility. Produce at least 2–3 genuinely different concepts.
- **Gate:** every concept traces to a persona's goal or frustration, and features that serve no persona are cut.

### 4. Prototype — build to think, test to learn
Read `references/prototype.md`.
- Climb the fidelity ladder only as far as the open questions require: sketches → paper or lo-fi → wireframe (structure, hierarchy, navigation) → hi-fi interactive → code.
- Design the conceptual model before the screens: objects, actions, terminology, and the metaphor that matches the users' existing mental model.
- Close both gulfs: **execution** (can they tell what to do and how?) and **evaluation** (can they tell what happened and whether it worked?). The interface is all users have — you won't be there to explain it.
- Apply the design principles: visibility, feedback, constraints, mapping, consistency, signifiers; Fitts' law; recognition over recall; accessibility.
- For data-heavy screens, hand structure to the `interaction-design` skill and visual styling to a frontend-design skill.
- **Gate:** each prototype states the question it exists to answer.

### 5. Test — will it work for them?
Read `references/test.md`.
- Inspection first, because it is cheap and Claude can do it: heuristic evaluation (Nielsen's 10, with severity ratings) and a cognitive walkthrough of each storyboard task. Label these results as inspection, not user evidence.
- Usability test with real users (`templates/usability-test-plan.md`): about 5 representative participants per round; realistic tasks taken from the storyboards with success criteria; think-aloud; measure effectiveness (completion, errors), efficiency (time, steps) and satisfaction (SUS); debrief.
- Analyze into issues × severity × evidence, fix, and test again.
- **Gate:** the core tasks succeed with representative users, or the remaining issues are known, ranked and scheduled.

### Ethics in every stage
Read `references/ethics.md`. Covers research ethics (consent, anonymity, withdrawal, power, vulnerable groups) and design ethics (privacy defaults, accessibility, dark patterns, bias — test with diverse users).

## Artifacts

Write artifacts into the project, by default under `docs/design/<topic>/`, one file per artifact, from `templates/`. Each artifact carries its evidence level (primary, traces, requester, assumption) and date. When the user wants the answer in chat, give the same structure in chat.

## Hand-offs

- Structuring how data and records appear on screen → `interaction-design` skill.
- Visual styling → frontend-design skill.
- If AI agents also use this product's interface (MCP server, CLI, API, chat tools), run `aci-design-process` for the agent side, and reuse this process's tasks and storyboards as its eval tasks.
