# Ali Aliyev · Gilvex

**Frontend & product engineering.** At **Yandex**, I lead and own the Pickup Point Platform and build tools for the engineering team.

I build collaborative applications, reusable UI, and the systems behind them. **TypeScript / React**, from the first interaction to persistence and delivery.

Based in Baku; building for the web since 2018.

**[Explore the projects ↓](#pick-a-project)** · [Website](https://www.gilvex.link/) · [Résumé](https://www.gilvex.link/resume/) · [Say hello](mailto:skaneprime@gmail.com)

<a href="https://www.gilvex.link/">
  <img src="./assets/workbench.svg" width="100%" alt="Gilvex — I like to imagine stuff and then make it. Open my website.">
</a>

## Pick a project

Click a preview to try it. Open an inspector to see the engineering underneath.

<a href="https://www.aril.studio/?demo=1">
  <img src="./assets/aril.svg" width="100%" alt="Aril — illustrated collaborative canvas. Click to open the editable, account-free demo.">
</a>

**A shared space for architecture, interface design, requirements, and notes.**

[Launch demo ↗](https://www.aril.studio/?demo=1) · [Source](https://github.com/gilvex/aril) · [Case study](https://github.com/gilvex/aril/blob/main/docs/engineering-case-study.md)

[![Aril verification status](https://github.com/gilvex/aril/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/gilvex/aril/actions/workflows/ci.yml)

<details>
<summary><strong>Inspect Aril → What happens when two people edit at once?</strong></summary>

<br>

An edit is more than a new value. It has a base revision, preconditions, and a recovery path.

```text
edit → validate → revision check → atomic save
                       ↓
                 conflict detected
                       ↓
              preserve draft → recover
```

- **Durable work:** SQLite/Postgres persistence, revision checks, request deduplication, and personal undo.
- **Live collaboration:** Yjs note editing; transient cursors and previews stay separate from durable writes.
- **Evidence:** real HTTP tests, two-instance Postgres CI, a SQLite restore drill, and a measured contention baseline.
- **A useful finding:** the benchmark exposed long waits from immediate retries under contention. [Read the results and trade-offs](https://github.com/gilvex/aril/blob/main/docs/engineering-case-study.md#measured-local-baseline--2026-10-14).

The demo uses sample data and simulated teammates. Aril plans systems; it does not execute deployments.

</details>

<br>

<a href="https://gilvex.github.io/vagabondui/">
  <img src="./assets/vagabond.svg" width="100%" alt="Vagabond UI — illustrated component workbench. Click to explore the live React component showcase.">
</a>

**A React component library with visual presets and interactive application templates.**

[Explore components ↗](https://gilvex.github.io/vagabondui/) · [Source](https://github.com/gilvex/vagabondui) · [npm](https://www.npmjs.com/package/vagabond-ui) · [Case study](https://github.com/gilvex/vagabondui/blob/main/docs/engineering-case-study.md)

[![Vagabond UI verification status](https://github.com/gilvex/vagabondui/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/gilvex/vagabondui/actions/workflows/ci.yml)

<details>
<summary><strong>Inspect Vagabond UI → Does it work outside its own repository?</strong></summary>

<br>

The showcase working is only the first check. CI also exercises what a consumer actually installs.

```text
source → build → npm tarball
                     ↓
            isolated consumer install
                     ↓
        types + exports + browser checks
```

- **Package contract:** typed subpath exports, React peers, and compiled CSS.
- **Interaction contract:** keyboard/focus behavior, reduced motion, responsive layouts, and accessibility checks.
- **Consumer evidence:** a separate npm installation checks declarations and React identity, then runs a production browser build.
- **In use:** Aril consumes the versioned package. Both projects are maintained by me.

[Read the packaging decisions](https://github.com/gilvex/vagabondui/blob/main/docs/engineering-case-study.md) · [Try the banking template](https://gilvex.github.io/vagabondui/#template/banking)

</details>

## Beyond the demos

<details>
<summary><strong>Open the experience drawer → Platforms, teams, and delivery</strong></summary>

<br>

- **Yandex:** Pickup Point Platform ownership, frontend architecture, release pipelines, and developer tooling.
- **Farcana:** real-time search interfaces, WebSocket connection handling, server state, and component-library work.
- **Onix:** full-stack development and leadership of a distributed team.
- **Desktop and product work:** React/Tauri integration, file-integrity checks, frontend performance, and deployment workflows.

[Full résumé](https://www.gilvex.link/resume/) · [Selected professional work](https://www.gilvex.link/#work)

</details>

<details>
<summary><strong>Browse contributions → Changes in other people's projects</strong></summary>

<br>

Merged contributions:

- **rucken:** [database connection targeting](https://github.com/rucken/rucken/pull/17), [multi-user search](https://github.com/rucken/rucken/pull/18), and [missing-database handling](https://github.com/rucken/rucken/pull/20).
- **discord.js:** [documentation formatting correction](https://github.com/discordjs/discord.js/pull/9116).

[All public pull requests in external repositories](https://github.com/pulls?q=is%3Apr+author%3Agilvex+-user%3Agilvex)

</details>

## Field notes

- [Migrating a frontend to Feature-Sliced Design](https://www.gilvex.link/writing/architecture-that-earns-its-complexity/)
- [Finding a frontend performance bottleneck](https://www.gilvex.link/writing/performance-is-a-product-feature/)
- [Handling disconnects and stale WebSocket responses](https://www.gilvex.link/writing/building-resilient-realtime-interfaces/)

---

**I like to imagine stuff and then make it.**

[Let's build something ↗](mailto:skaneprime@gmail.com) · [LinkedIn](https://www.linkedin.com/in/the-ali-aliyev/) · [How this README works](./docs/profile-design.md)
