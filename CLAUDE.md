# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with this repository.

## Repository Overview

**awesome-drl-cloud-scheduling** is an [awesome-list](https://awesome.re)-style curated catalog of Deep Reinforcement Learning (DRL) research papers and resources for cloud computing:

- **Resource scheduling / placement** in cloud environments
- **Service autoscaling** (microservice scaling)
- **Cloud-level scheduling** combining task placement and dynamic resource allocation

The entire repository is a single `README.md` — no code, no build system, no tests.

## Key Directories (external to this repo)

PDF collections referenced for paper additions live in sibling directories:

| Directory | Purpose |
|---|---|
| `D:/Papers/CloudScheduling/` | Resource scheduling & cloud management PDFs (~60 files) |
| `D:/Papers/Autoscaling/` | Autoscaling & microservice PDFs (~55 files) |
| `D:/Papers/DRL/` | General DRL papers |

## Paper Entry Format

Every paper in the README follows this exact template:

```markdown
- **[Title](official_url)**
  *Authors*: Author list
  *Publication*: Conference/Journal-Year (e.g., TPDS-2024, OSDI-2020, KDD-2022)
  *Summary*: 2-4 sentence English summary of problem, method, and results
```

**Conventions:**
- Links should point to IEEE Xplore, ACM DL, USENIX, or the paper's official page. Fall back to arXiv if none available.
- Publication abbreviations: `TPDS`, `TSC`, `TAAS` (IEEE journals); `OSDI`, `ATC`, `ASPLOS`, `KDD`, `ICWS`, `SoCC`, `EuroSys` (conferences); include tier markers like `-A会`, `-A刊`, `-B会` when known.
- All DRL papers have specific summaries. Beyond DRL papers may use generic summaries — see Known Issues below.
- Many PDF filenames include a `[Venue-Year-Tier]` prefix that helps with classification.

## README Structure

```
# Awesome DRL Cloud Scheduling (header + badge)
## Contents (table of contents)
## Introduction
## Research Papers
  ### DRL — Resource Scheduling
  ### DRL — Autoscaling
  ### DRL — Edge Computing
  ### DRL — Robustness & Security
## Beyond DRL
  ### Benchmarks & Simulators
  ### Heuristic & Evolutionary Scheduling
  ### ML Predictive Autoscaling
  ### Microservice Architecture & Analysis
  ### Other
  ### Surveys & Reviews
  ### System Design & Platform
  ### Traditional Autoscaling
  ### Traditional Resource Management
  ### Workload Analysis & Characterization
## Open-Source Projects (empty placeholder)
## Datasets (currently has alibaba/clusterdata)
## Tools & Frameworks (empty placeholder)
## Contributing
## References
## License (MIT)
```

Total: ~219 paper entries across 14 sections.

## Common Tasks

### Adding a new paper
1. Find the appropriate section (Resource Scheduling / Autoscaling / Edge Computing)
2. Add a new entry using the format above, placing it after existing entries in that section
3. Extract metadata from the PDF file or its filename (which often contains venue/year)
4. Write a concise 50-80 word summary from the abstract/introduction

### Extracting PDF metadata
PDFs in `CloudScheduling/` and `Autoscaling/` directories have naming conventions like:
`[TPDS-2023-A刊]Paper_Title.pdf` — extract venue, year, and tier from the prefix.

### Searching for open-source code
Search `"paper title" GitHub` or `"first author" code GitHub` to find associated repositories. Record as `Code: [Available](url)` or `Not available`.

## Notes
- The `### Paper Template` section is a reference placeholder — it should be removed when the README is finalized
- The Open-Source Projects and Tools & Frameworks sections are empty placeholders
- Commit messages follow a simple convention: `"add X papers"`, `"update."`, etc.
- The repo uses MIT License

## Known Issues (as of 2026-05-05)
- **Generic summaries in Beyond DRL sections**: ~60 papers in "Beyond DRL" categories (Heuristic & Evolutionary Scheduling, Traditional Autoscaling, Traditional Resource Management, etc.) use generic placeholder summaries like "This paper presents a traditional (non-RL) approach for cloud resource management..." or "This paper proposes a heuristic or evolutionary algorithm for cloud task scheduling...". These require reading each paper's abstract/introduction individually to replace with specific summaries.
- **Beyond DRL author data**: Some Beyond DRL papers have "TBD" authors because the review document only lists them as reference numbers without full author names.
- **URL verification**: ~10 ACM/Elsevier/MDPI links return HTTP 403 for automated checks (likely fine in browser); not individually verified.
