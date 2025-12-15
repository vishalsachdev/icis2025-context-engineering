# Talk Preparation: "From Tool Users to Capability Architects"
**Monday 3:30 PM | Table Talk**

> **Session**: Teaching Tech Differently: From Tool Users to Capability Architects
> **Convenor**: Vishal Sachdev (University of Illinois at Urbana Champaign)

---

## Core Thesis

Business schools teach students to use technology—Excel formulas, Python scripts, BI dashboards. But AI systems like Claude Skills reveal what employers actually need: graduates who can **architect capabilities**—designing reusable, composable knowledge systems that encode business logic.

**Industry Validation:**
- **Tobi Lütke** (Shopify CEO): *"I really like the term 'context engineering' over prompt engineering. It describes the core skill better: the art of providing all the context for the task to be plausibly solvable by the LLM."* ([source](https://x.com/tobi/status/1935533422589399127))
- **Andrej Karpathy**: *"Think of an LLM like a CPU, and its context window as the RAM. Your job as an engineer is akin to an operating system: load that working memory with just the right code and data for the task."* ([source](https://x.com/karpathy/status/1937902205765607626))

---

## The Problem: What Business Schools Teach Now

| Tool Thinking | Reality |
|--------------|---------|
| "Learn Excel formulas" | Excel formulas are commoditized |
| "Master Python syntax" | AI writes Python faster than students |
| "Use BI dashboards" | Dashboards are point-and-click |

## The Shift: What Employers Actually Need

**Capability Architecture** = Designing reusable, composable knowledge systems that encode business logic.

---

## Evidence: 4 Case Studies From My Work

### Case Study 1: Claude Skills Library
**Repo**: [github.com/vishalsachdev/claude-skills](https://github.com/vishalsachdev/claude-skills)

8 production-ready, reusable capabilities extracted from real projects:

| Skill | What it Encodes |
|-------|-----------------|
| `vibe-coder-sdlc` | Complete software development lifecycle as a composable system |
| `secure-nextjs-api-routes` | 671 lines encoding security best practices (auth, rate limiting, CSRF) |
| `ai-model-cascade` | Fallback logic + cost optimization for AI integration |
| `type-safe-form-validation` | Validation patterns that work client & server |
| `resilient-async-operations` | Memory leak prevention + graceful error handling |
| `advanced-text-search-matching` | Boyer-Moore search + fuzzy matching algorithms |

**The SKILL.md format—encoding business logic as reusable context:**
```yaml
---
name: secure-api-routes
description: This skill should be used when users want to add
             comprehensive security middleware to Next.js API routes
---
```

**Key insight:**
> "A student who can *design* the `secure-nextjs-api-routes` skill has a fundamentally different capability than one who can *use* a security library. The first understands what problems the library solves; the second just calls functions."

---

### Case Study 2: Canvas-MCP
**Repo**: [github.com/vishalsachdev/canvas-mcp](https://github.com/vishalsachdev/canvas-mcp) (33★)

I didn't just *use* Canvas. I built infrastructure that lets AI systems interact with Canvas—a **capability layer**.

| Tool User | Capability Architect |
|-----------|---------------------|
| Uses Canvas dashboards to check grades | Designs MCP server that any AI can use to query Canvas |
| Manually identifies struggling students | Creates bulk_grade_submissions for 99.7% token savings |
| Exports data to Excel | Enables FERPA-compliant analytics with automatic anonymization |

**Key insight:**
> "The MCP protocol is the new API design. Students who understand how to expose capabilities through structured protocols will build the systems that others use."

---

### Case Study 3: AgentLab / VentureBots
**Repo**: [github.com/vishalsachdev/AgentLab](https://github.com/vishalsachdev/AgentLab)

Multi-agent systems where **each agent is a capability**:

| Agent | Encoded Capability |
|-------|--------------------|
| Agent 1 | Idea validation expertise |
| Agent 2 | Market research methodology |
| Agent 3 | Financial modeling logic |
| Agent 4 | Pitch deck structure |
| Agent 5 | Feedback synthesis |

25+ students in current pilot at Gies College of Business.

**Key insight:**
> "We're not teaching students to use 5 AI chatbots. We're teaching them to *architect a team of specialists*—decomposing a complex goal into capabilities and orchestrating them."

---

### Case Study 4: Context Engineering
**Article**: [Context engineering is the new Prompt Engineering](https://chatwithgpt.substack.com/p/context-engineering-is-the-new-prompt)

**What context engineering includes:**
1. Task instructions
2. Few-shot examples
3. Retrieved facts (RAG)
4. Multimodal data
5. Relevant tools
6. State history
7. **Compacting into limited window**

**Key insight:**
> "We teach students to write prompts. We should teach them to *engineer context*—deciding what information an AI needs, how to retrieve it, and how to structure it."

---

## Curriculum Redesign Discussion

### Questions for the Table

1. **If AI can write code, what do we assess?**
   - Proposal: Assess the *skill definition* they create, not the code it produces.

2. **What's the business school equivalent of a "skill"?**
   - Financial modeling workflow encoded as reusable capability
   - Customer segmentation logic that can be applied to any dataset
   - Risk assessment framework with embedded domain expertise

3. **How do we grade "capability architecture"?**
   - Reusability: Can another team use this skill?
   - Composability: Does it integrate with other capabilities?
   - Correctness: Does the encoded logic reflect best practices?

### Concrete Curriculum Module Transformation

| Traditional Module | Capability Architecture Module |
|-------------------|-------------------------------|
| "Excel: PivotTables and VLOOKUP" | "Design a data analysis skill that any AI can invoke" |
| "Python: Pandas for data wrangling" | "Build a data validation capability with clear triggers and outputs" |
| "Tableau: Dashboard design" | "Create a composable reporting system with defined inputs/outputs" |

---

## Soundbites

1. **"The prompt is dead, long live the context"** — We're moving from crafting magic sentences to architecting information systems.

2. **"Skills are the new APIs"** — Just as APIs let systems talk to each other, skills let AI understand and execute domain expertise.

3. **"We teach students to row boats. AI is giving them motors. We need to teach them to design boats."**

4. **"Tool users ask 'how do I use this?' Capability architects ask 'what should this do and why?'"**

5. **"The best prompt engineer is an obsolete job title. The best context engineer is a systems thinker."**

---

## Visual: The Shift

```
                      THE SHIFT

     TOOL USER                    CAPABILITY ARCHITECT
        │                                  │
   Uses Excel ───────────────────► Designs reusable
                                   financial model skill
        │                                  │
   Writes Python ─────────────────► Creates validation
                                   capability with triggers
        │                                  │
   Prompts ChatGPT ───────────────► Engineers context
                                   for complex tasks

   [Knows WHAT to click]          [Knows WHY it works]
```

---

## Additional Angles for Business School Focus

### The "Non-Coder Capability Architect" Opportunity

This is the underexplored angle: **business students don't need to code to be capability architects.**

Claude Skills are written in *Markdown*, not Python:

```yaml
---
name: financial-due-diligence
description: This skill should be used when users want to
             systematically evaluate acquisition targets
---

## Triggers
- User mentions "due diligence", "M&A", "acquisition target"
- User asks about financial health of a company

## Process
1. Request financial statements (10-K, 10-Q)
2. Calculate key ratios: current ratio, debt-to-equity, ROIC
3. Compare to industry benchmarks
4. Flag anomalies for human review
...
```

**Provocation for the table:**
> "A finance major who can write this skill definition—encoding what 'good due diligence' looks like—is more valuable than one who can run the formulas in Excel. The AI runs the formulas. The human defines what matters."

---

### The Three Layers Business Students Should Understand

| Layer | What It Is | Business Role |
|-------|-----------|---------------|
| **Tools** | Excel, Python, Tableau | Being automated away |
| **Capabilities** | Skills, MCP servers, agent workflows | **Where the value is moving** |
| **Strategy** | What capabilities to build, buy, or orchestrate | Still uniquely human |

Most curricula focus on Layer 1. Employers increasingly need Layer 2. Strategy (Layer 3) requires understanding Layer 2.

**Discussion question:**
> "If a consulting firm can encode their frameworks as Claude Skills, what happens to junior analysts?"

---

### MCP as "APIs for AI" — A Business Concept

Canvas-MCP is a perfect teaching example. MCP (Model Context Protocol) is essentially:

> "A standard way to expose business systems to AI agents"

Business students already understand:
- APIs (how systems talk to each other)
- Integration (connecting Salesforce to Slack)
- Data flows (what goes where)

MCP is the same concepts, but for AI. **The student who understands how to define what capabilities a business system should expose to AI is designing the future integration layer.**

**Concrete example:**
> "Imagine you're the product manager for your company's CRM. Your job isn't just 'make the dashboard better.' It's 'what capabilities should AI agents have access to?' Can they read contacts? Create deals? Send emails on behalf of salespeople? These are business decisions, not engineering decisions."

---

### From "Prompt Engineering" to "Capability Specification"

A reframe that resonates with business students:

| Prompt Engineering | Capability Specification |
|-------------------|-------------------------|
| "Write me a marketing email" | Define the inputs, outputs, constraints, and quality criteria for marketing emails |
| One-shot, disposable | Reusable, versionable, auditable |
| Art/craft | Engineering/design |
| Individual skill | Organizational asset |

**The business case:**
> "A great prompt dies with the person who wrote it. A great skill definition becomes organizational IP—it can be reused, improved, and scaled."

---

### What "Teaching AI" Actually Means

From the session description: *"When AI can be 'taught' domain expertise through structured skill packages..."*

**What makes a skill effective:**
1. **Clear triggers** — When should AI activate this capability?
2. **Domain context** — What does "good" look like in this field?
3. **Process structure** — What steps should AI follow?
4. **Quality criteria** — How do we know if AI did it right?
5. **Edge cases** — What should AI escalate to humans?

**This is essentially a PRD (Product Requirements Document) for AI behavior.**

Business students already learn to write requirements. The skill is transferable—they just need to learn the new medium.

---

### The "Judgment Layer" — What AI Can't Do

Balance the capability architect framing with what remains human:

| AI Does Well | Humans Must Do |
|-------------|----------------|
| Execute defined processes | Decide which processes matter |
| Apply consistent logic | Make ethical tradeoffs |
| Process massive data | Interpret context and politics |
| Generate options | Choose among options with incomplete information |

**Key point for business students:**
> "Your job isn't to compete with AI at execution. It's to be the person who defines what 'good execution' means—and takes responsibility when it doesn't work."

---

### Concrete Assignment Idea

If someone asks "how would you actually teach this?":

**Assignment: "Build a Capability"**

> Design a Claude Skill for a business function you understand well. Your deliverable is a SKILL.md file that includes:
> 1. Clear description of when this skill should activate
> 2. The business logic it encodes (what does "good" look like?)
> 3. Inputs required and outputs produced
> 4. Quality criteria for evaluating outputs
> 5. Edge cases that should escalate to humans
>
> You will be graded on: clarity, completeness, reusability, and whether a classmate can successfully use your skill for a realistic scenario.

**Why this works:**
- No coding required
- Forces deep thinking about business processes
- Produces something tangible and shareable
- Can be tested by peers (composability!)

---

### The Emerging Job Titles

For career-minded students:

| Emerging Role | What They Do |
|--------------|-------------|
| **AI Product Manager** | Defines what capabilities AI systems should have |
| **Capability Designer** | Creates reusable skill definitions and agent workflows |
| **AI Operations Manager** | Monitors, evaluates, and improves deployed AI systems |
| **Context Engineer** | Designs what information AI systems need to do their jobs |
| **Agent Architect** | Designs multi-agent systems for complex workflows |

**None of these require deep coding skills. All require deep business understanding.**

---

### Provocative Closing Question

End the table talk with:

> "In 5 years, will 'I know Excel' be on anyone's resume? Probably not. What will be? My bet: 'I designed 12 capabilities that are still in production use.' The question is: are we teaching students to create those capabilities, or just to use tools that won't matter?"

---

## Resources

### My Work
- **GitHub**: [github.com/vishalsachdev](https://github.com/vishalsachdev) (66+ repos)
- **Substack**: [chatwithgpt.substack.com](https://chatwithgpt.substack.com/)
- **Canvas-MCP**: [github.com/vishalsachdev/canvas-mcp](https://github.com/vishalsachdev/canvas-mcp)
- **Claude Skills**: [github.com/vishalsachdev/claude-skills](https://github.com/vishalsachdev/claude-skills)
- **AgentLab**: [github.com/vishalsachdev/AgentLab](https://github.com/vishalsachdev/AgentLab)

### Industry Sources
- [Tobi Lütke on Context Engineering](https://x.com/tobi/status/1935533422589399127)
- [Karpathy on Context Engineering](https://x.com/karpathy/status/1937902205765607626)
- [Simon Willison: Context Engineering](https://simonwillison.net/2025/jun/27/context-engineering/)
- [O'Reilly: Context Engineering Guide](https://www.oreilly.com/radar/context-engineering-bringing-engineering-discipline-to-prompts-part-1/)

---

*Created: 2025-12-14 | Last Updated: 2025-12-14*
