# G2 Claude Guide

Interactive field guide to Anthropic's four products — Claude Chat, Cowork, Code, and Design — built for G2 teammates. A 3-step wizard personalizes the guide by role: Designer, Product Manager, Engineer, Leadership, UX Researcher, Operator, or Curious.

## View it

- **Live:** `https://lsanchez-g2.github.io/g2-claude-guide/` *(once Pages is enabled — see Deploy below)*
- **Local:** open `index.html` in any modern browser. No build step, no dependencies beyond Google Fonts.

## What's inside

- **Single-file HTML** — no framework, no build, no bundler. ~240 KB.
- **Wizard with 7 roles** that personalizes:
  - Product priority (which Claude to start with)
  - Three example prompts that match your work
  - The playbook to run end-to-end first
  - Top 10 skills to install (mandatory items highlighted in ember)
- **4 product sections** — each with an animated demo: chat-to-Artifact, Cowork folder-reorganize, Claude Code terminal session, Claude Design canvas + handoff bundle.
- **3 cross-product playbooks** — Spec → Ship, Inbox → Insight, Repo → Refactor.
- **Full accessibility** — `prefers-reduced-motion`, keyboard navigation, focus rings, skip-to-content, ARIA live regions.

## Need access?

Use the **G2 Assist Slackbot**. If it doesn't work, ping **@Johnny Trieu**.

## Skills bundled

The `skills-to-install/` folder ships two `SKILL.md` files you can install into Cowork:

- `frontend-design` — Anthropic official (Apache 2.0).
- `product-self-knowledge` — third-party (MIT), routing methodology.

The custom **ds-architect** skill referenced in the guide lives at [github.com/lsanchez-g2/ds-architect](https://github.com/lsanchez-g2/ds-architect) — mandatory for designers.

## Deploy (GitHub Pages)

After pushing the repo:

1. Go to **Settings → Pages** in the repo on GitHub.
2. Source: **Deploy from a branch**.
3. Branch: **main**, folder: **/ (root)**.
4. Save. Pages will publish at `https://lsanchez-g2.github.io/g2-claude-guide/` within ~60 seconds.

Or via the GitHub CLI:

```bash
gh api repos/lsanchez-g2/g2-claude-guide/pages \
  -X POST \
  -F source[branch]=main \
  -F source[path]=/
```

## Editing

The whole experience lives in one file: `index.html`. Sections you'll touch most:

- **`ROLES` object** — the wizard's role catalog (questions per role).
- **`recommend()` function** — the per-role recommendation engine (products, prompts, playbook, fold).
- **`SKILLS` catalog** — what each skill is, its source, its URL.
- **`SKILLS_BY_ROLE`** — the top-10 list per role (with `mandatory: true` for required items).

All are at the top of the wizard script block (search for `WIZARD — first-visit personalization`).

---

Lex Sánchez · G2 · Product Builder — 2026
