# linear-ui-performance

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/getlabs/linear-ui-performance/pulls)

**Agent Skill** that teaches AI coding agents how to build extremely fast, native-feeling web UIs — inspired by Linear.app’s architecture.

Makes your agent an expert in local-first patterns, optimistic updates, granular reactivity, and high-performance rendering.

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

## Example

After adding the skill, your agent will automatically apply these patterns when you ask things like:

- “Build a fast issue list with optimistic updates”
- “Create a high-performance dashboard with virtualized tables”
- “Implement local-first state management for this feature”
 
## Source

Based on the excellent technical breakdown at:
https://performance.dev/how-is-linear-so-fast-a-technical-breakdown

All credit for the original research and Linear's engineering team.

## License

MIT — feel free to fork, improve, and share.

---

**Pro tip**: Combine this skill with other performance or frontend skills for even stronger results (e.g. React best practices, virtualization libraries, etc.).
