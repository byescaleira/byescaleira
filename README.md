<div align="center">

<img src="https://raw.githubusercontent.com/byescaleira/byescaleira/main/assets/helmet.png" width="132" alt="">

### How native software gets built when it can't fail.

**Rafael Escaleira** — iOS Specialist at **Globo**, on **Cartola**

</div>

---

Cartola is the largest fantasy football game in Brazil. Millions of people open
it on the same Sunday afternoon, every round, and the scores have to be right
the first time. That constraint is most of what I've learned: how to build
native software for a system that can't quietly fail and be fixed on Monday.

Everything below is either something I ship at work, or something I build to
make that work repeatable.

---

### Apple platform libraries

Two sibling Swift packages, built as one system. Cosmos is what things look
like; Nebula is how they're put together.

| | |
|---|---|
| **[cosmos](https://github.com/byescaleira/cosmos)** | A multi-platform SwiftUI design system for iOS, macOS, tvOS, watchOS and visionOS. Tokens, components and patterns that stay consistent across five platforms. |
| **[nebula](https://github.com/byescaleira/nebula)** | A clean-room Swift foundation and architecture library — the layer everything else is built on, with no third-party dependencies. |
| **[markly](https://github.com/byescaleira/markly)** | A SwiftUI markdown e-reader: chapters, multi-colour highlights, an Apple-Books-style toolbar, themes and share. Apple-only stack, Swift 6. |

All three carry CI and coverage, because a design system nobody trusts is
just a folder of opinions.

### Tooling for AI-assisted iOS work

The bet is that AI accelerates the craft and a human owns the outcome. These
exist to make that true in practice rather than in principle — by giving the
model the same conventions, tests and guardrails a senior reviewer would apply.

| | |
|---|---|
| **[daedalus](https://github.com/byescaleira/daedalus)** | A disciplined iOS agent for Claude Code — memory, planning, TDD, subagents and documentation in one plugin. |
| **[helios](https://github.com/byescaleira/helios)** | An invisible iOS specialist for Claude Code. Detects iOS projects and validates every change with build, tests, lint and format. |
| **[ios-spec](https://github.com/byescaleira/ios-spec)** | A local Ollama model tuned as an iOS engineering specialist, following the Cosmos and Nebula conventions. Built on `qwen3-coder:30b`. |
| **[byescaleira-plugin](https://github.com/byescaleira/byescaleira-plugin)** | My own operating system as a Claude Code plugin — codenames, repo template, branding rules, engineering rituals. |
| **[nova](https://github.com/byescaleira/nova)** | A reusable documentation template that renders a live OpenAPI spec into a readable site. |

### Shipped

| | |
|---|---|
| **Cartola** | Fantasy football, millions of players every round | [App Store](https://apps.apple.com/br/app/cartola-oficial/id1129547202) |
| **Next Joy** | Kids banking at Banco Next | [App Store](https://apps.apple.com/br/app/banco-next/id1435035468) |

---

### Career

**Globo / Cartola** — iOS Specialist · 2022–Present
**Deliver IT / Letsbank** — iOS Developer · 2022
**Next** — iOS Developer · 2021
**TocaLivros** — Mobile Developer · 2020
**Boviplan** — Mobile Developer · 2019
**A.A.A. UFMS** — Developer · 2018
**CATWORK** — Developer · 2017

### Stack

**Core** — Swift · SwiftUI · UIKit · Swift Concurrency · SPM
**Platforms** — iOS · iPadOS · watchOS · macOS · visionOS
**Architecture** — Modular SPM · Clean Architecture · MVVM · TDD
**Tooling** — Xcode · GitHub Actions · Fastlane · Firebase
**AI** — LLM APIs · CoreML · Vision · on-device inference

---

### How I work

**Native first.** Platform APIs before cross-platform shortcuts. Apple's
frameworks come before abstractions over them.

**Design is engineering.** Spacing, motion and typography are architecture
decisions, and they get the same review as any other interface.

**Small modules, clear contracts.** A boundary you can test is worth more than
a boundary that reads well in a diagram.

**Ship, then polish.** Working software in production beats a perfect branch.

---

<div align="center">

[byescaleira.com](https://byescaleira.com) ·
[LinkedIn](https://linkedin.com/in/rafael-eescaleira) ·
[X](https://x.com/byescaleira)

</div>
