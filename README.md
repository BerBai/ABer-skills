# ABer-skills

Personal agent-skills collection by **Jason Pai** ([@BerBai](https://github.com/BerBai)，鳄鱼儿）。

Self-developed, self-used, shipped one at a time.

## What this is

A small, curated shelf of [Agent Skills](https://agentskills.io) — folders of instructions and resources that coding agents (Claude Code, Codex CLI, Cursor, …) load dynamically to perform specialized tasks. Every skill published here is written and maintained by the author, exercised in real workflows before release, and works standalone — no framework to buy into.

## Positioning

Most skill libraries are either official demonstration sets ([anthropics/skills](https://github.com/anthropics/skills)) or complete engineering methodologies built as interlocking frameworks ([obra/superpowers](https://github.com/obra/superpowers)). This repo takes the opposite bet: a personal shelf, not a framework. Only skills the author actually uses get published — no filler, no vendored third-party skills. Skills ship one at a time, when they are ready; an empty table below means the first batch is still being curated, not that the project is idle.

大部分技能库要么是官方示例集，要么是成套的工程方法论框架。这个仓库走另一条路：一面个人书架，而不是一套框架。只上架作者本人日常在用、亲手维护的技能——不凑数、不搬运第三方。技能一个一个上，准备好才上；下表为空表示首批还在打磨，不代表弃坑。

## Skills

_None yet — the first batch is being curated._

When a skill lands, this table is generated verbatim from the `name` and `description` fields of its `SKILL.md` frontmatter — never hand-written, never invented.

## Install

Clone the repo:

```bash
git clone https://github.com/BerBai/ABer-skills.git
```

Then copy the skills you want into your agent's skills directory:

```bash
cp -r ABer-skills/skills/<skill-name>/ ~/.claude/skills/
```

| Agent | Skills directory |
|---|---|
| Claude Code | `~/.claude/skills/` |
| Codex CLI | `~/.codex/skills/` |
| Cross-agent (many tools) | `~/.agents/skills/` |

## Usage

Skills trigger on natural language. Once a skill is installed, just describe the task in the agent chat — the agent loads the matching skill automatically based on its description. No slash commands, no configuration.

## Layout

```text
skills/
└── <skill-name>/
    ├── SKILL.md      # frontmatter (name, description) + instructions
    └── …             # optional references/, scripts/, assets/
```

Every `SKILL.md` follows the [Agent Skills](https://agentskills.io) convention: a lowercase-hyphen `name`, and a `description` that states what the skill does and when to use it.

## Also by this author

- [devops-skills](https://github.com/BerBai/devops-skills) — DevOps & cross-device debugging marketplace, 8 Claude Code plugins
- [sheke-bid](https://github.com/BerBai/sheke-bid) — 国社科及中文社科课题申报工作流 skill

## License

[Apache-2.0](LICENSE) © 2026 Jason Pai
