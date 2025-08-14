---
marp: true
theme: custom
header: AI Workshop for Engineers
footer: SMARTSHEET © 2025
paginate: true
backgroundColor: white
size: 16:9
---

<!-- _class: title -->
# AI Workshop for Engineers
## Integrating AI into Daily Engineering Workflows

**Transform Your Development Process with AI-Powered Collaboration**

---

## Workshop Overview
### Duration: 60 minutes

- **Introduction** (5 min) - AI in engineering workflows overview
- **Code Review Demo** (20 min) - Live AI-assisted code review process
- **Custom Prompts Creation** (15 min) - Building your "gems" toolkit
- **Practical Application** (15 min) - Adapting existing workflows
- **Q&A and Wrap-up** (5 min) - Questions and key takeaways

---

<!-- _class: section -->
# Introduction
## The "Holding It Right" Concept
![Holding It Right Concept](iphone4.png)

---

## AI in Engineering Workflows

### The Reality Check
- AI is not magic - it's a **skill amplifier**
- Success comes from **iterative, collaborative** usage
- Most engineers are "holding it wrong" initially

### Core Principle: Multi-Step Process
- **Not**: Fire-and-forget commands
- **Yes**: Conversational refinement and iteration

---

## Common "Holding It Wrong" Patterns

### ❌ Single-Shot Approach
```
"Write a function to parse JSON"
[Copy code without review]
```

### ✅ Collaborative Approach
```
"Help me design a robust JSON parser"
→ Discuss requirements
→ Review proposed approach
→ Iterate on edge cases
→ Validate final implementation
```

---

## AI as Your Engineering Pair Partner

### Traditional Pairing
- **Human + Human** = Shared knowledge, different perspectives

### AI-Enhanced Pairing
- **Human + AI** = Domain expertise + vast pattern recognition
- AI doesn't replace judgment - it **amplifies** capabilities
- Best results come from **continuous collaboration**

---

<!-- _class: section -->
# Code Review Demo
## AI-Assisted Analysis Process

---

## Demo Setup: Reviewing a Pull Request

### Scenario
- Need to understand impact and identify issues

### Tools We'll Use
- **Github Copilot** - Code generation and analysis in the GitHub UI
- **Claude/Cursor/Copilot** - Code analysis and explanation
- **Multi-step workflow** - Iterative understanding

---

## Step 1: High-Level Overview

### Initial AI Prompt
```
"Help me understand this pull request. Here are the changed files:
[File list]

Please analyze:
1. What is the main purpose of these changes?
2. Which areas of the system are affected?
3. What should I focus on during review?"
```

### What We Get
- **Context understanding** - Overall purpose and scope
- **Risk assessment** - Critical areas to examine
- **Review strategy** - Focused approach rather than random browsing

---

## Step 2: Deep Dive Analysis

### Follow-up Prompts
```
"Let's examine the [SPECIFICS FROM RESPONSE]:

Questions:
- Are there any backward compatibility issues?
- ...
```

### Iterative Refinement
- Start broad → narrow focus
- AI highlights concerns → human validates context
- Continuous back-and-forth dialogue

---

## Step 3: Edge Case Discovery

### Pattern Recognition
```
"I see error handling was added here:
[Error handling code]

Help me think through edge cases:
- What error scenarios might be missed?
- Are there race conditions to consider?
- How does this interact with existing error handling?"
```

### AI's Strength
- **Pattern matching** against thousands of similar scenarios
- **Edge case identification** from broader experience
- **Security implications** you might overlook

---

## Step 4: Testing Strategy

### Validation Approach
```
"Based on this code review, help me design a testing strategy:

1. What unit tests are critical?
2. What integration scenarios need validation?
3. What performance implications should we test?"
```

### Collaborative Test Design
- AI suggests test cases → Human adds domain context
- Identifies testing gaps → Focus efforts efficiently
- Creates reproducible validation plan for use later

---

## Demo Takeaways

### What We Achieved
- **Code Review** → **< 15 minutes** with AI assistance
- **Surface-level scan** → **Deep architectural understanding**
- **Reactive bug hunting** → **Proactive risk identification**

### The Secret Sauce
- **Iterative questioning** - Build understanding step by step
- **Domain context** - You provide business logic, AI provides patterns
- **Collaborative refinement** - Neither human nor AI alone

---

<!-- _class: section -->
# Custom Prompts Creation
## Building Your "Gems" Toolkit

---

## What Are "Gems"?

### Definition
**Custom prompts** that capture your specific workflows and context

### Why They Matter
- **Consistency** - Same quality analysis every time
- **Efficiency** - Skip repetitive context-setting
- **Team alignment** - Shared approaches and standards

---

## Anatomy of a Great Gem

### Essential Components
1. **Context setting** - What's the situation?
2. **Role definition** - What expertise do you need?
3. **Output specification** - What format do you want?
4. **Iteration guidance** - How to refine results?

---

## Example Gem: Code Review Assistant

```markdown
# Code Review Gem

You are an experienced software engineer conducting a thorough code review.

## Context
I'm reviewing [LANGUAGE] code for [PROJECT_TYPE]. Focus on:

- Security vulnerabilities
- Performance implications
- Maintainability concerns

## Process

1. First, give me a high-level summary
2. Identify the 3 most critical issues
3. Suggest specific improvements
4. Ask clarifying questions about business context

## Output Format

- **Summary**: [2-3 sentences]
- **Critical Issues**: [Numbered list]
- **Recommendations**: [Specific, actionable items]
- **Questions**: [Context I should provide]
```

---

## Gem Creation Workshop

### Your Turn: Personal Workflow Gems
**Think about your daily tasks:**
- Code reviews
- Architecture decisions
- Bug investigations
- Documentation writing
- Meeting preparation

**Pick one and create a gem following the pattern**

---

## Example Gem: Architecture Decision

```markdown
# Architecture Decision Gem

You are a senior systems architect helping evaluate technology choices.

## Context
I need to make a decision about [COMPONENT/TECHNOLOGY] for [PROJECT].

## Analysis Framework
1. **Requirements Analysis**: What are the key constraints?
2. **Option Evaluation**: Compare 2-3 viable alternatives
3. **Trade-off Assessment**: Performance, complexity, cost, team skills
4. **Risk Analysis**: What could go wrong with each option?
5. **Recommendation**: Clear choice with rationale

## Follow-up Questions
- What's missing from my requirement analysis?
- What alternatives should I consider?
- What risks am I not seeing?
```

---

## Example Gem (reviewing a patch diff)

```markdown
# Patch Diff Review Gem
You are a senior engineer reviewing a patch diff.

## Context

Review the provided patch diff, if the user hasn't provided you with one, then ask them for it.

Focus on:

- Architectural impact
- Security implications
- Performance considerations

## Process

1. First, give me a high-level summary of the changes
2. Identify the 3 most critical issues
3. Suggest specific improvements
4. Ask clarifying questions about business context
```

---

## Gem Library Management

### Organization Strategy
- **Personal gems** - Your specific workflows
- **Team gems** - Shared standards and processes
- **Project gems** - Context-specific prompts

### Version Control
- Store gems (system prompts) in a **team wiki**
- **Document and share** effective patterns
- **Iterate and improve** based on results

---

## Building Team Gem Libraries

### Collaborative Development
1. **Share successful gems/prompts** in team channels
2. **Customize for team context** - coding standards, architecture patterns
3. **Create project-specific gems** - domain knowledge, business rules
4. **Regular review and improvement** - What's working? What's not?

---

<!-- _class: section -->
# Practical Application
## Adapting Your Existing Workflows

---

## Workflow Transformation Strategy

### Step 1: Audit Current Processes
- **List your daily engineering tasks**
- **Identify repetitive or complex activities**
- **Note time-consuming decision points**

### Step 2: AI Integration Opportunities
- **Information gathering** - Research, documentation review
- **Analysis and synthesis** - Code review, architecture evaluation
- **Creative generation** - Test cases, documentation, code snippets

---

## Real-World Integration Examples

### Bug Investigation Workflow

**Before:**
1. Read bug report
2. Reproduce issue
3. Dig through code
4. Form hypothesis
5. Test and validate

---

## Real-World Integration (continued)

### Bug Investigation Workflow

**With AI:**
1. **AI analyzes** bug report for patterns
2. **AI suggests** likely code areas to examine
3. **Collaborate** on hypothesis formation
4. **AI helps design** targeted tests

---

## Architecture Review Workflow

**Traditional Approach:**
- Solo analysis of design documents
- Manual identification of issues
- Experience-based recommendations

---

## Architecture Review Workflow (continued)

**AI-Enhanced Approach:**
- **AI pattern matching** against architectural anti-patterns
- **Collaborative exploration** of alternatives
- **Systematic risk assessment** with AI assistance
- **Iterative refinement** of designs

---

## Daily Integration Patterns

```
1.  Morning Planning
    - "Help me prioritize today's tasks:
    - [Task list with context]
    - Consider: Impact, dependencies, team blockers"
1. Code Review Prep
    - "I'm about to review a [COMPONENT] change.
    - What should I focus on for this type of modification?"

1. Problem Solving
    - "I'm debugging [ISSUE]. Here's what I know: [CONTEXT]
    - What investigation paths should I explore?"
```

---

## Team Adoption Strategy

### Individual Level
- **Start small** - Pick one workflow to enhance
- **Measure impact** - Time saved, quality improved
- **Build confidence** - Success breeds adoption

### Team Level
- **Share successes** - Demo effective AI workflows
- **Create standards** - Shared gems and approaches
- **Skill development** - Prompt engineering as core skill

---

## Measuring Success

### Quantitative Metrics
- **Time to resolution** - Bugs, code reviews, decisions
- **Quality indicators** - Fewer regressions, better designs
- **Team velocity** - Feature delivery, technical debt reduction

### Qualitative Indicators
- **Confidence in decisions** - Better-informed choices
- **Learning acceleration** - Faster onboarding, skill development
- **Job satisfaction** - More strategic work, less tedium

---

<!-- _class: section -->
# Q&A and Wrap-up
## Key Takeaways and Next Steps

---

## Key Takeaways

### 1. AI is a Collaboration Tool
- **Not** a replacement for engineering judgment
- **Yes** an amplifier for existing skills
- Success requires **iterative, conversational** approach

### 2. "Holding It Right" Matters
- **Multi-step workflows** beat single commands
- **Context and iteration** drive quality results
- **Domain expertise** remains essential

---

## Questions and Discussion

**Remember: AI is most powerful when you treat it as a collaborative partner, not a magic wand.**

---

## Advanced Workflow Examples

### Security Review Process
1. **AI scans** for common vulnerability patterns
2. **Human reviews** business logic and access controls
3. **Collaborative assessment** of attack vectors
4. **AI generates** security test scenarios
5. **Human validates** and prioritizes remediation

---

### Performance Optimization
1. **AI analyzes** code for performance anti-patterns
2. **Human provides** usage context and constraints
3. **Collaborative exploration** of optimization strategies
4. **AI suggests** profiling and measurement approaches
5. **Iterative refinement** of solutions

---

## Troubleshooting Common Issues

### "AI Responses Are Too Generic"
- **Add more context** - Specific tech stack, constraints, requirements
- **Use iterative prompting** - Build understanding step by step
- **Create domain-specific gems** - Capture your specific context

---

### "Results Aren't Reliable"
- **Validate AI suggestions** with human expertise
- **Use AI for exploration** not final decisions
- **Cross-reference** with documentation and best practices

---

### "Takes Too Much Time"
- **Invest in gem creation** - Upfront work pays off
- **Focus on high-impact workflows** - Code review, architecture, debugging
- **Share gems with team** - Collaborative efficiency gains

---

## Key Takeaways (continued)

### 3. Custom Prompts (Gems) Are Your Superpower
- **Consistency** in analysis and decision-making
- **Efficiency** through reusable workflows
- **Team alignment** through shared approaches

### 4. Start Small, Scale Gradually
- **Pick one workflow** to enhance first
- **Measure and iterate** based on results
- **Share successes** to drive team adoption


---

<!-- _class: outro -->
# Thank You!

