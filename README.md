# 👋

I'm Eric Wang. Product manager by day. Builder by craft.

Currently working on ad-tech and influencer marketing — ad networks, creator marketplaces, the platform logic that connects advertisers with creators. Products at the intersection of money and content.

Before that I spent years in cross-border e-commerce, building the operational backbone: OMS, TMS, WMS, customer service platforms. The kind of infrastructure nobody notices until something breaks.

Somewhere around late 2025 I started building with AI agents. Not as a side project — because I needed tools that didn't exist and waiting for dev cycles wasn't an option. These are the ones that survived daily use.

---

## What I've built

### spec-analyze — the one I reach for every day

I write requirements. I hand them to a coding agent. The agent makes assumptions I never intended.

That was the original problem. So I built [spec-analyze](https://github.com/SWUNwy/spec-analyze) to close that gap — run requirements through multiple expert lenses before any code gets written. Force the edge cases to surface before the agent goes off-course.

That was v3.

**v5.0.0** reshapes it around how PMs actually work, not just how coding agents receive specs.

The old version started with a requirement and asked: how do I make this clear enough? The new version starts earlier: should I even be writing this requirement?

Five modes, one entry point — routed by what you actually need right now:

- **Understand** — you received something from your boss, a user, sales. Strip the noise, restate the real problem, name what's still unknown.
- **Challenge** — identify the hidden assumptions. Find the weak spots. Build the argument for pushing back. The output is an assumption map, a list of pointed questions to ask the requester, and a verdict: proceed / validate X first / push back.
- **Design** — problem is clear, now figure out how to solve it. Two or three directions, key tradeoffs per direction, a recommendation with the one variable that would flip it.
- **Specify** — PM-only interaction annotations (numbered badge anchors, bidirectional scroll sync, no SVG drift on complex pages), PRD, or the full proposal + design + tasks set.
- **Decide** — RICE, Kano, Decision Matrix. Guided scoring, not just framework names listed.

The challenge mode is what was missing before. Most requirement tools assume you've already decided to build. This one helps you decide whether to.

Annotations are PM-only now. Feature, logic, states, boundary, copy. No API paths, no CSS specs, no accessibility annotations sitting in a product document. The output is what a PM actually needs to hand off, not a mixed bag of product and implementation details.

### project-knowledge — session continuity

Claude Code starts every session with no memory of your project. I'd spend the first 10 minutes re-explaining architecture, naming conventions, design decisions.

This skill scans any codebase and generates a `.claude/knowledge/` directory — an index, a project glossary, key architectural points, and reference docs. The agent loads it at session start. No more context reset.

### spec-sdd — the methodology

This formalizes how I approach AI-assisted development:

**Spec → Plan → Implement → Verify**

Each phase has a Definition of Done. No phase starts until the previous one passes. It prevents the most expensive mistake in AI-assisted development: building the wrong thing really fast.

MIT-licensed.

### llm-knowledge-base

I had documents everywhere — Lark, PDFs, web pages, meeting transcripts. I wanted one place to search across all of them.

So I built a self-hosted knowledge base. It ingests 15+ file formats, converts them to Markdown via Microsoft MarkItDown, builds an Obsidian wiki with `[[bidirectional links]]`, and answers questions against your content.

114 commits. Many Docker compose rewrites.

---

## How I work

I define the boundaries. The agent fills the details. I review everything.

If I can't understand the code after the agent writes it, I refactor until I can. Code I don't understand is code I can't ship.

Stack: Python, JavaScript, Go, Docker — whatever the problem needs.

---

## Find me

- [@EricW7777777](https://x.com/EricW7777777) on X
