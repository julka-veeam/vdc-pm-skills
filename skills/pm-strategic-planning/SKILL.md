---
name: pm-strategic-planning
description: "Use when you have a strategy or product concept approved and need to create a detailed execution plan — PRD structure, phased roadmap, workstream breakdown, or go-to-market plan. Produces structured plans that can be handed to engineering, design, marketing, or leadership. Adapted for Product Managers at Veeam Data Cloud."
---

# Strategic Planning for Product Managers

Write comprehensive product execution plans assuming the reader has minimal context about the workload, market, or technical constraints. Document everything needed: what to build in each phase, dependencies, success criteria, risks, and validation steps. Adapted from obra/superpowers writing-plans for Product Management.

**Announce at start:** "I'm using the pm-strategic-planning skill to create the execution plan."

## Scope Check

If the strategy covers multiple independent workloads or product areas, it should have been broken into sub-strategies during brainstorming. If it wasn't, suggest breaking this into separate plans — one per workload or product area. Each plan should deliver clear value on its own.

## Plan Types

### Type 1 — Product Roadmap Plan
For phased product delivery:

```markdown
# [Product/Feature] Roadmap Plan
**Date** | **Author** | **Status**: Draft / Review / Final

## Goal
[One sentence: what this delivers and why it matters]

## Context
[2-3 sentences: market driver, customer need, competitive pressure]

## Phase Structure
### Phase 1: MVP (minimum credible product)
- What's included and why
- Target user scenario
- Success criteria
- Dependencies
- Estimated relative effort

### Phase 2: V1 (first paying customers)
- Additional capabilities
- What customer feedback determines scope
- Success criteria

### Phase 3: Growth (scale and differentiate)
- Differentiating features
- Platform integration depth
- Competitive moats

## Key Decisions Required
[Decisions that block progress — with options and recommendation]

## Risks & Mitigations
[Top 5 risks with mitigation plans]

## Open Questions
[What must be validated before committing]
```

### Type 2 — PRD Execution Plan
For engineering handoff:

```markdown
# [Feature] PRD Execution Plan

## Problem Statement
- Who has the pain
- How severe / how frequent
- Current workaround

## Solution Overview
- What we're building
- Architecture approach
- Key technical decisions

## Workstreams
### Workstream 1: [Name]
- Scope: what's included
- Dependencies: what must exist first
- Acceptance criteria: how we know it's done
- Estimated effort: relative (S/M/L/XL)

### Workstream 2: [Name]
[Same structure]

## User Stories Summary
[High-level story list — detailed stories via jira-story-architect skill]

## Non-Functional Requirements
- Performance targets
- Security requirements
- Compliance requirements
- Scalability expectations

## Go/No-Go Criteria
[What must be true before launch]
```

### Type 3 — GTM Execution Plan
For go-to-market:

```markdown
# [Product] Go-to-Market Plan

## Positioning
- For [target user] who [problem], [product] is [category] that [key benefit]
- Unlike [alternatives], [product] [differentiation]

## Launch Phases
### Phase 1: Private Preview
- Target customers, success criteria, feedback loops

### Phase 2: Public Preview
- Enablement, documentation, pricing validation

### Phase 3: General Availability
- Full launch, marketing, sales enablement

## Messaging Framework
- Primary message
- Supporting messages (by persona)
- Competitive responses

## Sales Enablement
- Battlecards needed
- Demo scenarios
- Pricing guidance

## Success Metrics
- Leading indicators (first 30 days)
- Lagging indicators (first 90 days)
```

## Veeam Data Cloud Planning Context

When planning for VDC, always include:

**Technical planning considerations:**
- API rate limits and backup frequency constraints
- Data model complexity (what objects, what relationships, what breaks during restore)
- Restore dependency ordering (groups before memberships, apps before assignments)
- Incremental backup strategy (change detection method)
- Storage architecture (Veeam-managed vs BYOS)

**Product planning considerations:**
- How this workload fits into VDC packaging (standalone vs bundle)
- Pricing model alignment with existing VDC pricing
- Shared UI patterns with existing VDC workloads
- Cross-workload features (unified dashboard, alerts, compliance reporting)
- Securiti AI integration touchpoints

**Competitive planning considerations:**
- What competitors offer for this workload today
- Where Veeam can differentiate (restore fidelity, coverage depth, platform consolidation)
- Time-to-market pressure (who's launching what, when)

## Plan Quality Standards

Every plan must be:
- **Decision-useful**: A reader can make decisions based on this plan
- **Actionable**: Each phase/workstream has clear scope and criteria
- **Honest about unknowns**: Open questions are explicit, not hidden
- **Prioritized**: Must-have vs nice-to-have is clear
- **Measurable**: Success criteria are specific, not vague

## After the Plan

Offer next steps:
1. **Engineering handoff** — Create detailed user stories using `jira-story-architect` or `user-story-architect` skills
2. **Executive presentation** — Create deck using `pptx` skill
3. **Competitive validation** — Deep-dive using `saas-competitive-intel` skill
4. **Technical validation** — Platform research using `saas-platform-researcher` skill
5. **Formal document** — Create Word doc using `docx` skill
