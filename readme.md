# AI/ML Literature Review Repository

A structured and scalable repository for collecting, comparing, and synthesizing research papers in machine learning and AI.

This repository is designed for long-term PhD research workflows, enabling consistent documentation across hundreds of papers with a unified review schema.

## Repository Purpose

The goal of this repository is to support systematic literature review by:

- Tracking paper metadata and technical contributions in a standardized format
- Comparing methods, datasets, and evaluation practices across studies
- Recording critical analysis (strengths, limitations, and research relevance)
- Maintaining reproducible references and optional BibTeX integration

## Repository Structure

```text
.
+-- README.md
+-- LICENSE
+-- papers/
¦   +-- pdf/
¦   ¦   +-- 2025_Smith_ToolAugmentedReasoning.pdf
¦   ¦   +-- ...
¦   +-- notes/
¦   ¦   +-- P0001.md
¦   ¦   +-- ...
¦   +-- bib/
¦       +-- references.bib
+-- tables/
¦   +-- literature_review.csv
¦   +-- literature_review.xlsx
¦   +-- literature_review.md
+-- templates/
    +-- paper_note_template.md
    +-- literature_row_template.md
```

## Workflow: How to Add a Paper

1. Assign a new unique paper ID (e.g., `P0142`).
2. Save the PDF in `papers/pdf/` using the naming convention.
3. Add a BibTeX entry to `papers/bib/references.bib` (optional but recommended).
4. Create or update a detailed note file in `papers/notes/` (e.g., `P0142.md`).
5. Add one row to the master table in `tables/literature_review.csv` (or `.xlsx` / `.md`).
6. Validate completeness using the quality checklist.
7. Commit with a descriptive message.

## Literature Review Table Template

Use the same column schema across all table formats (`.csv`, `.xlsx`, `.md`).

| ID | Year | Title (with Authors) | Area | Problem | Key Contribution | Method Type | Dataset | Metrics | Strengths | Limitations | Artifacts (Code/Data availability) | Links | Personal Notes / Verdict |
|---|---:|---|---|---|---|---|---|---|---|---|---|---|---|
| P0001 | 2025 | *Reasoning with External Tools* (A. Smith, B. Lee) | LLM Reasoning | Multi-step reasoning failures in complex math tasks | Introduces verifier-guided tool interaction to reduce reasoning errors | Framework | GSM8K; MATH | Accuracy; Pass@1 | Strong empirical gains; clear ablations | Higher inference cost; tool dependency | Code: Yes; Data: Partial | [Paper](https://example.com) \| [Code](https://github.com/example) | Relevant baseline for tool-augmented reasoning; strong methodology |

## Naming Conventions

- **Paper ID:** `P0001`, `P0002`, ... (fixed-width numeric IDs)
- **PDF filename:** `YYYY_FirstAuthor_ShortTitle.pdf`
  - Example: `2024_Wang_SelfConsistencyReasoning.pdf`
- **Notes filename:** `<PaperID>.md`
  - Example: `P0001.md`
- **BibTeX key:** `FirstAuthorYearShortTag`
  - Example: `Wang2024SelfConsistency`

## Optional BibTeX Management

Maintain references in a single canonical file:

- `papers/bib/references.bib`

Recommended practice:

- Use one BibTeX entry per reviewed paper
- Keep venue names standardized (e.g., `NeurIPS`, `ICLR`, `ICML`, `ACL`)
- Include DOI, arXiv ID, and URL fields when available
- Align BibTeX key format with repository naming conventions

## Quality Checklist for Paper Review

Before marking a paper as reviewed, verify:

- [ ] Bibliographic metadata is complete (authors, year, venue, links)
- [ ] Problem statement is clearly and accurately summarized
- [ ] Key contribution is concise and technically specific
- [ ] Method type is categorized consistently
- [ ] Datasets and metrics are explicitly recorded
- [ ] Strengths and limitations include concrete technical points
- [ ] Artifact availability (code/data/models) is verified
- [ ] Personal verdict states relevance to your research direction
- [ ] Table formatting and naming conventions are consistent

## Scalability Guidelines

For long-term management of large literature sets (100+ papers):

- Keep `tables/literature_review.csv` as the source of truth for analysis
- Reserve `.xlsx` for manual filtering/visual review when needed
- Do not recycle paper IDs; preserve historical traceability
- Use controlled vocabulary in the `Area` and `Method Type` columns
- Prefer append-and-update workflows over destructive edits

## License and Copyright

- Add a repository `LICENSE` file (commonly `MIT` for repository structure/scripts or `CC BY 4.0` for notes).
- Original research papers remain the intellectual property of their respective authors/publishers.
- Store and share PDFs only in compliance with publisher and copyright policies.
