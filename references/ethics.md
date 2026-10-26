# Ethics in every stage

## Research ethics (Empathize, Test)

- **Informed consent.** Tell participants what the study is about, what you will do with the data, whether you are recording, and how long it takes. Get explicit permission to record and to use the data.
- **Voluntary participation.** People may skip questions, stop at any time, and withdraw afterwards without consequences.
- **Anonymity and confidentiality.** Don't record full names in transcripts or deliverables. Mark pseudonyms as pseudonyms, and strip identifying details: employer, exact address, unusual job titles. Store recordings securely and only as long as needed.
- **No power relationships.** Don't recruit your own students, your employees, or anyone whose answers could be coerced. Avoid family and close friends too; that is a bias problem as much as an ethics one.
- **Special populations need extra protection**: children (parental consent plus the child's assent), elderly people, cognitively impaired people, prisoners.
- **Deception** is acceptable only when the research justifies it, and must always be followed by a debrief that explains what really happened and why.
- **Formal review.** Publishable research needs an ethics review board (IRB). Internal product research still follows the principles above.
- **Online data.** Scraping public posts may violate a site's terms and users' expectations. "Public" doesn't mean consented. Classic cautionary cases are Tuskegee, Milgram, and the Facebook emotional-contagion study.
- **Research integrity.** Never fabricate or "tidy" data, never misrepresent findings, and disclose conflicts of interest.

## Design ethics (Define → Test)

### Privacy by default

Make the defaults match what users believe. For example, if interviews show users think nobody can see their "last active" time, while the app shows it to every contact by default, the design is the problem. Fix it with:
- a privacy-preserving default
- visible state: who can see this right now
- control placed next to the thing it controls
- explanation at the moment it matters, not buried in settings

### Accessibility

Treat accessibility as a design requirement, not polish: contrast, scalable text, screen-reader semantics, keyboard use, captions, and never color as the only signal. Include people with impairments in research and tests.

### Dark patterns

Don't design flows that work against users' interests:
- **Confirmshaming**: "No thanks, I don't like saving money."
- **Roach motel**: easy to subscribe, hard to cancel.
- **Forced continuity**: a free trial that silently converts to paid.
- **Sneak into basket**, hidden costs, disguised ads.
- **Privacy zuckering**: confusing settings that make people share more than they intended.
- **Nagging**, and preselected consent boxes.

Dark patterns also carry legal risk in many jurisdictions. If a business goal pushes toward one, make the trade-off explicit to the team.

### Bias and inclusion

Algorithms and AI components can encode bias: skewed training data, feedback loops (a risk score that drives decisions which then generate the next training data), and over-corrections. Counter it by testing with diverse users (age, culture, ability, gender, language) and by measuring outcomes per group.

### Persuasion and wellbeing

Engagement mechanics such as streaks, infinite feeds and variable rewards should serve the user's stated goal, not just time-on-app.

### Honest prototypes

When showing concepts to users or funders, say which parts are real, simulated (Wizard of Oz), or aspirational.
