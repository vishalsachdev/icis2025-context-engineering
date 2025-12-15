# Context Engineering Exercise
**Teaching Tech Differently | ICIS 2025**

---

## The Challenge

You've been hired by an insurance company to design an AI capability that flags potentially fraudulent claims for human review.

**You're not a claims adjuster. You've never processed a claim.**

But you need to define what "suspicious" looks like well enough for AI to help—without making the AI the final decision-maker on fraud.

---

## Your Task: Draft a SKILL.md

Work with your partner(s) for 10 minutes. Fill in what you can. Mark what you're uncertain about.

```
---
name: claim-fraud-flagger
description: _______________________________________________
             _______________________________________________
---
```

### TRIGGERS
*What types of claims should this skill analyze?*

1. ________________________________________________________
2. ________________________________________________________

### RED FLAGS
*What patterns suggest possible fraud?*

1. ________________________________________________________
2. ________________________________________________________
3. ________________________________________________________
4. ________________________________________________________

### CONFIDENCE LEVELS
*How certain must the AI be before flagging?*

| Level | Threshold | Action |
|-------|-----------|--------|
| Low | | |
| Medium | | |
| High | | |

### HUMAN HANDOFF
*What does the human reviewer need to see?*

1. ________________________________________________________
2. ________________________________________________________
3. ________________________________________________________

### ETHICAL BOUNDARIES
*What must this skill NEVER do?*

1. ________________________________________________________
2. ________________________________________________________

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

| Stage | What You Did |
|-------|-------------|
| **UNDERSTAND** | Tried to grasp a problem you're not expert in |
| **DECIDE** | Chose what to flag vs. escalate to humans |
| **SPECIFY** | Wrote it in a format AI could execute |

At every stage, you practiced **context engineering**—figuring out what information matters, how to structure it, what to include and exclude.

**This is what we're asking students to do.**

Business schools already teach understanding and decision-making. What's new:
- All three stages can be AI-enabled
- The output of Stage 3 might be a specification AI itself executes
- Context engineering is the meta-skill across all three

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

## Let's Continue the Conversation

**Vishal Sachdev**
University of Illinois at Urbana-Champaign
Gies College of Business

- GitHub: [github.com/vishalsachdev](https://github.com/vishalsachdev)
- Substack: [chatwithgpt.substack.com](https://chatwithgpt.substack.com)
- Claude Skills Library: [github.com/vishalsachdev/claude-skills](https://github.com/vishalsachdev/claude-skills)

*What exercises are YOU trying? I'd love to learn from you.*

---

*ICIS 2025 | Created: 2025-12-15*
