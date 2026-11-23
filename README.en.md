# xingtu-bot · Bot Form Factor Case Notes

> Under local construction, not published yet. This repo covers publicly verifiable Bot projects and form-factor breakdowns; it is not the official repo of any Bot product.

[![License: MIT](https://img.shields.io/badge/License-MIT-orange.svg)](./LICENSE) ![Status](https://img.shields.io/badge/status-local-lightgrey)

## In one line

A breakdown of the "Bot form factor" — persistent memory, multiple specialized Bots, group chat handoffs, and chat-channel integrations — focused on engineering trade-offs rather than product reviews or rankings.

## Inspiration and boundaries

Grok Bot turned "a team of named Bots with their own computers that work on schedule" into a paid product. The open-source community then produced several alternative routes. This repo cares about the engineering trade-offs behind these forms, not about endorsing any of them:

- How multi-Bot memory persists, and where the limits are.
- Who speaks first in a group chat and who stays silent, to save tokens.
- How Bots call coding agents already installed on the machine instead of rebuilding a model.
- Where data lives, and who bears the cost.

## Boundaries with neighboring repos

| Repo | Covers | Does not cover |
|---|---|---|
| `xingtu-super-agent` | Control plane and protocol design for cross-agent collaboration | Does not break down individual Bot products |
| **xingtu-bot** (this repo) | Public case breakdowns and mechanism notes for Bot forms | Not a methodology flagship or a skill library |
| `teamai-harness` | Team AI configuration SSoT (skills/rules/agents assembly) | Does not record external open-source Bot cases |

## Core content

- **Form comparison**: mechanisms such as persistent memory, chief-Bot coordination, `[PASS]` silence, and channel integration, compared side by side.
- **Case cards**: one card per public project, with author, license, install form, cost structure, and check date.
- **Trade-off notes**: why a design was chosen, its cost, and when it stops holding.

## Home and Navigation

This repo belongs to the case-study section of the [XingTu open-source matrix](https://github.com/xingtu1996) and is maintained independently. The [profile repo](https://github.com/xingtu1996) only indexes; it does not duplicate this repo's content.

The four case repos divide by boundary and cross-reference each other:

- [xingtu-testting](https://github.com/xingtu1996/xingtu-testting) - AI testing
- [xingtu-bot](https://github.com/xingtu1996/xingtu-bot) - Bot form factors
- [xingtu-agent](https://github.com/xingtu1996/xingtu-agent) - Agent deployment
- [xingtu-bci](https://github.com/xingtu1996/xingtu-bci) - Collaboration bad cases

## Quick start

```bash
git clone <repo-url> xingtu-bot
cd xingtu-bot
# Template: cases/_TEMPLATE.md; collected public cases: cases/public/
```

Before adding a case, read `cases/_TEMPLATE.md`. Public cases are always `public-source` with a source link and check date. Only cases installed and tested locally may be marked `verified`.

## Case status labels

| Label | Meaning |
|---|---|
| `design` | Design or idea only, not verified |
| `public-source` | Compiled from public material, not tested here; needs link and check date |
| `verified` | Run locally with reproducible evidence |
| `production` | In production use |

## Contribution rules

- Only publicly verifiable projects. Never present public demos as hands-on tests, and never invent efficiency numbers.
- Keep similarly named but distinct projects separate, with install package name and license, to avoid confusion.
- Prices and star counts go stale: record the check date and defer to official pages; do not use them as long-term criteria.
- De-identify every case: no client names, personal names, internal domains, or internal platform paths.

## License

[MIT](./LICENSE) · 行途 XingTu

## Author

行途 XingTu (engineering byline) · WeChat: 行途技术手记
