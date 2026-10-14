# Hi, I'm Gilvex

I like to imagine stuff and then make it.

I build collaborative web applications and reusable UI libraries with **TypeScript and React**, working across interaction design, APIs, persistence, and delivery. My current projects focus on preserving user work and making software reliable to integrate.

[Website](https://www.gilvex.link/) · [Public contributions](https://github.com/pulls?q=is%3Apr+author%3Agilvex+-user%3Agilvex)

## Selected work

### [Aril](https://github.com/gilvex/aril) — collaborative planning studio

Architecture diagrams, interface design, requirements, and shared notes in one workspace.

- Revision-checked saves, recoverable conflicts, personal undo, and concurrent note editing.
- SQLite and Postgres storage, workspace roles, expiring guest access, and scoped automation credentials.
- Real HTTP and two-instance Postgres integration tests, a reproducible contention benchmark, and a fixture-based SQLite restore drill.

[Try the demo](https://www.aril.studio/?demo=1) · [Engineering case study](https://github.com/gilvex/aril/blob/main/docs/engineering-case-study.md)

### [Vagabond UI](https://github.com/gilvex/vagabondui) — React component library

A published UI package with typed component exports, visual presets, and interactive application templates.

- Radix-based interactions, keyboard/focus behavior, responsive layouts, and accessibility checks.
- CI installs the packed library in an external npm consumer, checks declarations and React identity, and exercises the production browser build.
- Used as a versioned dependency in Aril; package publication and showcase deployment have separate verification workflows.

[Live showcase](https://gilvex.github.io/vagabondui/) · [npm](https://www.npmjs.com/package/vagabond-ui) · [Engineering case study](https://github.com/gilvex/vagabondui/blob/main/docs/engineering-case-study.md)

## Selected open-source contributions

- **rucken:** merged fixes for [database connection targeting](https://github.com/rucken/rucken/pull/17), [multi-user search](https://github.com/rucken/rucken/pull/18), and [missing-database handling](https://github.com/rucken/rucken/pull/20).
- **discord.js:** merged [documentation formatting correction](https://github.com/discordjs/discord.js/pull/9116).

## Engineering interests

Collaborative editing · Design systems · TypeScript package design · Persistence and recovery · Reproducible verification
