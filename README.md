# Hi, I'm Tony 👋

I build small open-source tools that remove real, daily friction for [Claude Code](https://code.claude.com) users.

The way they get built matters more than any single repo: I run a continuous loop — **study open-source repos and AI tooling → validate what actually works against my own heavy, multi-session workflow → fold the verified lessons into a continuously improving engineering system → publish the reusable parts as tools anyone can use.** House rule: every lesson must end up as a file, a test, or a tool — if it only lives in a chat, it doesn't exist.

When Claude Code ships a new capability, my default pattern is: try it against real work, find the friction, publish the tool that removes it. usage-guard's real-quota mode exists because Claude Code started exposing `rate_limits` to status lines — the capability appeared, and the tool followed.

## Claude Code tools I maintain

| Tool | The daily friction it removes |
|---|---|
| [usage-guard](https://github.com/eltonylfgi-blip/claude-code-usage-guard) | Getting cut off mid-task by the 5-hour/weekly plan quota — warns you in-session, *before* it happens, with real `rate_limits` numbers |
| [claude-session-triage](https://github.com/eltonylfgi-blip/claude-session-triage) | 15 chats open across projects, 3 waiting on you — which 3? One triage panel of every idle session and what it was waiting on |
| [claude-usage-pacer](https://github.com/eltonylfgi-blip/claude-usage-pacer) | Burning the weekly quota before the reset — a single-file, local-first pacing app |

All built under the same six constraints — local-first, zero deps, fail-open, warn-don't-block, honest READMEs, one real friction per tool: **[ENGINEERING_PRINCIPLES.md](https://github.com/eltonylfgi-blip/claude-code-usage-guard/blob/main/ENGINEERING_PRINCIPLES.md)**, each with where it's implemented. Both plugins are submitted to [awesome-claude-plugins](https://github.com/ComposioHQ/awesome-claude-plugins/pulls?q=is%3Apr+author%3Aeltonylfgi-blip).

## Currently exploring

Direction, not promises — this is where the workflow is pointed right now:

- **Hardening usage-guard's real-quota capture** across real-world setups (OS × plan × status-line configs) — top of the [public roadmap](https://github.com/eltonylfgi-blip/claude-code-usage-guard/blob/main/ROADMAP.md); each field report becomes a fixture and a test.
- **Lower-friction installs** — publishing session-triage to npm so `npx claude-session-triage` works without the `github:` prefix.
- **Distribution** — landing the suite in community lists and marketplaces (PRs already open).
- **Whatever friction surfaces next** — the workflow keeps finding it; I ship weekly.

## Other tooling

- [tikslide](https://github.com/eltonylfgi-blip/tikslide) — read a TikTok photo slideshow (carousel) as clean, per-slide Markdown. Built because my content-absorption pipeline needed it; published because nothing else did exactly this.

## Learning in public

- [madre-arquitectura](https://github.com/eltonylfgi-blip/madre-arquitectura) — the architecture and *open pain points* of the engineering system behind all of the above (in Spanish, with an English TL;DR). I publish the problems, not just the wins, to collect feedback and repo recommendations via Issues.

---

These projects stay open source either way. If you use Claude Code and one of these removes a papercut for you — that's the whole point. Issues and PRs welcome, in English or Spanish.
