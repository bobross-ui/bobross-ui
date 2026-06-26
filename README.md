# Kshitij Ghode

Full-stack engineer building AI systems that hold up past the demo: agent memory, grounded retrieval,
and real-time apps with real users. I ship full products end-to-end, from the database schema to the
screen.

> Currently open to backend / AI-infrastructure roles.

## Featured Work

### [CAT-DUEL](https://github.com/bobross-ui/CAT-DUEL) - real-time 1v1 exam-prep duels

Two players, one question set, live Elo matchmaking, and timed scoring. The UI is the easy part; the
hard part is keeping game state consistent when both players answer on the same millisecond and
connections drop mid-duel. Solved with two-phase locking and Redis `NX` guards for race-free
concurrent scoring, plus reconnect-safe state so a dropped player rejoins exactly where they left
off.

`TypeScript | React Native | Expo | Node.js | Socket.io | Postgres | Redis | Prisma`

### [brain](https://github.com/bobross-ui/brain) - local-first memory layer for long-running agents

Scoped memories over raw conversation history with hybrid vector + BM25 retrieval, automatic fact
extraction, and reconciliation when new facts contradict old ones, all exposed as MCP tools so any
agent can plug in. Built with an eval harness from day one, so retrieval quality is measured, not
guessed.

LOCOMO `conv-26` reranker blend: **64.8% judged accuracy** (129/199), **73.6% fused evidence recall**,
**77.7% evidence hit rate**, 0 failures. Single-conversation experiment, 199 questions.

`Python | SQLite | sqlite-vec | FTS5 | Ollama | MCP`

### [cortex](https://github.com/bobross-ui/cortex) - social exports into a grounded knowledge base

Ingests personal exports into a pgvector store and answers questions with cited sources, so every
claim traces back to where it came from. Hybrid retrieval with reciprocal rank fusion instead of
naive score addition.

`Python | FastAPI | Postgres | pgvector | React | DeepSeek`

## What I'm Into

AI that's more than a chat box: memory that gets better the longer it runs, retrieval that can show
its work, and real-time interfaces that make complex flows feel direct. Most of what I build is solo,
in public, and shaped by real users instead of a slide.

## Stack

**Languages** | TypeScript | Python | SQL | JavaScript

**Frontend** | React | Next.js | React Native | Expo | Tailwind | Framer Motion

**Backend** | Node.js | Express | FastAPI | Prisma | PostgreSQL | Redis | SQLite

**AI / Retrieval** | RAG | embeddings | vector search | BM25/FTS | MCP | local LLM tooling

**Infra** | Docker | GitHub Actions | CI | testing | observability-minded design

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=bobross-ui&show_icons=true&theme=transparent&hide_border=true" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=bobross-ui&layout=compact&theme=transparent&hide_border=true" />
</p>
