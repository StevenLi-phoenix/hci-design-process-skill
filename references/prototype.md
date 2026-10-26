# Prototype: build to think, test to learn

A prototype is "the iterative generation of artifacts intended to answer questions that get you closer to your final solution". Every prototype should state the question it answers: *Do users understand the setup steps? Can they find the share button? Does the reminder fit their routine?*

> Course coverage note: the course's sketching/prototyping, design-principles and mobile lectures follow its persona/storyboard lecture. Until those are folded in, this file follows *Interaction Design* ch. 3 and 12 and the standard HCI canon. The mental-models section comes from the course lecture.

## Fidelity ladder

Climb only as high as the open question needs.

| Level | What it is | Answers |
|---|---|---|
| Sketch | Rough drawings of screens and flows | "Which concept direction?" |
| Paper / lo-fi | Paper screens, sticky-note UI, card-based flows, simulated by a person | "Do people understand the flow and the vocabulary?" |
| Wireframe | Grayscale layout: content hierarchy, navigation, components, no visual design | "Is the structure right? Can they find things?" |
| Hi-fi | Interactive mock (e.g. Figma) with real content and visual design | "Does it feel right? Are there details that block tasks?" |
| Working code | Real implementation, possibly partial | "Does it work with real data and timing?" |

- **Horizontal** prototypes cover many features shallowly; **vertical** ones cover one feature in depth.
- **Wizard of Oz**: a human simulates the system's intelligence behind the interface.
- Lo-fi prototypes invite honest criticism because they look cheap to change. Hi-fi ones invite comments on color and polish.
- In a codebase, an ASCII or Markdown wireframe of each screen and its states is a valid lo-fi step before writing UI code.

**States to cover in wireframes:**
- empty, loading, partial, error, success
- first use versus returning user
- offline
- permission denied

## Conceptual model first

Before screens, decide the conceptual model:
- **Objects**: what users manipulate.
- **Actions**: what they can do to those objects.
- **Relations** between objects.
- **Terminology**: users' words, not internal jargon.
- **Metaphor**: desktop, shopping cart, save icon.

Interaction types to choose among:
- *instructing*: commands
- *conversing*: dialog
- *manipulating*: direct manipulation
- *exploring*: navigating a space

## Mental models (course lecture)

- A **mental model** is a person's internal small-scale model of how something works. They use it to predict and explain (Craik). Models can be *shallow* (a tap, a door handle) or *deep* (how a car or a computer works). They needn't be correct to be usable: plenty of people drive without understanding the engine.
- People bring models from earlier products. A visitor who only knows doors that pull may never try pushing. Drivers mirror their habits when the wheel moves to the other side of the car.
- **Designers are too familiar with their own system** to see it the way users do. That is why we do user-centered design.
- Match the users' existing model; use metaphors and conventions; break a model only with strong reason and market readiness. Paradigm shifts such as touch phones happen roughly once a decade, and invented interaction languages often fail.
- **Gulf of execution**: the gap between knowing what you want and knowing how to do it with this interface (finding the elevator's door-hold button). Minimize it with visible, well-labeled options.
- **Gulf of evaluation**: the gap between what the system shows and understanding what happened. Minimize it with clear feedback and state, and make sure people *do* evaluate. Users dismiss notifications and dialogs too quickly, so important state can't hide in a dismissible toast.
- **The interface is all users have.** You won't be beside them to explain it. A good UI discloses how it is to be used, with no manual needed.
- Ask users to describe how they think something works, in words or as a diagram or state machine ("what is it doing now, what happens next?"). This reveals models cheaply.

## Direct manipulation (Shneiderman)

- Continuous representation of the objects of interest.
- Physical actions (drag, pinch, click) instead of complex syntax.
- Rapid, incremental, reversible operations with immediately visible effects.

This narrows both gulfs and supports learning.

## Fitts' law

The time to hit a target grows with its distance and shrinks with its size.
- Make frequent targets bigger and closer.
- Exploit screen edges and corners, which act as infinitely deep targets.
- Put primary actions where the thumb or pointer already is.
- Don't use adaptive menus that reorder items by frequency: they break the user's learned expectation of where things are.
- Pie menus are faster to hit but rarely used: they hold few options and are hard to read.

## Design principles (Norman)

- **Visibility**: the relevant functions and state can be seen.
- **Feedback**: every action has a timely, perceivable result.
- **Constraints**: impossible actions are prevented, not just reported afterwards.
- **Mapping**: controls relate naturally to their effects (spatial layout matches the thing controlled).
- **Consistency**: same operations, same look and behavior, internally and with platform conventions.
- **Affordances and signifiers**: what can be done is perceivable, and clickable things look clickable.

## Psychological principles

- **Recognition over recall**: show options; don't make users remember them.
- **Hick's law**: decision time grows with the number of choices, so stage and group them.
- **Chunking**: working memory holds a few chunks, so group information.
- **Gestalt**: proximity, similarity, common region and alignment create the perceived structure.
- **Attention**: one primary action per screen; avoid competing highlights.

## Mobile design

- Touch targets of at least 44 pt (iOS) or 48 dp (Android); primary actions within thumb reach; design for one hand.
- Design for interruption: save state, keep flows short and resumable.
- Context of use: glanceable, outdoors in sunlight, on the move, poor connectivity.
- Pick the medium on purpose. An app earns its place through notifications, sensors (camera, location), offline use or frequency. Otherwise a website may serve better.

## Accessibility

- Text contrast of at least 4.5:1 (WCAG AA). Never use color as the only signal.
- Text must scale; layouts must work with screen readers (labels, order, roles) and with keyboard-only use.
- Captions and transcripts for media.
- Cover the 15–35% of users with some impairment in the persona set, or at least in the tests.

## Hand-offs while prototyping

- Data-heavy screens (tables, dashboards, feeds, detail pages): use the `interaction-design` skill to decide structure (overview → filter → details on demand).
- Visual styling: frontend-design skill.
- Keep the storyboard next to the wireframes. Each frame should map to a screen or state, and each screen should serve a frame.
