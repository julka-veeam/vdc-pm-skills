---
name: pm-brainstorming
description: "Use BEFORE any product strategy work — defining features, scoping workloads, designing product concepts, evaluating market opportunities, or making product decisions. Explores user intent, requirements, market context, and strategic options before committing to a direction. Adapted for Product Managers at Veeam Data Cloud working on SaaS backup/protection products."
---

# Product Strategy Brainstorming

Help turn product ideas into fully formed strategies and specs through structured collaborative dialogue. Adapted from obra/superpowers brainstorming for Product Management context.

Start by understanding the strategic context, then ask questions one at a time to refine the idea. Once you understand what you're building, present the strategy and get user approval.

**HARD GATE**: Do NOT produce deliverables (PRDs, strategy docs, roadmaps, presentations) until you have presented a strategic direction and the user has approved it. This applies to EVERY product decision regardless of perceived simplicity.

## Anti-Pattern: "This Is Too Simple To Need A Strategy Discussion"

Every product decision goes through this process. A single feature, a pricing change, a new workload connector, a competitive response — all of them. "Simple" decisions are where unexamined assumptions cause the most wasted effort. The strategy can be short (a few sentences for truly simple decisions), but you MUST present it and get approval.

## Process

### 1. Explore Context
Before asking detailed questions:
- What is the product area? (SaaS backup, identity protection, DevOps protection, collaboration, etc.)
- What triggered this work? (customer request, competitive pressure, compliance requirement, strategic initiative)
- What existing work exists? (prior PRDs, research, competitive analysis, user research)
- What constraints exist? (timeline, engineering capacity, platform limitations, dependencies)

### 2. Ask Clarifying Questions (one at a time)
- Prefer multiple choice when possible
- Only one question per message
- Focus on: target user, problem severity, competitive landscape, technical feasibility, business value
- If the scope is too large (multiple independent workloads or product areas), flag immediately and help decompose

### 3. Propose 2-3 Strategic Approaches
For each approach, cover:
- **What we'd build**: Scope and capabilities
- **For whom**: Target persona and segment
- **Why it wins**: Differentiation vs competitors
- **Risks**: Technical, market, and execution risks
- **Effort estimate**: Relative sizing (S/M/L/XL)
- **Your recommendation**: Lead with the recommended option and explain why

### 4. Present the Strategy
Once you understand what you're building, present the strategy in sections:
- **Problem statement**: Who has the pain, how severe, how frequent
- **Target user**: Primary persona with context
- **Proposed solution**: What we're building and why
- **Competitive positioning**: How this positions against competitors
- **Success metrics**: How we'll measure success
- **Scope**: MVP vs V1 vs future
- **Key risks**: What could go wrong

Ask after each section whether it looks right. Be ready to revise.

### 5. Document the Strategy
Save the validated strategy to a document:
- Use the `docx` skill for formal strategy documents
- Use the `pptx` skill for executive presentations
- Or save as markdown for quick reference

### 6. Transition to Next Step
After strategy approval, offer next steps:
- **PRD writing**: Detailed product requirements
- **Competitive deep-dive**: Using `saas-competitive-intel` skill
- **Technical research**: Using `saas-platform-researcher` skill
- **User research**: Using `saas-backup-user-researcher` skill
- **Pricing analysis**: Using `pricing-strategy` skill
- **Executive presentation**: Using `pptx` skill

## Veeam Data Cloud Context

When brainstorming for Veeam, always consider:
- **Shared responsibility model**: What does the SaaS vendor protect vs what is customer responsibility?
- **Backup-through-restore**: Don't just think about backup — think about the full restore workflow
- **Irrecoverability question**: What data/config is permanently lost if not backed up?
- **Blast radius**: If this data is lost, what breaks downstream?
- **Regulatory drivers**: DORA, NIS2, SOC 2, ISO 27001 — which apply to this workload?
- **Competitive landscape**: Who else protects this workload? What do they do well/poorly?
- **Securiti AI integration**: Where does DSPM/governance/privacy add differentiated value?
- **Platform consolidation**: How does this fit into VDC's multi-workload story?

## Key Principles

- **One question at a time** — Don't overwhelm with multiple questions
- **Multiple choice preferred** — Easier to decide than open-ended
- **Challenge assumptions** — "Is this really the right workload to prioritize next?"
- **Explore alternatives** — Always propose 2-3 approaches before settling
- **YAGNI ruthlessly** — Remove scope that doesn't serve the core value proposition
- **Incremental validation** — Present strategy, get approval before producing deliverables
- **Evidence-based** — Every claim about market/competitors/users must be verifiable
