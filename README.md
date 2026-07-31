# arinaesp.github.io

Personal portfolio of **Arina Bolotbekova** — full-stack web developer, formerly an IDP-certified IELTS
instructor and TEFL/TESOL English teacher. Live at **[arinaesp.github.io](https://arinaesp.github.io)**.

## Projects

### [axo](https://arinaesp.github.io/axo.html) — [live app →](https://arinaesp.github.io/axo/)
A Telegram Mini App that teaches kids to code — and teaches them to read, write, and speak
English through the coding commands themselves. Grounded in Total Physical Response (TPR), a
language-teaching method that pairs instruction with action. Runs on a Cloudflare Worker
with a D1 database: server-side verification of Telegram `initData` signatures, group
membership gating, per-user rate limiting, and secrets that never reach the browser. Full
market research and positioning documented on the
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

### [Teaching Kids English Through Code, Not Around It](https://arinaesp.github.io/writing.html)
A personal essay on why I built axo — the classroom moment that sparked it, the research
behind Total Physical Response as a teaching method, and an honest look at where the idea
could still be wrong. First-person, research-backed, illustrated with original charts.

## Background

Before writing code, I taught English — IELTS Writing and Speaking, TEFL/TESOL certified,
with course curricula I wrote and built myself from scratch. Teaching kids to code
later on, alongside my English teaching, is where the idea behind axo came from: the two
skills reinforced each other far more than teaching them separately. That observation is
the founding thesis behind everything in this portfolio.

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
