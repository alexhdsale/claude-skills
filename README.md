# Claude Code Skills — Curated Index

Personal index of Claude Code skill collections I use, with upstream links and quick "when to use" notes.

This repo is **a map, not a mirror.** Skills themselves stay at their upstream repos — install them locally with `git clone` into `~/.claude/skills/` (Mac/Linux) or `%USERPROFILE%\.claude\skills\` (Windows). All credit and license obligations belong to the upstream authors.

---

## Installed locally — 441 skills across 5 bundles

| Bundle | Skills | Focus | Upstream |
|---|---:|---|---|
| **alirezarezvani/claude-skills** | 229 | General purpose: engineering, marketing, c-level advisory, finance, product, QA, DevOps, security | [github](https://github.com/alirezarezvani/claude-skills) (5.2k ⭐) |
| **JoelLewis/finance_skills** | 84 | Financial advisory, client ops, compliance, trading ops, wealth management, data integration | [github](https://github.com/JoelLewis/finance_skills) |
| **tradermonty/claude-trading-skills** | 71 | Stock trading: backtesting, screeners (CANSLIM, Finviz), earnings, FTD detection, exposure | [github](https://github.com/tradermonty/claude-trading-skills) |
| **anthropics/financial-services-plugins** | 56 | Anthropic-official: equity research, financial analysis, IB, PE, wealth management | [github](https://github.com/anthropics/financial-services-plugins) |
| **teng-lin/notebooklm-py** | 1 | NotebookLM API — create notebooks, generate podcasts/mind maps, full programmatic access | [github](https://github.com/teng-lin/notebooklm-py) |

Plus `quant-sentiment-ai/claude-equity-research` (slash-commands, not SKILL.md format) — 9 commands for equity research workflows.

---

## Recommended to add

These are top-tier collections I haven't installed yet but should:

| Repo | Stars | Why |
|---|---:|---|
| [`anthropics/skills`](https://github.com/anthropics/skills) | official | **The official Anthropic repo** — 17 production-quality skills (docx/pdf/xlsx/pptx, MCP dev, web testing, etc). Power Claude.ai's document features. |
| [`obvious-incantations/Superpowers`](https://github.com/obvious-incantations/Superpowers) | ~94k | Anthropic-accepted marketplace skill. Enforces a 7-phase workflow: Brainstorm → Spec → Plan → TDD → Subagent → Review → Finalize. |
| [`VoltAgent/awesome-agent-skills`](https://github.com/VoltAgent/awesome-agent-skills) | curated | 1000+ agent skills, multi-tool (Claude Code, Codex, Gemini CLI, Cursor). |
| [`travisvn/awesome-claude-skills`](https://github.com/travisvn/awesome-claude-skills) | curated | Quality "awesome list" of community skills. |

---

## Install pattern

```bash
cd ~/.claude/skills/    # or %USERPROFILE%\.claude\skills on Windows
git clone https://github.com/<owner>/<repo>.git
```

After cloning, Claude Code auto-discovers SKILL.md files on next session. Verify with `/skills` (or watch the system reminder for available skills).

---

## Bundle details (when to reach for which)

### alirezarezvani/claude-skills (229 skills)
Broadest collection. Covers:
- **engineering / engineering-team**: a11y-audit, aws/gcp/azure architects, security-pen-testing, terraform-patterns, senior-frontend/backend/qa, secrets-vault-manager
- **business-growth, marketing-skill**: SEO, ad-creative, A/B testing, content strategy
- **c-level-advisor, ra-qm-team**: regulatory, quality management, exec advisory
- **product-team, project-management**: agile, PM frameworks
- **finance, custom-gpt, orchestration, agents**

Use when: you need a generalist skill not specific to trading/finance.

### tradermonty/claude-trading-skills (71 skills)
Trading-specific deep stack. Notable:
- `backtest-expert`, `walk-forward-backtest`
- Screeners: `canslim-screener`, `finviz-screener`, `dividend-growth-pullback-screener`
- `earnings-trade-analyzer`, `earnings-calendar`, `economic-calendar-fetcher`
- `edge-*` family (8 skills) for systematic strategy R&D
- `ftd-detector`, `breadth-chart-analyst`, `exposure-coach`

Use when: equity trading research, strategy design, backtesting.

### JoelLewis/finance_skills (84 skills)
Wealth-management & advisory bias. Plugin groups: advisory-practice, client-operations, compliance, core, data-integration, trading-operations, wealth-management.

Use when: client-facing financial advisory work, compliance.

### anthropics/financial-services-plugins (56 skills)
Anthropic-built, deal-team focused: equity-research, financial-analysis, investment-banking, private-equity, wealth-management, claude-in-office. Highest quality bar.

Use when: institutional finance workflows, want Anthropic-quality.

### teng-lin/notebooklm-py
Single skill, but unlocks the full NotebookLM API beyond the web UI — programmatic notebook creation, source upload (URLs, YouTube, PDFs, audio, video), all artifact types (podcasts, mind maps, briefings, FAQs), download in multiple formats.

Use when: building a knowledge base from many sources, generating podcasts/briefings.

---

## License

This repo's index content (this README) is MIT. Each upstream skill bundle has its own license — see the upstream repo.
