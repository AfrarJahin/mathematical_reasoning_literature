# AI/ML Literature Review Repository

A structured and scalable repository for collecting, comparing, and synthesizing research papers in machine learning and AI.

This repository is designed for long-term PhD research workflows, enabling consistent documentation across hundreds of papers with a unified review schema.

## Repository Purpose

The goal of this repository is to support systematic literature review by:

- Tracking paper metadata and technical contributions in a standardized format
- Comparing methods, datasets, and evaluation practices across studies
- Recording critical analysis (strengths, limitations, and research relevance)
- Maintaining reproducible references and optional BibTeX integration

<!-- ## Repository Structure

```text
.
+-- README.md
+-- LICENSE
+-- papers/
�   +-- pdf/
�   �   +-- 2025_Smith_ToolAugmentedReasoning.pdf
�   �   +-- ...
�   +-- notes/
�   �   +-- P0001.md
�   �   +-- ...
�   +-- bib/
�       +-- references.bib
+-- tables/
�   +-- literature_review.csv
�   +-- literature_review.xlsx
�   +-- literature_review.md
+-- templates/
    +-- paper_note_template.md
    +-- literature_row_template.md
``` -->

<!-- ## Workflow: How to Add a Paper

1. Assign a new unique paper ID (e.g., `P0142`).
2. Save the PDF in `papers/pdf/` using the naming convention.
3. Add a BibTeX entry to `papers/bib/references.bib` (optional but recommended).
4. Create or update a detailed note file in `papers/notes/` (e.g., `P0142.md`).
5. Add one row to the master table in `tables/literature_review.csv` (or `.xlsx` / `.md`).
6. Validate completeness using the quality checklist.
7. Commit with a descriptive message. -->

## Literature Review Table Template

## Literature Review Table

| No. | Paper | Year | Venue | Dataset | Method | Strength | Weakness | Gaps | Link |
|---:|---|---|---|---|---|---|---|---|---|
| 1 | VCR: A "Cone of Experience" Driven Synthetic Data Generation Framework for Mathematical Reasoning | 2025 | AAAI 2025 |  |  |  |  |  | [Paper](https://doi.org/10.1609/aaai.v39i23.34645) |
| 2 | Flow-DPO: Improving LLM Mathematical Reasoning | 2024 (Oct) | Microsoft Research (Preprint) |  |  |  |  |  | [Paper](https://arxiv.org/abs/2410.22304) |
| 3 | Group-in-Group Policy Optimization for LLM Agent Training | 2025 | NeurIPS 2025 (Poster) |  |  |  |  |  | [Paper](https://arxiv.org/abs/2505.10978) |
| 4 | Adaptive Coopetition: Leveraging Coarse Verifier Signals for Resilient Multi-Agent LLM Reasoning | 2025 | arXiv / IJCNLP 2025 SRW |  |  |  |  |  | [Paper](https://arxiv.org/abs/2510.18179) |
| 5 | NeuroSymbolic LLM for Mathematical Reasoning and Software Engineering | 2024 | IJCAI 2024 |  |  |  |  |  | [Paper](https://www.ijcai.org/proceedings/2024/961) |
| 6 | AgenticMath: Enhancing LLM Reasoning via Agentic-based Math Data Generation | 2026 (Jan) | arXiv |  |  |  |  |  | [Paper](https://arxiv.org/abs/2510.19361) |

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


