# linear-ui-performance

**Agent Skill** for Cursor, Claude Code, Codex, and other compatible AI coding agents.

Encodes the technical performance architecture and best practices from Linear.app's "How is Linear so fast?" breakdown. Makes your AI agent an expert at building lightning-fast, native-feeling web UIs — especially data-heavy SaaS tools like issue trackers, project management, dashboards, tables, and real-time collaborative interfaces.

## Installation (one command)

```bash
npx skills add getlabs/linear-ui-performance
```

Or for a specific agent:

```bash
npx skills add getlabs/linear-ui-performance --agent cursor
```

After installation, the skill appears in Cursor under **Settings → Rules → Skills** (or equivalent in other agents). The agent will automatically activate it when relevant (performance, UI lists, state management, data fetching, etc.) or you can invoke it explicitly with `/linear-ui-performance`.

Browse all skills: https://skills.sh/

## What this skill teaches the agent

- Local-first architecture (IndexedDB as primary store + in-memory observable hydration)
- True optimistic updates with local apply + async background sync (no spinners)
- Granular reactivity (MobX-style per-property observables → cell-level re-renders only)
- Advanced bundling & loading (per-package chunks, modulepreload, service worker precache, inlined app shell)
- Virtualization + fine-grained updates for large lists/tables
- Real-time collab patterns (Yjs + ProseMirror)
- Animation, keyboard-first, and perceived performance principles
- Concrete config examples (Vite/Rolldown, etc.)
- Stack-specific guidance (React/Next.js, Angular, general)

## How to publish / update this skill yourself

1. Create a new public GitHub repository (recommended name: `linear-ui-performance`)
2. Copy the contents of this folder into the repo root (especially `SKILL.md`)
3. Commit and push
4. Install from your repo: `npx skills add getlabs/linear-ui-performance`
5. (Optional) Add a `.skills.json` lockfile in projects for reproducible team installs

The skill uses the open **Agent Skills** standard (SKILL.md + YAML frontmatter). It works across Cursor, Claude Code, and many other agents without modification.

## Source

Based on the excellent technical breakdown at:
https://performance.dev/how-is-linear-so-fast-a-technical-breakdown

All credit for the original research and Linear's engineering team.

## License

MIT — feel free to fork, improve, and share.

---

**Pro tip**: Combine this skill with other performance or frontend skills for even stronger results (e.g. React best practices, virtualization libraries, etc.).