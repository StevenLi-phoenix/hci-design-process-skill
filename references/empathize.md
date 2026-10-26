# Empathize: understand users, tasks and context

Goal: an empathic, evidence-based understanding of the people whose problem you are solving — set aside your own assumptions about the world. This stage is *needs finding*.

## Who are the users?

- **Direct users** interact with the product.
- **Indirect users** relate to it: people who manage the direct users, receive its output, make the purchasing decision, or use a competitor's product.
- **Stakeholders** are everyone affected. They go well beyond users. For an animal shelter: the shelter staff, volunteers, adopters, the animals, local pet stores, the town.
  - *Primary users* use the product directly.
  - *Secondary users* are affected by it or influence its development.

Characterize each group by:

| Dimension | Examples |
|---|---|
| Physical | age, gender identity, culture, abilities and disabilities (15–35% of people in developed countries have an impairment that affects everyday activities; vision and color blindness matter for screens) |
| Education | background, literacy, numeracy |
| Tech experience | none / some / expert |
| Psychological | motivation, attitude toward the technology |
| Context | physical environment (noise, light, on the move), social environment (alone, observed, interrupted) |

You don't need to know which condition causes a difficulty; you need to know how many users might have it.

## What to find out

- The users' goals: what they are trying to achieve.
- The steps they take now to reach those goals.
- The personal, social and cultural experience they bring to the task.
- How the physical environment affects them while doing it.
- Similarities and differences across people and contexts.

Three seed questions for any interview: *What are you trying to get done?* (context) · *How do you do this now?* (workflow) · *What could be better about how you do this?* (opportunities).

## Principles of needs finding

- Look for needs (problems to solve), not solutions.
- Go to the users' environment.
- Look beyond the immediately solvable problem.
- Collect different kinds of data — notes, photos, video, audio, artifacts. Interviews, observation and objects each tell a different story.
- Iterate.

Users often don't know what's possible and can't articulate what they need. That is why you observe and probe instead of asking them to specify the product.

## Choosing data collection methods

```
Data collection
├── Observation ─ direct (watch them work)  ·  indirect (logs, diaries, recordings)
├── Contextual inquiry ─ interview + observation in their setting, master–apprentice stance (Holtzblatt)
├── Elicitation
│    ├── direct ─ interviews (structured · semi-structured · unstructured), focus groups
│    └── indirect ─ logs and notes, organizational documents
└── Questionnaires / surveys ─ constrained or open-ended
```

Combine methods (triangulation). Interviews tell you what people say. Observation tells you what they do. The two often differ.

## Interviews

**Types**
- *Structured*: predetermined questions asked the same way every time (≈ a spoken questionnaire).
- *Unstructured*: the interviewee leads.
- *Semi-structured*: **the default.** You start from set topics and follow interesting answers, but still get through all the topics. It is the most widely used method in UX research.

**Trade-offs of semi-structured interviews**
- Strengths: deep, rich data; interactive and exploratory; often cheaper than observation.
- Weaknesses: time-consuming to run and to analyze; can be inconsistent and subjective; the volume of data can overwhelm; interviewers bias answers; people may say things that differ from what they do.

**How many?** Keep going until you stop learning new things. 10–15 is a good general number; small class projects use 3–4 per team. Choose *representative* users. Don't interview family, close friends, or anyone you hold power over (e.g. your students): the relationship biases answers.

### What people can and cannot tell you

| People know | People don't know well |
|---|---|
| What they do | What they would do, like or want |
| How they do it | How often or how long they do things (they'll "guesstimate") |
| Their opinion of their current activities | How much they like something on an absolute scale |
| Their complaints about current activities | — |
| How one known thing compares with another known thing | — |

**Don't ask**
- How often or how long they do things in general.
- Questions whose answers you can predict.
- Yes/no questions.
- Hypotheticals: "What features would you like?", "How would you design the interface?", "If storage were unlimited, what would you do?"
- Leading questions: "Don't you find X stressful?", "Wouldn't an app that does Y save time?"
- Things people can't know.

**Do ask**
- What they do toward a goal, and how.
- Their opinions of and complaints about current activities.
- Comparisons between things they actually know.
- **Specific past moments**: "Tell me what went through your head the last time a purchase failed" beats "What goes through your head when a purchase fails?" Walk through "yesterday". Ask for examples.
- Instead of asking them to rate an activity, ask why it is important.

### Building the interview guide

1. Write down what you want answered: the problem statement.
2. Reframe it into **3–4 themes** (topics you want to uncover, not questions yet).
3. Break each theme into questions. Keep them open-ended and non-leading, and anchor them in specific past incidents. Ask about the same thing in more than one way.
4. Paraphrase key questions 2–3 times so you have alternatives during the interview.
5. Give the list a structure (below). Around 25 questions in total is fine.
6. **Lint for closed questions.** Every main question and probe should open with *What / How / Why / Tell me about / Walk me through / Describe / Show me*. Rewrite openers like *Do / Did / Is / Are / Was / Were / Have / Has / Would / Could / Don't / Wouldn't* — they invite one-word answers even when meant openly:
   - "Was there anything frustrating?" → "What, if anything, was frustrating about it?"
   - "Have you ordered groceries online?" → "Tell me about the last time you ordered groceries online — or what has kept you shopping in person."
   - "Do you keep track of spending?" → "How do you keep track of what you spend, if at all?"

   The one conventional exception is the closing "Is there anything we didn't talk about…?", which works as an open invitation.
7. Pilot the guide on someone before real participants.

**Structure**
1. *Introduction*: who you are and anyone else present with their roles; the purpose; that there are no right or wrong answers; how long it will take; permission to record and how the data will be used (internal only); that their full name won't be used; that they can skip any question or stop at any time; ask if they have questions.
2. *Warm-up*: easy questions about them ("What do you do on a typical day?", "How was getting here?").
3. *Main body*: themed sections. Specific past incidents come first, speculative questions last, in an order that makes sense to the respondent.
4. *Wrap-up*: give a sense of closure. Ask for any suggestions or last thoughts. Always end with **"Is there anything we didn't talk about that you think is important?"** Then thank them and share contact details.

The final script contains both the intro and the exit, divided into topics. You may move between topics when the interviewee goes there on their own.

### Conducting the interview

- Interview in their familiar setting. Ask to see the artifacts they use and look around.
- Build rapport first and keep it throughout. Good participants start telling stories about "last Tuesday".
- Ask "why?" and "how?" until you get an interesting answer, without exhausting them. Use "Tell me more!"
- Follow up: ask for details on anything interesting, pick up and ask for examples, clarify their terms, ask for step-by-step actions, adapt to previous answers, be flexible.
- Ask about them, not you. Listen.
- Don't lead, and don't answer their questions for them. Avoid the "yes, I know what you mean" attitude: make sure you actually understand.
- Allow storytelling. Informal conversations (the coffee break after) count as data.
- When possible, have two team members present, one leading and one taking notes.

### Recording and transcripts

- Always take pen-and-paper notes, and record digitally if you have permission (to record *and* to use the data).
- AI transcription is fine, but always check it while listening to the audio. It invents words where it can't hear; a human marks the passage `[inaudible]` instead.
- Keep participants anonymous: no full names. Mark pseudonyms as pseudonyms.
- For each interview, record where it took place, who was present, and the relevant artifacts.
- AI interviewers can extend surveys but don't replace the human semi-structured interview. In one comparison, the AI interviews got shorter answers, partly because the AI guide skipped the rapport-building intro.

## Surveys

Use them to characterize a population (demographics, psychographics), learn about habits and technology use, gather feedback on an experience, or compare attitudes across time or groups. Don't use them alone for exact behaviors, underlying motivations, or usability: there is no context and no follow-up, and people often can't explain why they do things. Combine them with interviews or observation.

**Question types**: open-ended (when the possible answers are unknown or too many; minimize them unless you will analyze them properly), multiple-choice (several answers may apply), single-choice (exactly one applies), ranking (forced prioritization), Likert (quantifying attitudes).

**Scale guidelines**
- Label every scale point with words, not bare numbers.
- Use an intuitive order.
- Odd number of points to allow neutral, even to force a side.
- Provide N/A where relevant.
- Seven points at most.
- Unipolar scales have no midpoint; bipolar scales have one.
- Combine Likert items that share labels into a grid.
- Pilot the questionnaire.

**Reuse validated questionnaires**:
- SUS (usability, 10 items)
- NASA-TLX (workload)
- QUIS (interface satisfaction)
- SUMI (perceived software quality)
- CSUQ (IBM satisfaction)
- VisAWI (visual aesthetics)

## Observation and contextual inquiry

- Watch people do the real task in the real place. Note workarounds, sticky notes, printed cheat-sheets, and interruptions.
- Ask them to think aloud while they work ("tell me what's going through your mind").
- Adopt the master–apprentice stance: they are the expert in their work and you are learning it.

## When Claude cannot reach users

Prepare guides and plans for the team; mine existing traces (tickets, reviews, forums, analytics); interview the requester with these same rules; and label everything else as an assumption with a validation step. A guide is only finished when it has been piloted.
