# Gnophy

[![Website](https://img.shields.io/badge/web-gnophy.com-blue)](https://gnophy.com)  
[![License – TBD](https://img.shields.io/badge/license-TBD-lightgrey)]()

# gnophy.com

> A philosophy companion powered by AI — converse with philosopher personas, explore a knowledge graph of ideas, and sharpen your reasoning.

---

## 🎯 What Is Gnophy?

**Gnophy** is an AI-driven tool for engaging with philosophical ideas in a conversational, exploratory way. You can:

- Chat with **philosopher personas** built on primary texts and structured summaries
- Navigate a **knowledge graph** of interrelated ideas, themes, and thinkers
- Use **semantic (vector-based) search** to find conceptually relevant content (not just by keywords)
- Interact by **text or voice**, with transcripts flowing into a unified timeline

The mission: make philosophy **accessible, interactive, and personally meaningful** — so users learn by questioning and exploring, not by rote memorization. :contentReference[oaicite:0]{index=0}

---

## 🧩 Architecture (High-Level)

Here’s how the components of Gnophy fit together:

| Layer / Component                 | Purpose                                                | Technology (current)                                                              |
| --------------------------------- | ------------------------------------------------------ | --------------------------------------------------------------------------------- |
| **Document & Content Store**      | Curated texts, summaries, and metadata                 | —                                                                                 |
| **Knowledge Graph**               | Models philosophers, concepts, connections             | Neo4j :contentReference[oaicite:1]{index=1}                                       |
| **Semantic / Vector Layer**       | Conceptual similarity search & embeddings              | Qdrant :contentReference[oaicite:2]{index=2}                                      |
| **Application & Session Storage** | Chat histories, user metadata, session state           | MongoDB :contentReference[oaicite:3]{index=3}                                     |
| **Frontend / UI**                 | Web client, pages like Chat, Explore, Persona, Academy | Next.js + Tailwind CSS :contentReference[oaicite:4]{index=4}                      |
| **Voice / Speech Integration**    | Speech-to-text input, audio handling                   | Custom pipeline (integrated into chat flow) :contentReference[oaicite:5]{index=5} |

**Key design principles:**

- Modular separation between content, graph, and chat logic
- Embeddings + vector search as a bridge between user intent and content
- Persona switching: you may “talk with” different philosophical voices
- Unified chat history: voice and text are merged seamlessly

---

## 🛠️ Public Repo Purpose & Scope

This public repository is **informational only** — it is not intended to hold private or production code (which remains in a separate private repository). Its goals:

1. **Public Visibility & Discovery**  
   Make Gnophy discoverable by recruiters, researchers, AI indexing tools, and the general public.

2. **Documentation & Architecture Reference**  
   Serve as a home for design overviews, system diagrams, API sketches, conceptual notes, and project context.

3. **Onboarding / Collaboration**  
   Provide a clear reference so new contributors or external reviewers can understand the system and vision.

### What _can_ be included in this repo

- README / project overview
- Architecture diagrams and visual models
- Design documents (persona engine, graph models, search flow)
- API contracts, JSON schemas, endpoint specs
- Screenshots, user flows, UI sketches
- Public roadmap and feature backlog (view-only)
- Contributing guidelines, governance notes, style guides
- Licensing and attribution (if and when open source modules are released)

### What _must not_ be included

- Secrets, API keys, credentials
- Internal, proprietary, or production-only source code
- Sensitive scripts or internal-only utilities

---

## 🛤 Roadmap & Future Directions

Planned and ongoing enhancements include:

- **Persona configuration & debate modes** — allow users to customize or stage structured dialogues
- **Interactive graph exploration** — visual tools to traverse ideas, themes, and thinkers
- **Expanded concept library** — deeper coverage of authors, schools, and cross-comparisons
- **Live voice responses** — real-time spoken replies rather than just transcripts
- **Session analytics & insights** — data on usage, learning paths, concept drift
- **Potential public SDK / modules** — open source components for embedding Gnophy functionality

---

## 📋 Sample Usage / Scenarios

Here are some examples of how people might use Gnophy:

- **Recruiters / Tech Evaluators** — read system architecture to assess viability, engineering-level decisions, tradeoffs
- **Philosophy Enthusiasts / Learners** — explore how the project maps ideas and persona interactions
- **Potential Contributors** — review design docs, propose modules or improvements
- **Curious Observers** — see “what’s under the hood” behind the product

---

## 🧭 How to Navigate This Repo

- **`/docs/`** — design documents, diagrams, architecture notes
- **`/apis/`** — API schema definitions, public contracts
- **`/ui-designs/`** — mockups, wireframes, screenshots
- **`/roadmap.md`** — public feature roadmap
- **`CONTRIBUTING.md`** — guidelines (if you later open contributions)
- **`LICENSE`** — to be added when/if you open source parts

---

## 📣 Acknowledgments & Contacts

- Inspired by the mission to make philosophy a living conversation
- Thanks to early testers, feedback communities, and design reviewers
- For questions, feedback, or private collaboration, contact: _[your email or contact link]_

---

## 🧾 License & Attribution

This repository is informational and currently **no license** is applied. If/when parts of Gnophy are open-sourced, they may be released under a permissive or copyleft license (e.g. MIT, Apache 2.0).

---

_Thank you for your interest in Gnophy. I hope this repo helps clarify the vision, architecture, and possibilities behind the project. Let me know if you'd like a version with graphics (SVG diagrams), more diagrams embedded, or a variant in a lighter “for non-tech” tone._

Good day...