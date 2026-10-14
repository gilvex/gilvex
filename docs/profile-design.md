# The profile workbench

## Direction

A small product workbench: original project artwork, direct links into working demos, and expandable inspectors that explain the engineering. The palette connects Aril's rose accent and Vagabond's muted green with a neutral studio header.

The public profile stays useful as ordinary text: project descriptions, résumé, source, case studies, contributions, and writing remain Markdown/HTML. Images have descriptive alternatives and never contain the only copy of an important link or claim.

## References reviewed

### Engineers at large technology companies

Roles below are publicly stated in the linked profiles/READMEs, checked October 14, 2026; they are not independently verified employment records.

| Profile | Publicly stated role | Useful pattern |
| --- | --- | --- |
| [Eugene Zhulenev](https://github.com/ezhulenev) | Senior Staff Software Engineer, Google; OpenXLA | Lead with technical ownership and concrete systems; animation supports the content |
| [Nghia Truong](https://github.com/ttnghia) | Distributed System Software Engineer, NVIDIA; GPU-accelerated Spark | A short introduction identifies the actual team/problem. Also described on his [about page](https://ttnghia.github.io/about/) |
| [continue-revolution](https://github.com/continue-revolution) | Software Engineer, NVIDIA; Megatron-LM | Current work, contact routes, and a small amount of personal context |
| [Robert Lee](https://github.com/robertklee) | Senior Software Engineer, Microsoft | Concrete ownership, reported outcomes, and projects; his [website](https://www.robertkl.com) adds interactive explanations |

The applied lesson: put Ali's current Yandex ownership, specialization, and résumé before decorative artwork. Use the previews and expandable inspectors to explain real work. These examples do not establish that a particular README style caused a hiring outcome.

### Visual and interaction references

| Profile | Interesting idea | Applied here |
| --- | --- | --- |
| [George Kobaidze](https://github.com/GeorgeKobaidze) | A distinctive visual identity built from linked SVG panels | Original themed header/project artwork |
| [Braydon Coyer](https://github.com/braydoncoyer) | Project-first introduction, portfolio links, and writing | Clear routes to demos, résumé, source, and notes |
| [Marc Zhuravlev](https://github.com/marcizhu) | A genuinely playable README chess board using issue-driven moves | A reminder to provide actions visitors can actually take; this profile uses native disclosure controls and working demo links |
| [G00dS0ul](https://github.com/G00dS0ul) | A coherent illustrated world and a linked interactive experience | Visual continuity between profile and the projects it opens |
| [Sindre Sorhus](https://github.com/sindresorhus) | A playful, unmistakably personal retro profile | Keep the original “imagine stuff and then make it” personality |

Discovery: [Awesome GitHub Profile README](https://github.com/abhisheknaiidu/awesome-github-profile-readme). Reviewed October 14, 2026. These are design references, not a ranking. The SVG artwork and layout here are original; no reference assets or code were copied.

## What is interactive

- The header opens the personal site; project previews open the editable Aril demo and Vagabond showcase.
- Native `<details>` / `<summary>` inspectors expand in GitHub and support keyboard activation.
- Build badges link to the actual main-branch verification workflows. GitHub may cache badge images; workflow logs are authoritative.
- The header has a short, one-shot CSS animation inside its SVG. Reduced-motion users get the settled illustration immediately.

GitHub READMEs do not run arbitrary JavaScript. The SVG illustrations are images, not embedded live editors; clicking the whole image follows its enclosing link. Actual editor/component interaction happens in the linked applications.

## Maintenance

Edit `README.md` for copy and links. Edit `assets/*.svg` for artwork. SVGs are dependency-free, use system fonts, and adapt through `prefers-color-scheme`; no font or rendering service is required. The settled artwork remains visible if animation is unavailable.

Professional context follows the public [website](https://www.gilvex.link/) and [résumé](https://www.gilvex.link/resume/). Update those claims together when responsibilities change. Technical claims link to the project case studies and real verification.

Preview GitHub's rendered Markdown, not just raw HTML: check image loading, keyboard disclosure controls, links, light/dark appearance, narrow widths, and reduced motion. GitHub's own theme choice can affect embedded image appearance; the panels retain their borders and contrast in either palette.
