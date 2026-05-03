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
- Some summaries are empty — new additions should fill them by reading the paper's abstract and introduction.
- Many PDF filenames include a `[Venue-Year-Tier]` prefix that helps with classification.

## README Structure

```
# Awesome DRL Cloud Scheduling (header + badge)
## Contents (table of contents)
## Introduction
## Research Papers
  ### Resource Scheduling
  ### Autoscaling
  ### Edge Computing
  ### Paper Template (reference, should be removed before finalizing)
## Open-Source Projects (empty placeholder)
## Datasets (currently has alibaba/clusterdata)
## Tools & Frameworks (empty placeholder)
## Contributing
## References
## License (MIT)
```

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
- Several paper entries have empty `*Summary*:` fields that need filling
- The Open-Source Projects and Tools & Frameworks sections are empty placeholders
- Commit messages follow a simple convention: `"add X papers"`, `"update."`, etc.
- The repo uses MIT License
