# 👋

I'm Eric Wang. Product manager by day. Builder by craft.

Currently working on ad-tech and influencer marketing — ad networks, creator marketplaces, the platform logic that connects advertisers with creators. Products at the intersection of money and content.

Before that I spent years in cross-border e-commerce, building the operational backbone: OMS, TMS, WMS, customer service platforms. The kind of infrastructure nobody notices until something breaks.

Somewhere around late 2025 I started building with AI agents. Not as a side project — because I needed tools that didn't exist and waiting for dev cycles wasn't an option. These are the ones that survived daily use.

---

## What I've built

### spec-analyze — the one I reach for every day

I write requirements. I hand them to a coding agent. The agent makes assumptions I never intended.

An agent doesn't ask "what about this edge case?" It just picks something and runs. Then I catch it in review, and we waste a round trip fixing what should have been right the first time.

So I built a spec analyzer. It runs a product requirement through multiple expert perspectives — product strategy, architecture, user experience, risk — before any code gets written. Each lens surfaces assumptions and blind spots that a single-pass spec would miss.

The output is a spec with edge cases already annotated. The agent gets it right more often on the first try.

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

- [@EricWangPM](https://x.com/EricWangPM) on X
