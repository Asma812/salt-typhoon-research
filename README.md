# Trustworthy AI-Powered Threat Intelligence

## Evaluating LLMs for Evidence-Based Salt Typhoon Profiling

### 1. Project overview

This project evaluates whether evidence-grounded Large Language Models (LLMs)
produce more accurate, traceable and appropriately qualified Cyber Threat
Intelligence (CTI) profiles than models relying on their internal knowledge.

The study focuses on Salt Typhoon (MITRE ATT&CK G1045).

### 2. Research question

Does evidence-grounded AI profiling produce more accurate, traceable and
appropriately qualified CTI claims than standard closed-book LLM profiling?

### 3. Experimental design

Two models will be compared:

- NVIDIA Nemotron 3 Ultra
- Google Gemma 4 26B A4B

Two experimental conditions:

- A — Closed-book: the model receives no reference corpus.
- B — RAG: the model receives a reference corpus and must cite evidence passages.

The same analytical categories and output structure will be used
in both conditions.

### 4. Analysis categories

1. Objectives and intentions
2. Capabilities
3. Resources and organization
4. Targeted sectors and organizations
5. MITRE ATT&CK tactics and techniques
6. Attribution and confidence

### 5. Evaluation methodology

Generated claims will be manually annotated using four labels:

- Supported
- Distorted
- Unsupported / Invented
- Unverifiable

Evaluation will consider evidence support, uncertainty preservation,
claim quality, consistency across repeated runs, latency and cost.

### 6. Dataset

The reference corpus contains 29 evidence passages extracted from
publicly available government and cybersecurity research sources.

The corpus includes material from:

- MITRE ATT&CK
- FBI
- US Department of the Treasury
- CISA, FBI, NSA and partner agencies
- Canadian Centre for Cyber Security
- Tenable Research

Sources and passage identifiers are documented in the data directory.

ATT&CK Enterprise dataset version: 20.1.

Evidence concerning associated APT activity is distinguished from
direct Salt Typhoon attribution.

### 7. Repository structure

```text
salt-typhoon-research/
├── annotations/
│   └── annotation_guide.md
├── data/
│   ├── attack/
│   ├── originals/
│   ├── sources/
│   └── clean/
├── prompts/
│   ├── closed_book.txt
│   └── rag.txt
├── report/
├── results/
├── .gitignore
└── README.md
```

### 8. Pre-existing work

The following preparation was completed before the hackathon sprint:

- Research question and experimental scope definition.
- Selection of Salt Typhoon as the case study.
- Selection of the two LLMs and experimental conditions.
- Download and preparation of the MITRE ATT&CK dataset.
- Collection and cleaning of public reference sources.
- Creation and validation of 29 evidence passages.
- Preparation of the annotation guide.
- Drafting of the Closed-book and RAG prompts.
- Initial repository structure and documentation.
This preparation is disclosed to distinguish pre-event work
from implementation and experiments conducted during the sprint.

### 9. Project status

Pre-event preparation is ongoing.

The experimental pipeline, model executions, result analysis
and final evaluation will be conducted during the hackathon.

### 10. Reproducibility

Model versions, API parameters, execution dates, repetitions,
latency and cost will be documented during the experiment.

API keys and other secrets must never be committed to this repository.

