# arinaesp.github.io

Personal portfolio of **Arina Bolotbekova** — full-stack developer, author of the English Through Logic framework,
former TEFL/TESOL and IDP-certified instructor. Live at **[arinaesp.github.io](https://arinaesp.github.io)**.

## Research & Methodology

### [English Through Logic](https://arinaesp.github.io/methodology.html)

The framework behind axo: children learn English as the
language that runs a game, through commands that are English words and program
instructions at once. A conceptual paper is in preparation; **axo** (below) is the
app that implements the framework.

## Projects

### [axo](https://arinaesp.github.io/axo.html) — [play in browser →](https://play.axolab.space) · [Telegram →](https://t.me/axocoder_bot) · [site →](https://axolab.space)

A free game for children aged 5–9, in Telegram and in the browser, built on **English Through
Logic** (above): English is what children learn, and the logic of a game is the route, an
approach with no found precedent in the products surveyed. Kids hear and build a word, then
type it as a code command and watch axo act it out. **All 40 lessons are live**, in four zones:
sequences, arguments, loops and conditionals. axo complements formal instruction rather than
replacing it, and eight books are in progress, a student activity book and a teacher's book for
each zone, so teachers can run it in class. Its commands borrow the imperative from Total
Physical Response (James Asher); the action happens on screen instead of in the body. Runs on a Cloudflare Worker with a D1 database: server-side verification of Telegram
`initData` signatures, per-user rate limiting, anonymous usage totals with no IDs, and secrets
that never reach the browser. A paid access-code system is built and switched off by one
config flag while axo is free. Full market research and positioning documented on the
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
coding, I noticed something I didn't plan for: after one lesson, two brothers raced in the yard
shouting the commands they had typed, *move*, *turn right*, *attack*. The English had arrived as
the way to make something happen. That observation became the founding idea behind axo, and a
question I now want to measure properly.

## Stack

Each project is built on what it actually needs, not on one template:

- **axo** — Cloudflare Worker (edge runtime) + D1 SQLite database. Handles Telegram signature
  verification, rate limiting, anonymous usage counts, and static asset serving from a single
  Worker, with a switched-off access-code system kept behind one flag. Vanilla JS on the client, which holds no secrets and makes no access decisions.
- **Lead the Ship** — Astro: content collections, JSON-LD structured data, self-hosted
  subsetted fonts, GitHub Actions deploy pipeline.
- **WhisperFlow** — Python on top of faster-whisper, running entirely on-device.
- **Tic-Tac-Toe** — Node.js + Express + Socket.io backend. Server-authoritative game state
  over WebSockets, so it needs a persistent Node process — not static hosting.
- **These portfolio pages** — hand-written HTML/CSS/JS with no build step. Clone, open
  `index.html`, done.

## Contact

[GitHub](https://github.com/arinaesp) · Comments, suggestions, or a story of what worked (and what flopped) with axo: [hello@axolab.space](mailto:hello@axolab.space)
