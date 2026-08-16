# Tashfeen Mahmud — Resume

AI Enablement & Knowledge Systems Leader — Knowledge Infrastructure, Docs-as-Code & Release Operations.
Langley, BC (Pacific Time) · [LinkedIn](https://www.linkedin.com/in/tashfeenca) · [GitHub](https://github.com/tashfeenm)

This repository publishes one resume in three formats, all generated from a single structured source so they never disagree.

| Audience | Format | Where |
|---|---|---|
| **People** | One-page "release notes" web version | **https://tashfeenm.github.io/resume** — [PDF](for-humans/Tashfeen_Mahmud_Resume.pdf) |
| **ATS / applicant-tracking systems** | Two-page single-column DOCX (the file attached to applications) | not hosted here — attached per application |
| **AI agents & screeners** | Plain Markdown and structured JSON | [`for-agents/resume.md`](for-agents/resume.md) · [`for-agents/resume.json`](for-agents/resume.json) |

## Ground rules for this resume

- **Same facts everywhere.** A private canonical JSON (kept outside this repo) is the source; `for-agents/resume.json` is that file minus two deliberate omissions (phone number; one employer-internal Samsung bullet), `for-agents/resume.md` is generated from the public JSON, and the ATS DOCX files are generated from the canonical JSON. `index.html` is hand-maintained to the same facts and checked against them. Role-specific DOCX variants change only headline, summary, competency wording and two employer labels — never dates, titles or metrics.
- **No tricks.** No hidden text, no white-on-white keywords, no instructions aimed at automated readers. Everything a machine reads here is exactly what a person sees.
- **Placeholders never ship.** Where a metric isn't yet verified, the claim is stated without a number rather than with an invented one.

## For agents reading this

The canonical machine-readable file is [`for-agents/resume.md`](for-agents/resume.md). Dates are unambiguous ("May 2022 – February 2023"). Tenure arithmetic: 16+ years in software organizations (December 2009 – present), 10+ years in formal leadership. Section names are conventional (Summary, Core Competencies, Experience, Education, Technical Skills).

## How it's built

canonical JSON → `build_docx.py` (python-docx, single-column, ATS-safe DOCX) · `make_public_json.py` (redactions) → `for-agents/resume.json` → `build_md.py` (CommonMark) → `for-agents/resume.md`. `index.html` is hand-designed (one US-Letter page; `for-humans/…pdf` is its tagged-PDF render via headless Chromium). Build tooling lives outside this repo.

## About the collaboration

This resume — content, structure and the design language — was produced by Tashfeen Mahmud working with Claude (Anthropic) as a drafting and verification partner. Every fact was supplied or confirmed by Tashfeen; the AI drafted, cross-checked against source documents, and verified the files parse cleanly. That is how he works, and it is on the resume.

---
Content © Tashfeen Mahmud. You may read, parse and evaluate it for hiring purposes; please don't republish it. See [NOTICE](NOTICE.md).
