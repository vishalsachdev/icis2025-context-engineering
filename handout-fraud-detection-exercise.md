# Context Engineering Exercise
**Teaching Tech Differently | ICIS 2025**

---

## The Challenge

You've been hired by an insurance company to design an AI capability that flags potentially fraudulent claims for human review.

**You're not a claims adjuster. You've never processed a claim.**

But you need to define what "suspicious" looks like well enough for AI to help—without making the AI the final decision-maker on fraud.

---

## Your Task: Design a Claude Skill

Using the **Claude Skills** format, draft a reusable specification. This is the actual format used by Claude Code.

Work with your partner(s). Fill in what you can. Mark what you're uncertain about.

```yaml
---
name: claim-fraud-flagger
description: This skill should be used when ____________________
             ________________________________________________
---
```

### Purpose
*What does this skill accomplish? (1-2 sentences)*

_____________________________________________________________
_____________________________________________________________

### When to Use
*What triggers this skill? What types of claims should it analyze?*

- ________________________________________________________
- ________________________________________________________

### How It Works
*What patterns suggest possible fraud? List 3-4 red flags.*

1. ________________________________________________________
2. ________________________________________________________
3. ________________________________________________________
4. ________________________________________________________

### Human Handoff
*When should AI stop and escalate to a human? What must it NEVER decide alone?*

**Escalate when:** ___________________________________________
**Never:** ___________________________________________________

---

## The Twist

**New constraint from Legal:**

> "The AI cannot use zip code, neighborhood, or demographic proxies as fraud indicators due to fair lending and discrimination concerns."

**How does this change your design?**

_____________________________________________________________
_____________________________________________________________
_____________________________________________________________

---

## Reflection

After the exercise, consider:

| Question | Your Response |
|----------|---------------|
| How did you define "suspicious" without being a fraud expert? | |
| What was harder: the domain gap or the ethical constraints? | |
| How did the mid-task constraint change your thinking? | |

---

## The Point

You just worked through three stages:

| Stage | What You Did | Skill Section |
|-------|-------------|---------------|
| **UNDERSTAND** | Grasped a problem you're not expert in | Purpose, When to Use |
| **DECIDE** | Chose what to flag vs. escalate | Human Handoff |
| **SPECIFY** | Wrote it in a format AI could execute | How It Works |

At every stage, you practiced **context engineering**—figuring out what information matters, how to structure it, what to include and exclude.

**The format you used is real.** Claude Skills (SKILL.md files) are how developers teach AI domain expertise. The sections—Purpose, When to Use, How It Works, Human Handoff—are the actual structure.

Business schools already teach understanding and decision-making. What's new:
- All three stages can be AI-enabled
- The output of Stage 3 is a reusable capability that encodes business logic
- Context engineering is the meta-skill; Claude Skills are the artifact

---

## Try This With Your Students

Adapt this exercise for your course:

| Your Course | Possible Unfamiliar Domain |
|-------------|---------------------------|
| Analytics | Medical diagnosis support |
| Finance | Agricultural loan assessment |
| Marketing | Legal ad compliance |
| Operations | Air traffic scheduling |
| Strategy | Refugee resettlement matching |

The domain should be unfamiliar enough to create struggle, familiar enough to make progress.

---

## Your Next Step: Become a Builder

You just did in 15 minutes what most faculty haven't tried: you designed an AI capability.

**The best way to teach context engineering is to practice it yourself.**

What could you build for YOUR domain?

| If You Teach... | You Could Build... |
|-----------------|-------------------|
| Accounting | A skill that flags unusual journal entries |
| Marketing | A skill that analyzes campaign copy for brand consistency |
| Finance | A skill that stress-tests DCF assumptions |
| Operations | A skill that identifies supply chain bottlenecks |
| Strategy | A skill that maps competitive positioning |

**One build teaches more than ten papers.**

---

## Let's Continue the Conversation

**Vishal Sachdev**
University of Illinois at Urbana-Champaign
Gies College of Business

- GitHub: [github.com/vishalsachdev](https://github.com/vishalsachdev)
- Substack: [chatwithgpt.substack.com](https://chatwithgpt.substack.com)
- Claude Skills Library: [github.com/vishalsachdev/claude-skills](https://github.com/vishalsachdev/claude-skills)

*What will YOU build? I'd love to learn from you.*

---

*ICIS 2025 | Created: 2025-12-15*
