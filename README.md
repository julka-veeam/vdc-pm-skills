# VDC Product Management AI Skills

25 AI agent skills for Product Management at Veeam Data Cloud. Works with Warp (Oz), Claude Code, Claude Desktop, Cursor, and any agent that supports SKILL.md format.

## Installation

### Warp (Oz Agent)
Copy skills to `~/.agents/skills/`:
```bash
git clone https://github.com/julka-veeam/vdc-pm-skills.git
cp -r vdc-pm-skills/skills/* ~/.agents/skills/
```

### Claude Code
Copy skills to `~/.claude/skills/`:
```bash
git clone https://github.com/julka-veeam/vdc-pm-skills.git
cp -r vdc-pm-skills/skills/* ~/.claude/skills/
```

### Claude Desktop
Open each `SKILL.md` file, copy contents (without `---` frontmatter), and paste as Custom Instructions in a Claude Project.

### npx (skills.sh compatible)
```bash
npx skills add https://github.com/julka-veeam/vdc-pm-skills --skill <skill-name>
```

## Skills

### Strategy & Leadership
| Skill | Description |
|---|---|
| `vp-saas-data-protection` | Technical VP of Product for SaaS workload backup strategy |
| `veeam-devops-strategist` | VP of Strategy for DevOps platform backup (GTM, positioning, pricing) |
| `veeam-devops-pm` | VP-level PM for DevOps backup product strategy |
| `cto-tech-strategist` | CTO & Chief Architect for technical blueprints and ADRs |
| `ciso-compliance-reviewer` | CISO compliance SME — reviews docs against DORA, NIS2, GDPR, SOC 2, ISO 27001 |

### Research & Intelligence
| Skill | Description |
|---|---|
| `saas-competitive-intel` | Competitive intelligence for SaaS backup markets (feature matrices, battlecards) |
| `saas-platform-researcher` | Technical researcher for SaaS APIs, data models, rate limits, edge cases |
| `saas-backup-user-researcher` | User researcher for backup personas, journeys, JTBD |
| `devops-backup-persona` | DevOps admin + developer persona expert (GitHub, GitLab, Azure DevOps) |

### Product Planning
| Skill | Description |
|---|---|
| `pm-brainstorming` | Product strategy brainstorming with Veeam context |
| `pm-strategic-planning` | Roadmap, PRD, and GTM execution planning |
| `pricing-strategy` | SaaS pricing, packaging, and monetization strategy |
| `user-story-architect` | Implementation-ready user stories with edge-case coverage |
| `jira-story-architect` | Confluence → Jira story decomposition |

### Engineering
| Skill | Description |
|---|---|
| `principal-fullstack-dev` | CTO-level engineering standards for production code |
| `principal-frontend-ux` | Veeam UI/UX with React, Tailwind, shadcn/ui |
| `frontend-design` | Creative, distinctive frontend design (Anthropic official) |

### Document Creation
| Skill | Description |
|---|---|
| `docx` | Word document creation and editing (Anthropic official) |
| `pptx` | PowerPoint presentations (Anthropic official) |
| `xlsx` | Excel spreadsheets and data analysis (Anthropic official) |
| `pdf` | PDF processing, extraction, merging (Anthropic official) |
| `doc-coauthoring` | Collaborative document writing workflow (Anthropic official) |

### AI & Prompting
| Skill | Description |
|---|---|
| `llm-instruction-designer` | System prompt / instruction design for any LLM |
| `prompt-engineer` | Prompt crafting, debugging, and optimization |

### Integrations
| Skill | Description |
|---|---|
| `dcc-workflow-builder` | Securiti AI Data Command Center workflow builder |
