# Context Engineering Across the Business Workflow
**Teaching Tech Differently | ICIS 2025**

---

## The Core Insight

Every stage of business analysis—understanding, deciding, specifying—can now be AI-enabled.

The meta-skill across all three is **context engineering**: knowing what context to provide so AI can help you effectively.

---

## The Framework

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│                   CONTEXT ENGINEERING                       │
│        (How you work WITH AI at every stage)                │
│                                                             │
│   ┌─────────────┐   ┌─────────────┐   ┌─────────────┐      │
│   │ UNDERSTAND  │──▶│   DECIDE    │──▶│   SPECIFY   │      │
│   │             │   │             │   │             │      │
│   │  AI helps   │   │  AI helps   │   │  AI helps   │      │
│   │  analyze    │   │  evaluate   │   │  execute    │      │
│   └─────────────┘   └─────────────┘   └─────────────┘      │
│         │                 │                 │              │
│    What context     What context      What context         │
│    helps AI         helps AI          helps AI             │
│    see the          weigh             do the work          │
│    problem?         options?          correctly?           │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**Business schools teach all three stages. What's new: each can be AI-enabled.**

---

## What Is Context Engineering?

The term gained momentum in mid-2025 when two influential voices in tech endorsed it:

**Tobi Lütke** — CEO of Shopify, one of the world's largest e-commerce platforms. Under his leadership, Shopify achieved 80% Copilot adoption before ChatGPT even launched.

> *"I really like the term 'context engineering' over prompt engineering. It describes the core skill better: the art of providing all the context for the task to be plausibly solvable by the LLM."*
>
> — [Tweet, June 2025](https://x.com/tobi/status/1935533422589399127)

**Andrej Karpathy** — Former Director of AI at Tesla, founding member of OpenAI, created the widely-used neural network courses at Stanford.

> *"Context engineering is the delicate art and science of filling the context window with just the right information for the next step."*
>
> — [Tweet, June 2025](https://x.com/karpathy/status/1937902205765607626)

Karpathy's analogy: *"Think of an LLM like a CPU, and its context window as the RAM. Your job is akin to an operating system: load that working memory with just the right code and data."*

**Tobi's key insight:** "I think it makes you better in so many other ways that has nothing to do with AI." Learning to state problems completely makes you a better thinker, period.

---

## The Three Stages (All AI-Enabled)

### Stage 1: UNDERSTAND
| Without AI | With AI |
|-----------|---------|
| Analyze data manually | AI surfaces patterns |
| Research competitors | AI synthesizes and compares |
| Interview stakeholders | AI identifies gaps and themes |

**Context question:** What helps AI see the problem clearly?

### Stage 2: DECIDE
| Without AI | With AI |
|-----------|---------|
| Brainstorm options | AI generates alternatives |
| Evaluate trade-offs | AI models scenarios |
| Build business case | AI quantifies and stress-tests |

**Context question:** What helps AI weigh options appropriately?

### Stage 3: SPECIFY
| Without AI | With AI |
|-----------|---------|
| Write requirements docs | AI helps draft |
| Create process documentation | **AI executes the process** |
| Define acceptance criteria | Criteria become executable |

**Context question:** What helps AI do the work correctly?

---

## The New Artifact: The "Skill"

When Stage 3 produces a specification that AI executes:

```yaml
---
name: financial-due-diligence
description: Systematically evaluate acquisition targets
---

## Triggers
- User mentions "due diligence", "M&A", "acquisition"

## Process
1. Request financial statements (10-K, 10-Q)
2. Calculate key ratios: current ratio, debt-to-equity, ROIC
3. Compare to industry benchmarks
4. Flag anomalies for human review

## Escalation
- Unusual accounting treatments → human CPA
- Related party transactions → human review
```

**This is context engineering made durable—a reusable context package.**

---

## Implications for Curriculum

| Traditional Module | Context Engineering Lens |
|-------------------|-------------------------|
| Business analysis | + How to provide context for AI-assisted analysis |
| Decision-making | + How to provide context for AI-assisted evaluation |
| Requirements writing | + How to write specifications AI can execute |

**The fundamentals don't go away. They become the foundation for AI collaboration.**

---

## Discussion Questions

1. How do we teach "context engineering" explicitly?
2. Do students need Stage 1 & 2 skills before Stage 3?
3. How do we assess the quality of a specification?

---

## Resources

| Resource | Link |
|----------|------|
| Claude Skills Library | github.com/vishalsachdev/claude-skills |
| Canvas MCP Server | github.com/vishalsachdev/canvas-mcp |
| Writing on AI + Education | chatwithgpt.substack.com |
| All Repos | github.com/vishalsachdev |

---

**Vishal Sachdev** | University of Illinois at Urbana-Champaign | Gies College of Business

*Let's continue the conversation: find me at the conference or reach out online.*

---

*ICIS 2025 | Created: 2025-12-15*
