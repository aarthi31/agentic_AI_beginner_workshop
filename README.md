<p align="center">
  <img src="coAI%20logo%201%201.png" alt="Champions of AI (coAI) logo" width="400">
</p>

# Co-AI Beginner Workshop: Agentic AI Fundamentals

Materials for the beginner AI workshop held on **14 October 2026** (1:00–4:00 PM), presented by Aarthi Ravikrishnan and Deepa Ramasamy (A*STAR). The workshop uses Claude and Microsoft 365 Copilot on five hands-on examples drawn from everyday research work. **All data in this repository is synthetic.**

Each `ExampleN_*` folder contains a participant handout (`.docx` and `.pdf`) plus the files that exercise needs.

## Workshop schedule

See `Workshop schedule 14102026.docx`.

| Time | Session |
|---|---|
| 1:00 – 1:30 PM | Introduction |
| 1:30 – 2:10 PM | Data parsing example (Example 1) |
| 2:10 – 2:30 PM | Making an A*STAR template skill file (Example 2) |
| 2:30 – 2:45 PM | Break |
| 2:45 – 3:00 PM | ETO |
| 3:00 – 4:00 PM | Literature agent and experimental design (Examples 3–5); participants build a presentation with data visuals using the A*STAR template |

## Repository contents

### Example 1: Data parsing (`Example1_data_parsing/`)

Turn three messy clinical data files from the synthetic SKIN-AD study into one tidy CSV, comparing a naive prompt, an instruction-file prompt and a reusable Claude Project / skill.

| File | Description |
|---|---|
| `exercise1_handout.pdf` / `.docx` | Participant handout (naive, beginner and intermediate versions) |
| `data/SiteA_SKINAD_FINAL_v3.xlsx` | Raw Site A data (Excel) |
| `data/siteB_export_20240615.csv` | Raw Site B data (semicolon-delimited CSV) |
| `data/siteC_CRF_typed.txt` | Raw Site C data (typed CRF text) |
| `skinad_instructions.md` / `.txt` | Cleaning rules and data dictionary to paste into a Claude Project's instructions (same content in two formats) |
| `skills.md` | Plain-text copy of the project instructions and data dictionary |
| `skinad-data-wrangler.skill` | Packaged Claude skill that cleans and combines the three site files into `clean_skinad.csv` |
### Example 2: A*STAR presentation template skill (`Example2_astar_template/`)

Use Claude's skill-creator to turn the A*STAR master PowerPoint template into a reusable skill, then invoke it with `/astar-presentation-template`.

| File | Description |
|---|---|
| `exercise2_handout.pdf` / `.docx` | Participant handout |
| `ASTAR 00_MASTER_PPT_2026.potx` | A*STAR master PowerPoint template, the input for skill creation |
| `astar-presentation-template.skill` | Finished skill built from the template |

### Example 3: Literature mining (`Example3_Literature_mining/`)

Connect the PubMed connector to Claude and follow a workflow from topic to search strategy, screened reading list, citations, gap analysis and draft Specific Aims, with a prompt library for each stage.

| File | Description |
|---|---|
| `example3_handout.pdf` / `.docx` | Participant handout |
| `review-lit-agent.skill` | Skill that builds a topic-scoped PubMed search agent with a citation manager |

### Example 4: Biological data analysis (`Example4_BiologicalDataAnalysis/`)

Use the Claude for Microsoft 365 add-in in Excel to take raw qPCR Ct values through ΔCt, ΔΔCt, fold change, statistical testing and publication-style figures.

| File | Description |
|---|---|
| `exercise4_handout.pdf` / `.docx` | Participant handout |
| `Raw_data_analysis_qPCR.xlsx` | Raw qPCR dataset (starting point) |
| `Analysed_data_Claude_plugin.xlsx` | Worked result produced with the Claude Excel add-in, for comparison |

### Example 5: Demo, Wet Lab Biology Assistant (`Example5_Demo/`)

Build, use and verify a "Wet Lab Biology Assistant" agent in Microsoft 365 Copilot Agent Builder, covering planning, wet-lab calculations, data analysis and scientific writing.

| File | Description |
|---|---|
| `exercise5d_handout_copilot.pdf` / `.docx` | Participant handout |
| `Data_analysis_agent/` | Placeholder folder (currently empty) |

## Requirements

- **Examples 1–3:** a Claude account (skills and connectors need a paid plan).
- **Example 4:** a paid Claude plan and a Microsoft 365 work or school subscription for the Claude add-in.
- **Example 5:** Microsoft 365 Copilot with Agent Builder access.

## Usage notes

- To install a `.skill` file, upload it in Claude under Settings → Skills (or follow the steps in the matching handout).
- Raw data files are inputs only; the exercises are designed so that originals are never modified.

## Authors

Aarthi Ravikrishnan (A*SRL) and Deepa Ramasamy (IMCB), A*STAR.
