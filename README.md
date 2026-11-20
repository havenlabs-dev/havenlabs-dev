### Hi, I'm Aniken 👋

I build AI systems and the full-stack products and infrastructure underneath them, and I
ship them myself. Through HavenLabs I've built a self-hosted personal AI system I use every
day, a registration and payments platform in production, a RAG assistant for policy
documents, and mobile apps on iOS, Android and Garmin.

Most of my code is private because it holds real people's data. The repos below are case
studies with excerpts from the real code.

#### Featured work

**[HAVEN](https://github.com/havenlabs-dev/haven-case-study)**: a personal AI system that runs on my own server.
A Claude agent with 493 tools over one timeline of my data. Small decisions move to a local 4B
model only after it earns them statistically (Wilson lower bound ≥ 0.90 against Claude).
Speech-to-text, embeddings and the LLM all run on a 15 W laptop CPU.
*Python · FastAPI · SQLite · Claude Agent SDK · llama.cpp · Next.js · Expo · Kotlin*

**[EventHaven](https://github.com/havenlabs-dev/eventhaven-case-study)**: multi-tenant event registration, payments and CRM, live at eventhaven.app.
Atomic seat claims under advisory locks, webhooks that are safe to replay, Stripe Connect and
Authorize.net behind one interface, and org isolation enforced by Postgres RLS.
*Next.js 16 · TypeScript · Supabase · Stripe · Authorize.net*

**[PolicyLens](https://github.com/havenlabs-dev/policylens-case-study)**: a multi-tenant RAG assistant for policy documents.
Hybrid semantic and keyword retrieval, citations verified against the retrieved passages, and a
refusal with no LLM call when there's nothing to cite. Every provider can be swapped by config.
*Python · FastAPI · Qdrant · Postgres · React*

**[haven-architecture](https://github.com/havenlabs-dev/haven-architecture)**: how HAVEN is run.
A single-host production system, power-capped local inference, a scripted host migration with
20 minutes of downtime, backups, monitoring and real incident postmortems.
*Linux · systemd · Docker · Tailscale*

#### How I work

- **Reliability over cleverness.** The numbers in these write-ups were counted from the real repos,
  not estimated, and the HAVEN case study lists the command behind each one.
- **I build with AI coding agents** and act as the architect and reviewer, with guardrails
  that keep that safe: one restart path, test gates that can't touch real data, and checks that
  must be able to fail.
- **I'd rather show a known gap than hide it.** The write-ups say what isn't built yet.

#### Also built

Mobile apps on Expo/React Native (iOS + Google Play) · a Kotlin/Compose Android launcher ·
a Garmin Connect IQ watch app · client websites with online payments (Next.js, Neon, Vercel)

📫 [LinkedIn](https://www.linkedin.com/in/aniken-nielson/) · [havenlabs.dev](https://havenlabs.dev)
