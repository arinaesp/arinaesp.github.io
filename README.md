# arinaesp.github.io

Personal portfolio of **Arina Bolotbekova** — full-stack web developer, formerly an IDP-certified IELTS
instructor and TEFL/TESOL English teacher. Live at **[arinaesp.github.io](https://arinaesp.github.io)**.

## Projects

### [axo](https://arinaesp.github.io/axo.html) — [live app →](https://arinaesp.github.io/axo/)
A Telegram Mini App that teaches kids to code — and teaches them to read, write, and speak
English through the coding commands themselves. Grounded in Total Physical Response (TPR), a
language-teaching method that pairs instruction with action. Full market research and
positioning documented on the [research page](https://arinaesp.github.io/axo-research.html).

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
Real-time multiplayer over WebSockets, server-authoritative game state (the client only
renders what it's told), and a custom `security-reviewer` subagent audit before shipping —
four findings fixed pre-launch, including input validation, rate limiting, and CORS scoping.

## Background

Before writing code, I taught English — IELTS Writing and Speaking, TEFL/TESOL certified,
with course curricula I wrote and built myself from scratch. Teaching kids to code
later on, alongside my English teaching, is where the idea behind axo came from: the two
skills reinforced each other far more than teaching them separately. That observation is
the founding thesis behind everything in this portfolio.

## Stack

Everything here is static HTML/CSS/JS with no build step, except Lead the Ship (Astro) and
Tic-Tac-Toe (needs a persistent Node.js/Express/Socket.io server — planned for VPS deployment,
not hosted on GitHub Pages). No frameworks to install for the rest — clone it, open
`index.html`, done.

## Contact

[GitHub](https://github.com/arinaesp)
