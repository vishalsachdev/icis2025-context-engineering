# Table Talk Role-Play Exercises
**Teaching Tech Differently: From Tool Users to Capability Architects**

These exercises put participants in unfamiliar domains to simulate what students experience when asked to architect capabilities in areas where they're still learning.

---

## Exercise 1: The ER Triage Skill
**Domain:** Emergency medicine (very unfamiliar to business faculty)
**Duration:** 15-20 minutes
**Group size:** Pairs or groups of 3

### Setup (2 min)

Read aloud:

> "You're an AI product manager at a hospital. The ER wants an AI assistant that helps nurses with initial patient triage. You don't have a medical degree. Neither do most of your future students when they enter the workforce.
>
> Your job isn't to know medicine. Your job is to **define what 'good triage' looks like** well enough that an AI can help—while knowing when to escalate to humans."

### The Task (10-12 min)

In pairs or small groups, draft a **SKILL.md** for "ER Triage Assistant":

```markdown
---
name: er-triage-assistant
description: [Your description here]
---

## TRIGGERS
When should this skill activate?
-
-

## INPUTS
What information does the AI need from the nurse/patient?
-
-
-

## PROCESS
What steps should the AI follow?
1.
2.
3.

## QUALITY CRITERIA
How do we know the triage recommendation was good?
-
-

## ESCALATION
When must the AI defer to humans immediately?
-
-
```

### Debrief Questions (5 min)

After groups share their drafts:

1. "You just defined a capability in a domain where you're NOT the expert. How did that feel?"
2. "What did you have to figure out vs. look up vs. defer to humans?"
3. "This is exactly what we're asking students to do—architect capabilities in domains they're learning."

### Learning Objective

**You don't need domain expertise to architect capabilities. You need to know what questions to ask and when to escalate.**

---

## Exercise 2: The Insurance Claim Fraud Detector
**Domain:** Insurance claims processing (adjacent to business but unfamiliar specifics)
**Duration:** 15-20 minutes
**Group size:** Pairs or groups of 3

### Setup (2 min)

Read aloud:

> "You've been hired by an insurance company to design an AI capability that flags potentially fraudulent claims for human review. You're not a claims adjuster. You've never processed a claim.
>
> But you need to define what 'suspicious' looks like well enough for AI to help—without making the AI the final decision-maker on fraud."

### The Task (10-12 min)

Draft a **SKILL.md** for "Claim Fraud Flagger":

```markdown
---
name: claim-fraud-flagger
description: [Your description here]
---

## TRIGGERS
What types of claims should this skill analyze?
-
-

## RED FLAGS
What patterns suggest possible fraud? (You'll have to guess—that's the point)
-
-
-
-

## CONFIDENCE LEVELS
How certain must the AI be before flagging a claim?
- Low confidence:
- Medium confidence:
- High confidence:

## HUMAN HANDOFF
What information does the human reviewer need to see?
-
-
-

## ETHICAL BOUNDARIES
What must this skill NEVER do?
-
-
```

### The Twist (at 5-minute mark)

Interrupt the groups:

> "The legal team just told you: the AI cannot use zip code, neighborhood, or demographic proxies as fraud indicators due to fair lending and discrimination concerns. Revise your skill."

Give them 3 more minutes to adapt.

### Debrief Questions (5 min)

1. "How did you handle defining 'suspicious' without being a fraud expert?"
2. "What was harder: the domain knowledge gap or the ethical constraints?"
3. "How did the mid-task constraint change your design? This happens constantly in real projects."
4. "Students face this: partial knowledge, changing requirements, ethical boundaries."

### Learning Objective

**Capability architecture requires defining judgment criteria in domains where you're not the expert—and encoding ethical constraints that may change.**

---

## Exercise 3: The Peer Review Skill
**Domain:** Academic peer review (familiar process, unfamiliar to automate)
**Duration:** 15-20 minutes
**Group size:** Pairs or groups of 3

### Setup (2 min)

Read aloud:

> "A journal editor wants AI to help with initial screening of submissions—not to accept/reject, but to flag issues and route papers to appropriate reviewers.
>
> You've all DONE peer review. But can you define what you actually do well enough to teach an AI? This is the capability architecture challenge: making tacit knowledge explicit."

### The Task (10-12 min)

Draft a **SKILL.md** for "Manuscript Initial Screener":

```markdown
---
name: manuscript-screener
description: [Your description here]
---

## INPUTS
What does the AI receive?
- [ ] Full paper
- [ ] Abstract only
- [ ] Author information
- [ ] Other:

## SCREENING CRITERIA
What makes a paper suitable for review?

### Scope Fit
-
-

### Methodological Minimums
-
-

### Completeness Checks
-
-

## ROUTING LOGIC
How should papers be matched to reviewers?
-
-

## FLAGS FOR EDITOR
What requires human judgment? (Don't automate these)
-
-

## BOUNDARIES
What must this skill NEVER assess?
-
-
```

### Debrief Questions (5 min)

1. "You know this domain intimately—yet was it easy to make your tacit knowledge explicit?"
2. "Where did you disagree with your partner? That's where judgment lives."
3. "What did you decide the AI should NEVER do? Why?"
4. "Now imagine a student trying to do this for a domain they DON'T know yet."

### Learning Objective

**Even domain experts struggle to make tacit knowledge explicit. That's the core skill of capability architecture—and it's teachable.**

---

## Comparison of Exercises

| Dimension | ER Triage | Fraud Detection | Peer Review |
|-----------|-----------|-----------------|-------------|
| **Domain familiarity** | Very low | Low-medium | High |
| **Ethical complexity** | Life/death stakes | Fairness/bias | Academic integrity |
| **Core tension** | "I don't know medicine" | "I don't know fraud patterns" | "I can't articulate what I do" |
| **Key insight** | Architect without expertise | Constraints change design | Tacit knowledge is hard |
| **Energy level** | High (dramatic) | Medium-high | Medium (reflective) |
| **Best for** | Maximum discomfort | Business-adjacent relevance | Self-reflection |

---

## Facilitation Tips

1. **Embrace the discomfort.** The point is that it's hard. Don't rescue them.
2. **Time-box strictly.** Incomplete drafts are fine—the discussion matters more.
3. **Encourage "I don't know" sections.** Marking uncertainty is a skill.
4. **Compare across groups.** Different groups will make different choices. That's the point.
5. **Connect to students.** "This is what your students feel in YOUR class."

---

## Adaptation for Your Own Courses

After the exercise, invite participants to consider:
- What domain could YOU use in YOUR course?
- What's unfamiliar enough to create productive struggle?
- What's familiar enough that students can make progress?

---

*Created: 2025-12-14*
*Vishal Sachdev | University of Illinois at Urbana-Champaign*
*GitHub: github.com/vishalsachdev | Substack: chatwithgpt.substack.com*
