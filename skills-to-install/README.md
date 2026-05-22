# Skills to install

Two skill folders are dropped here so you can install them into Cowork persistently. The `.claude/skills` directory is read-only from my sandbox, so I can't install them directly — you'll want to do this through Cowork's skill UI (or via your local dotfiles if you sync them).

## What's here

### `frontend-design/SKILL.md`
- **Source:** https://github.com/anthropics/skills/tree/main/skills/frontend-design
- **Provenance:** Official Anthropic (Apache 2.0)
- **What it does:** Forces a bold, production-grade aesthetic direction. Forbids generic AI-style design (Inter/Roboto, purple-on-white gradients, cookie-cutter component layouts). Encourages distinctive typography, intentional motion, and unexpected spatial composition.

### `product-self-knowledge/SKILL.md`
- **Source:** https://github.com/unicorn-plugins/claude-skills/tree/main/skills/product-self-knowledge
- **Provenance:** Third-party (`unicorn-plugins/claude-skills`, MIT) — NOT canonical Anthropic. The Anthropic public `skills` repo does not currently publish a `product-self-knowledge` skill, so this is the closest available analog.
- **What it does:** A short Korean-language routing skill. Says: differentiate Claude.ai vs. Claude Code vs. Claude API; always cite official URLs (docs.claude.com, support.claude.com); verify against docs rather than rely on training data. No material product facts — it's methodology, not a fact sheet.
- **Caveat:** Treat it as a guardrail, not as ground truth. Continue verifying any product claim against the official Anthropic docs / news pages.

## Session note

For the current session I've already read both `SKILL.md` files into context and will apply their guidance directly while building. Installing them into Cowork will make that automatic in future sessions.
