# 🧠 persona-vault

A curated collection of **AI personas for prompt engineering** — ready to copy-paste into agentic development tools and AI-assisted workflows.

## Why this exists

I (Sasha) spent way too much time researching AI personas online — digging through scattered blog posts, half-baked GitHub repos, and ChatGPT suggestions that missed the mark. I wanted a single place with well-crafted, detailed, opinionated personas that actually work when you drop them into an AI agent's system prompt.

So I built this. Every persona is designed to be copied verbatim into your tool of choice and used immediately — no tweaking required (though you absolutely should tweak them for your context).

## Where to use these

These personas are designed for **agentic SDLC tools** and **AI-assisted workflows**, including:

| Tool | Description |
|------|-------------|
| [Paperclip](https://paperclip.dev) | Agentic SDLC platform — drop personas into agent configurations |
| [Claude Code](https://docs.anthropic.com/en/docs/claude-code) | Use as `CLAUDE.md` files or in project instructions |
| [Pentagon.run](https://pentagon.run) | Agentic workflow orchestration (emerging) |
| [Cursor](https://cursor.sh) | AI code editor — use in `.cursorrules` or project context |
| [Windsurf](https://codeium.com/windsurf) | AI IDE — use in workspace rules |
| [Codex](https://openai.com/codex) | OpenAI's coding agent — use as system prompts |
| [Devin](https://devin.ai) | Autonomous AI engineer — configure agent personas |
| [GitHub Copilot Workspace](https://githubnext.com/projects/copilot-workspace) | Use in workspace context |
| Any LLM chat | Claude, ChatGPT, Gemini — paste as system prompt or first message |

## Repo structure

```
persona-vault/
├── README.md
├── personas/
│   ├── engineering/
│   │   ├── senior-software-engineer.md
│   │   ├── software-architect.md
│   │   ├── devops-platform-engineer.md
│   │   ├── site-reliability-engineer.md
│   │   ├── qa-test-engineer.md
│   │   ├── database-engineer.md
│   │   ├── security-engineer.md
│   │   ├── frontend-engineer.md
│   │   ├── data-engineer.md
│   │   ├── ml-engineer.md
│   │   ├── technical-writer.md
│   │   └── tech-lead.md
│   ├── product/
│   │   ├── product-manager.md
│   │   ├── ux-researcher.md
│   │   ├── ux-ui-designer.md
│   │   ├── product-analyst.md
│   │   └── scrum-master.md
│   ├── marketing/
│   │   ├── growth-marketer.md
│   │   ├── content-strategist.md
│   │   ├── copywriter.md
│   │   ├── seo-specialist.md
│   │   ├── performance-marketer.md
│   │   ├── brand-strategist.md
│   │   ├── community-manager.md
│   │   └── email-marketing-specialist.md
│   ├── strategy/
│   │   ├── value-chain-analyst.md
│   │   ├── business-strategist.md
│   │   ├── management-consultant.md
│   │   ├── financial-analyst.md
│   │   └── change-management-lead.md
│   ├── compliance-legal/
│   │   ├── compliance-officer.md
│   │   ├── data-privacy-gdpr-specialist.md
│   │   ├── legal-counsel.md
│   │   └── supply-chain-manager.md
│   ├── operations/
│   │   ├── operations-manager.md
│   │   └── procurement-manager.md
│   ├── people/
│   │   ├── hr-business-partner.md
│   │   ├── recruiter.md
│   │   ├── learning-development-specialist.md
│   │   └── executive-coach.md
│   ├── sales/
│   │   ├── sales-strategist.md
│   │   ├── customer-success-manager.md
│   │   ├── solutions-engineer.md
│   │   └── partnerships-manager.md
│   └── creative/
│       ├── product-designer.md
│       ├── visual-designer.md
│       ├── motion-designer.md
│       ├── creative-director.md
│       └── ux-ui-designer-with-prototyping.md
```

## How to use

1. **Browse** the `personas/` directory for the role you need.
2. **Copy** the entire contents of the `.md` file.
3. **Paste** into your tool's system prompt, agent configuration, or `CLAUDE.md`.
4. **Customise** for your specific context — add your tech stack, company conventions, project constraints.

## Persona structure

Every persona follows the same format:

- **Role introduction** — Who you are and what you believe
- **Core Principles** — The non-negotiable beliefs that guide behaviour
- **Environment & Preferences** — Tech stack, tools, conventions
- **Workflow** — How you approach work, step by step
- **Anti-Patterns** — Things you NEVER do (critical for keeping AI on track)
- **How You Communicate** — Tone, audience adaptation, default phrases
- **Expected Outputs** — What deliverables this persona produces

## Experimental: autonomous UI prototyping

The `creative/ux-ui-designer-with-prototyping.md` persona includes an experimental workflow for generating working HTML/CSS/JS prototypes autonomously using the **Gemini API** (no browser, no OAuth required).

The agent writes a structured design brief, calls `gemini-2.0-flash` via the Gemini API, and produces a self-contained HTML file that opens directly in the browser. No human intervention needed beyond providing a `GEMINI_API_KEY` environment variable.

> Google Stitch (stitch.withgoogle.com) is also documented in that persona for manual use — it requires Google account authentication and has no public API, so it is not suitable for agentic automation.

## Contributing

PRs welcome. If you have a persona that's battle-tested in your workflow, open a PR. Keep the same structure and level of detail.

## Inspiration

Inspired by [Liz Howard's](https://github.com/lizTheDeveloper) work on AI personas for engineering education, and by the broader community building agentic development tools.

## License

MIT — use these however you want.
