# Define: from data to a sharp problem

Goal: turn what you learned into a carefully crafted, meaningful and actionable **problem statement**, backed by analyzed data. Your first statement presupposed the problem; the revised one is based on what users actually said and did.

## Problem statements

A problem statement:
- describes the problem in detail
- describes the user group
- describes the user context
- includes background and **relevance** (why it is worth solving)
- **contains no solution**

An underperforming current tool may appear as context, but its underperformance is not the problem itself. A good statement promotes creative thinking and considers several stakeholders.

**Five questions**
- **Who** is affected? Name the stakeholders beyond the obvious users.
- **What** is the current state, the desired state, the unmet need?
- **When** does it occur? Pinpoint it narrowly: "on delivery days when no one is home", not "sometimes".
- **Where** does it occur? Place, department, region, culture.
- **Why** does it matter? Who loses what, how big the gap is between current and desired state, and how many people it affects.

**Contextualize**: what do we already know, and what don't we know? What exact issue will the research address, and what still needs to be learned? Illustrate why it matters.

**Relevance test.** If people dislike something but keep doing it with no cost, the problem may not be worth solving. People hate waiting at self-checkout but still wait; it becomes a real problem when they abandon the store and the store loses sales.

**Beware invented problems** — problems manufactured to sell a product. Ask whether real people actually suffer from it.

**Examples of the problem part (no solutions):**
- *Medication adherence.* Chronically ill people struggle to remember whether they took today's dose. Weekly pill boxes must be refilled every week, and sometimes a full week's supply isn't available.
- *Animal shelter.* Too few animals are adopted, especially older "non-cute" ones. Keeping them is expensive for a non-profit shelter.

**For a product brief, also say why this medium.** For example, why a smartphone app and not a website: on the move, notifications, camera or location, always at hand. Keep one or two backup problems in case the first proves infeasible.

**Never write** "Our app will do A, B and C" in a problem statement. That is a solution.

## Qualitative analysis

**Goal**: turn unstructured data into a detailed description of the important aspects of the situation or problem.

**Stages**: identify the components of the topic → study the properties and dimensions of each → understand and make inferences about the whole.

**Coding** means assigning categories and descriptors to blocks of text. It is more than paraphrasing or counting keywords. Its two key elements are identifying concepts and establishing the relations between them.

- **Emergent coding**: no prior theory; look for any interesting concept in the data. This is the right choice for interview data.
- **A priori coding**: categories come from an established theory or hypothesis. It suits content analysis and testing a framework.

**Grounded theory** (Glaser & Strauss) is inductive: open coding → concepts → categories → theory, with data collection and analysis interleaved.
- Strengths: a systematic approach, with findings backed by coded evidence.
- Weaknesses: the details can overwhelm you, the result is hard to evaluate, and it is prone to bias.
- Product teams usually stop at themes rather than forming a theory.

**Code book**: organize the codes hierarchically, with multiple levels. Look for key items, ask questions of the data, and compare at different levels.
- *Sensitizing questions* help you understand: What is the problem? What did the participant do to try to solve it?
- *Theoretical questions* help you connect: What is the relationship between these two factors? How does the interaction change over time?

**Rules**
- **Don't count mentions across semi-structured interviews.** Questions differ per person and the interviewer steers, so frequencies are meaningless and easy to manipulate. Counting belongs to surveys and content analysis.
- **Code from the participant's perspective, not yours.** If the teen talks about why apps ask for her age, the theme is "perceived purpose of age checks", not "security of apps".
- **Themes are concepts, not topics or descriptions.**

  | Weak theme | Better theme | Why |
  |---|---|---|
  | "Social media use" | "Purpose of use" | The weak one is a topic |
  | "Parental permission" | "Parental trust / approval" | The weak one is too descriptive |
  | "Effectiveness" | — | You can't measure it from interviews |

- **It is iterative**: expect to regroup several times.

## Affinity diagram

An affinity diagram brings issues and insights from all users into one hierarchical picture of the user population. It organizes large amounts of language data by natural relationships, and shows how the work hangs together and what matters, rather than breaking it into lists.

**Procedure**
1. **Collect data**: interviews, surveys, observations, field notes.
2. **Extract raw notes**
   - Re-listen to the recordings while transferring insights onto notes. Transcribing helps, because you hear it again.
   - Write each note from the user's perspective. One insight per note, concise.
   - Use a different color per participant.
   - Reread the problem statement often. Much of the data won't be relevant; keep what helps solve the problem.
3. **Synthesize**
   - Find two notes that seem related and place them together off to one side.
   - Add the notes related to that pair, then start new groups for other related pairs.
   - Typical families of groups: frustrations, interactions and touch points, goals and motivations.
4. **Create headers**
   - A header is an idea that captures the essential link among the notes in a group. Reuse an existing note as the header when one fits, and discuss the wording as a team.
   - Group the groups under **super-headers**. Keep headers concise and clear.
5. **Draw the finished diagram**
   - Problem statement at the top, super-headers and headers above their groups.
   - Show the relationships between groups.
   - Review and clarify, then document it.

**Deliverable set** (typical for a team project; use it as a default):
1. the initial set of words and concepts
2. the themed and sorted set
3. a relational diagram of the concepts
4. a cleaned, readable final diagram
5. a written summary of findings

Export everything at high resolution so it stays readable. A sample summary paragraph: "Every parent said toys end up all over the home, felt overwhelmed by gift-giving, and had received duplicate toys; all described rotating toys between storage and play, which is hard to keep organized."

**Classic errors**
- **Clustering by interview question.** If the headers are your interview questions, it is a bad affinity diagram. A super-header may echo a question, but the headers beneath it must be themes.
- **A "design suggestions" cluster.** Participants' solution ideas are data about a need, not designs. You are the designer: dig for the need behind the suggestion.
- **Taking complaints at face value.** In the classic elevator case, tenants complained that the elevators were too slow. The real issue was the boredom of waiting, and mirrors in the lobby solved it, not faster elevators. Understand what causes each complaint.
- **Headers that don't carry the insight.** Skimming the headers alone must tell you every finding.

**Tools**: sticky notes on a wall; Miro or FigJam for remote teams (share view-only links).

## Close the stage: goal setting

Revisit the initial problem statement. Based on the insights, restate, edit, sharpen or replace it. Then define the problem's context with design artifacts: a **persona** (a representative user) and a **storyboard** (a representative context). Both are covered in `ideate.md`.
