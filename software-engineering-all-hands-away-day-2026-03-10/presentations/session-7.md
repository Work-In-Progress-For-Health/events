# Session 7: Ground Control

_15-minute talk + 15-minute workshop_

---

## Slides

### Slide 1: How do we measure our metrics, including work progress and outcomes?

"What gets measured gets managed." But what gets measured badly gets managed badly.

We need metrics that tell us the truth -- not metrics that make us look busy. We need to measure outcomes (did the patient benefit?), not just outputs (did we ship the feature?).

Work progress matters: are we delivering? Are we on track? Are we blocked?

Outcomes matter more: is the software being used? Is it helping? Is it making a difference?

Ground control is the discipline of watching the instruments, interpreting the signals, and making adjustments before problems become crises.

### Slide 2: This is a cross-cutting concern

In software, we call something a "cross-cutting concern" when it affects every part of the system without belonging to any one part. Security is a cross-cutting concern. Logging is a cross-cutting concern. Performance is a cross-cutting concern.

Measurement is a cross-cutting concern too. It is not one team's job. It is not one tool's responsibility. It belongs to all of us.

In aspect-oriented programming, we weave cross-cutting concerns into the fabric of the code. In the same way, we must weave measurement into the fabric of our work -- not as an afterthought, not as a separate report, but as an integral part of how we build and deliver.

Non-functional requirements (NFRs) like reliability, performance, and accessibility are cross-cutting too. They do not have a feature flag. They are always on.

### Slide 3: Coordination is our weakest link

This is an honest assessment: coordination across teams, programmes, and organisations is where we struggle most.

It is not for lack of effort or goodwill. It is because coordination is genuinely hard, especially at scale. The more teams we have, the more connections between them, and the more opportunities for miscommunication, duplication, and drift.

We all must work to make coordination better. Not through more meetings or more governance, but through better tools, better visibility, and better habits. When ground control works well, every team can see where they are, where others are, and where they are all heading.

### Slide 4: Top fears

- **One size doesn't fit all** -- the fear that any measurement framework will be too rigid for the diversity of teams, projects, and contexts across NHS Wales
- **Lack of demo areas** -- the fear that without safe environments to demonstrate progress, work remains invisible and trust erodes
- **Conformance compliance** -- the fear that measurement becomes a tick-box exercise, optimising for compliance rather than genuine improvement

---

### Slide 5: Top Levers

- **Baseline open-source success** -- adopting open-source metrics frameworks (like DORA metrics) as a starting point, then adapting them to our context
- **Rainbow deployments** -- each topic or initiative gets its own deployment environment, making progress visible and demonstrable without risking production
- **Product-service ITIL 5** -- integrating modern product management with ITIL service management to create a coherent framework that serves both innovation and stability

---

## Advice for event creators

### Brainstorms and ideas

- This session covers measurement, which can feel dry. Combat this by making it personal: "How do YOU know if you're doing a good job? What signals tell you that your work matters?"
- Introduce DORA metrics (Deployment Frequency, Lead Time for Changes, Change Failure Rate, Time to Restore Service) as a starting vocabulary. These are well-researched, widely adopted, and provide a common language for teams with very different technology stacks.
- The "rainbow deployments" concept is vivid and practical. Each initiative has its own colour, its own environment, its own dashboard. You can see at a glance which initiatives are progressing and which are stalled.
- Address conformance anxiety directly. Many NHS staff have experienced measurement as surveillance. Reframe it: "We measure to learn, not to punish. The data is for us, not for a report that nobody reads."
- The ITIL 5 reference connects modern agile delivery with established service management. For teams that operate in an ITIL context, this bridge is important.

### Insights

- "Cross-cutting concern" is an excellent metaphor because it names something everyone feels but struggles to articulate: measurement is everyone's problem and nobody's job. Making it a named concern gives it legitimacy.
- Coordination as the "weakest link" is a deliberately vulnerable admission. It signals honesty and invites collective ownership rather than blame.
- Demo areas and rainbow deployments solve two problems at once: they make work visible (coordination) and they provide safe spaces to experiment (innovation). Advocate for them as infrastructure investments, not luxuries.

### Quotations to consider

- "Not everything that counts can be counted, and not everything that can be counted counts." -- William Bruce Cameron
- "Measure what matters, not what's easy." -- inspired by John Doerr
- "In God we trust. All others bring data." -- W. Edwards Deming
- "The goal is not to be perfect by the end. The goal is to be better today." -- Simon Sinek

### References

- "Accelerate" by Nicole Forsgren, Jez Humble, Gene Kim (DORA metrics)
- DORA State of DevOps reports
- ITIL 4/5 Foundation: integrating service management with agile
- "Team Topologies" by Matthew Skelton and Manuel Pais (team interaction patterns)
- GDS Service Standard (UK Government Digital Service)

---

## Workshop ideas

### Activity: Build Your Dashboard (15 minutes)

**Format:** Small groups of 4-5 people

**Step 1 (4 minutes):** Each group imagines they have a dashboard on the wall of their workspace. It shows four metrics that tell them how their work is going. What are those four metrics? They can be technical (deployment frequency, test coverage), team-based (cycle time, satisfaction), or outcome-based (user adoption, error rates). Write each metric on a sticky note.

**Step 2 (4 minutes):** Groups compare their dashboards. Which metrics are common? Which are unique? Discuss: "If every team had these metrics visible, what would change about how we coordinate?"

**Step 3 (4 minutes):** Now each group designs one "coordination metric" -- a metric that would help them work better with OTHER teams, not just their own. Examples: "time from request to response between teams," "number of shared components reused," "time to onboard a new team member from another team."

**Step 4 (3 minutes):** Groups share their coordination metrics. Facilitator identifies the themes and proposes a lightweight "NHS Wales software engineering dashboard" concept built from the group's ideas.

**Facilitator tip:** Resist the urge to prescribe metrics. Let the groups discover them. The best metrics are the ones teams choose for themselves because they find them genuinely useful. If groups struggle, offer the DORA metrics as a starting framework.

**Alternative activity:** "Demo day simulation." Each group has 2 minutes to prepare and deliver a mock demo of something they have worked on recently (real or imagined). The audience gives feedback on: "Did I understand what you built? Did I understand why it matters? Did I understand what happens next?" This practises the habit of making work visible and demonstrates why demo areas matter.
