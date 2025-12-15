# Conceptual Framework
**Context Engineering Across the Business Analysis Workflow**

---

## The Core Insight

Every stage of business analysis—understanding, deciding, specifying—can now be AI-enabled. The meta-skill across all three is **context engineering**: knowing what context to provide so AI can help you effectively.

---

## The Framework

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│                   CONTEXT ENGINEERING                       │
│        (How you work WITH AI at every stage)                │
│                                                             │
│   ┌─────────────┐   ┌─────────────┐   ┌─────────────┐      │
│   │             │   │             │   │             │      │
│   │ UNDERSTAND  │──▶│   DECIDE    │──▶│   SPECIFY   │      │
│   │             │   │             │   │             │      │
│   │ (AI helps   │   │ (AI helps   │   │ (AI helps   │      │
│   │  analyze)   │   │  evaluate)  │   │  execute)   │      │
│   │             │   │             │   │             │      │
│   └─────────────┘   └─────────────┘   └─────────────┘      │
│         │                 │                 │              │
│         ▼                 ▼                 ▼              │
│   What context      What context      What context        │
│   helps AI          helps AI          helps AI            │
│   understand        evaluate          execute             │
│   the problem?      options?          correctly?          │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

---

## The Three Stages

### Stage 1: UNDERSTAND
**Goal:** See the problem clearly

| Without AI | With AI |
|-----------|---------|
| Analyze data manually | AI surfaces patterns, synthesizes research |
| Interview stakeholders | AI helps identify gaps and themes |
| Research competitors | AI summarizes and compares |

**Context engineering question:** What context helps AI understand the problem?
- Raw data + what you're looking for
- Industry context for correct interpretation
- What you already know (so AI doesn't repeat it)
- What would surprise you (so AI focuses on anomalies)

---

### Stage 2: DECIDE
**Goal:** Choose wisely among options

| Without AI | With AI |
|-----------|---------|
| Brainstorm options | AI generates and stress-tests alternatives |
| Evaluate trade-offs | AI models scenarios, surfaces hidden costs |
| Build business case | AI helps quantify and present |

**Context engineering question:** What context helps AI evaluate options?
- The options you're considering
- Constraints (budget, time, politics, ethics)
- Criteria for success and how to weight them
- Stakeholder perspectives to consider

---

### Stage 3: SPECIFY
**Goal:** Define what "good" looks like for execution

| Without AI | With AI |
|-----------|---------|
| Write requirements docs | AI helps draft and refine |
| Create process documentation | AI executes the process directly |
| Define acceptance criteria | Criteria become executable specifications |

**Context engineering question:** What context helps AI execute correctly?
- Task description and scope
- Examples of good output
- Constraints and guardrails
- Tools available
- Escalation criteria (when to stop and ask)

**New artifact:** The "skill"—a specification that AI itself executes.

---

## What Is Context Engineering?

The term gained momentum in mid-2025 when two influential voices in tech endorsed it:

### Andrej Karpathy's Definition

**Who:** Former Director of AI at Tesla (led Autopilot), founding member of OpenAI, creator of widely-used neural network courses at Stanford. One of the most respected voices in AI.

> "Context engineering is the delicate art and science of filling the context window with just the right information for the next step."
>
> — [Tweet, June 2025](https://x.com/karpathy/status/1937902205765607626)

**His CPU/RAM analogy:** "Think of an LLM like a CPU, and its context window as the RAM. Your job is akin to an operating system: load that working memory with just the right code and data."

**Components:** Task descriptions, few-shot examples, retrieved data (RAG), tools, state/history, and compacting it all into limited space.

### Tobi Lütke's Definition

**Who:** CEO of Shopify, one of the world's largest e-commerce platforms. Under his leadership, Shopify achieved 80% GitHub Copilot adoption before ChatGPT even launched.

> "I really like the term 'context engineering' over prompt engineering. It describes the core skill better: the art of providing all the context for the task to be plausibly solvable by the LLM."
>
> — [Tweet, June 2025](https://x.com/tobi/status/1935533422589399127)

**Key insight from the [Acquired Podcast](https://www.acquired.fm/episodes/how-to-live-in-everyone-elses-future-with-shopify-ceo-tobi-lutke):** "The fundamental skill of using AI well is to be able to state a problem with enough context, in such a way that without any additional pieces of information, the task is plausibly solvable."

### Why It Matters Beyond AI

Tobi: "I think it makes you better in so many other ways that has nothing to do with AI."

Learning to state problems completely makes you a better thinker, period.

---

## How This Changes Business Education

### The Old Question
> "Do we teach business fundamentals OR AI skills?"

### The New Answer
> "We teach business fundamentals WITH AI as collaborator. Context engineering is how you collaborate with AI at every stage."

### What Students Still Need to Learn
- How to understand business problems (Stage 1)
- How to make decisions under uncertainty (Stage 2)
- How to specify requirements clearly (Stage 3)

### What's New
- Each stage is now AI-enabled
- Context engineering applies to all three stages
- The output of Stage 3 might be a specification FOR AI (a "skill"), not just a requirements doc for humans

---

## Implications for Curriculum

| Traditional Module | Context Engineering Lens |
|-------------------|-------------------------|
| Business analysis | + How to provide context for AI-assisted analysis |
| Decision-making | + How to provide context for AI-assisted evaluation |
| Requirements writing | + How to write specifications AI can execute |

**The fundamentals don't go away. They become the foundation for effective AI collaboration.**

---

## The Skill as Artifact

When Stage 3 produces a specification that AI executes, that specification is a **skill**:

```yaml
---
name: [what this capability is called]
description: [when this should activate]
---

## Triggers
[When should AI use this?]

## Inputs
[What information does AI need?]

## Process
[What steps should AI follow?]

## Quality Criteria
[How do we know it worked?]

## Escalation
[When should AI stop and ask a human?]
```

This is **context engineering made durable**—a reusable context package.

---

## Faculty as Capability Architects

There's a prerequisite to teaching this: **you can't teach building until you've built.**

### The Shift in Faculty Role

| Traditional Role | New Role |
|------------------|----------|
| Domain expert who lectures | Capability architect who demonstrates |
| Assigns tools for students to use | Designs capabilities for students to extend |
| Teaches frameworks abstractly | Models the building process explicitly |

### Why Building Matters

1. **Experience teaches what papers can't.** The struggle of specifying business logic for AI reveals edge cases, ambiguities, and design trade-offs that theory alone won't surface.

2. **Artifacts become teaching tools.** A skill you built for your course becomes something students can examine, critique, and extend.

3. **Credibility through practice.** Students can tell when you've done the work vs. just read about it.

### Starter Builds for Faculty

| If You Teach... | You Could Build... |
|-----------------|-------------------|
| Accounting | A skill that flags unusual journal entries for review |
| Marketing | A skill that analyzes campaign copy for brand consistency |
| Finance | A skill that stress-tests DCF model assumptions |
| Operations | A skill that identifies supply chain bottlenecks |
| Strategy | A skill that maps competitive positioning from 10-Ks |

**One build teaches more than ten papers.**

---

## Sources

- [Karpathy on Context Engineering](https://x.com/karpathy/status/1937902205765607626)
- [Tobi Lütke on Context Engineering](https://x.com/tobi/status/1935533422589399127)
- [Acquired Podcast with Tobi Lütke](https://www.acquired.fm/episodes/how-to-live-in-everyone-elses-future-with-shopify-ceo-tobi-lutke)
- [LangChain: Context Engineering for Agents](https://blog.langchain.com/context-engineering-for-agents/)

---

*Created: 2025-12-15*
*Vishal Sachdev | University of Illinois at Urbana-Champaign*
