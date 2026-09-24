# arinaesp.github.io

Personal portfolio of **Arina Bolotbekova** — full-stack developer, author of the CT-DGBLL framework (formerly ILLA),
former TEFL/TESOL and IDP-certified instructor. Live at **[arinaesp.github.io](https://arinaesp.github.io)**.

## Research & Methodology

### [CT-DGBLL (formerly ILLA)](https://arinaesp.github.io/methodology.html)

ILLA was the 2026 working name of the framework now called CT-DGBLL (Computational
Thinking Digital Game-Based Language Learning): early English literacy and computational
thinking, learned at the same time through commands that are English words and program
instructions at once. Two conceptual papers are in preparation; **axo** (below) is the
app that implements the framework.

## Projects

### [axo](https://arinaesp.github.io/axo.html) — [live app →](https://axo.axocoder.workers.dev/)

A Telegram Mini App built on **CT-DGBLL** (above) — the methodology I developed fusing early coding logic with
English language acquisition into a single learning loop, an approach with no found precedent
in the products surveyed. axo works as an interactive bridge into English literacy for children,
complementing rather than replacing formal instruction: kids see a word, type the code command,
hear it spoken, and watch axo act it out. Grounded in Total Physical Response (TPR), a
language-teaching principle developed by James Asher that pairs instruction with physical
action. Runs on a Cloudflare Worker with a D1 database: server-side verification of Telegram
`initData` signatures, group membership gating, per-user rate limiting, and secrets that never
reach the browser. Full market research and positioning documented on the
[research page](https://arinaesp.github.io/axo-research.html).

### [Lead the Ship](https://arinaesp.github.io/leadtheship.html)

A bilingual (Russian/English) education platform for young people in Kyrgyzstan and Central
Asia — 40+ pages, built solo in four days. Full Astro build: content collections, structured
data across six JSON-LD schema types, self-hosted subsetted fonts (Latin + Cyrillic + Kyrgyz),
and a GitHub Actions deploy pipeline.

### [WhisperFlow](https://arinaesp.github.io/whisperflow.html) — [source →](https://github.com/arinaesp/local-whisper-flow)

An independent, local alternative to Wispr Flow: private, on-device push-to-talk voice
dictation for Windows, built on faster-whisper. No cloud calls after the initial model
download, no disk writes of transcripts, published as v1.0.0.

### [Tic-Tac-Toe](https://arinaesp.github.io/tictactoe.html) — [source →](https://github.com/arinaesp/tic-tac-toe-game)

A Node.js/Express/Socket.io backend running real-time multiplayer over WebSockets. Game
state is server-authoritative — the client only renders what it's told, no game logic runs
in the browser. Hardened with per-IP connection caps, a bounded matchmaking queue, move
rate limiting, input validation, and scoped CORS, all after a custom `security-reviewer`
subagent audit before shipping.

## Writing

### [Bridging Code Mechanics and Language Acquisition](https://arinaesp.github.io/writing.html)

A personal essay on why I built axo — the moment while teaching coding when I watched a
child pick up English commands fast without even knowing the alphabet, the research behind
Total Physical Response as a teaching method, and a candid look at its open questions and
how I'm putting them to the test. First-person, research-backed, illustrated with original
charts.

## Background

Before transitioning into full-stack development, I spent years teaching English across every
age group — adults, teenagers, and young learners. When I later began teaching children introductory
coding alongside language, I noticed an immediate pattern: the two skills reinforced each other
far more effectively together than apart. That core observation became the founding thesis behind
axo and the driving philosophy behind my software development.

## Stack

Each project is built on what it actually needs, not on one template:

- **axo** — Cloudflare Worker (edge runtime) + D1 SQLite database. Handles auth, group-membership
  verification against the Telegram Bot API, rate limiting, and static asset serving from a
  single Worker. Vanilla JS on the client, which holds no secrets and makes no access decisions.
- **Lead the Ship** — Astro: content collections, JSON-LD structured data, self-hosted
  subsetted fonts, GitHub Actions deploy pipeline.
- **WhisperFlow** — Python on top of faster-whisper, running entirely on-device.
- **Tic-Tac-Toe** — Node.js + Express + Socket.io backend. Server-authoritative game state
  over WebSockets, so it needs a persistent Node process — not static hosting.
- **These portfolio pages** — hand-written HTML/CSS/JS with no build step. Clone, open
  `index.html`, done.

## Contact

[GitHub](https://github.com/arinaesp)
