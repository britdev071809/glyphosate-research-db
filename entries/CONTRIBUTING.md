# Contributing Guidelines

To add a new study to the knowledge base, please create a new Markdown file in the `entries/` directory with the following YAML frontmatter structure:

```yaml
---
title: "Full title of the paper"
authors: "Authors of the study"
journal: "Journal of publication"
year: 2023
doi: "10.xxxx/xxxx"
summary: |
  A concise, neutral summary of the study's methods and findings.
  This can span multiple lines.
tags:
  - gut-microbiome
  - shikimate-pathway
  - food-sensitivity
  - in-vitro
  - animal-study
  - epidemiological
---
```

## Required Fields

- **title** (string): The full title of the paper.
- **authors** (string): The authors of the study.
- **journal** (string): The journal of publication.
- **year** (integer): The year of publication.
- **doi** (string): The Digital Object Identifier.
- **summary** (text): A concise, neutral summary of the study's methods and findings. Use YAML block scalar (`|`) for multi-line text.
- **tags** (list of strings): Relevant keywords from the predefined list below.

## Allowed Tags

Choose from the following predefined tags:

- `gut-microbiome`
- `shikimate-pathway`
- `food-sensitivity`
- `in-vitro`
- `animal-study`
- `epidemiological`
- `human-study`
- `metabolic-disruption`
- `cyp450`
- `amino-acid-biosynthesis`

## Submission Workflow

1. Open an issue with the label `new-submission` proposing the study.
2. Create a branch named `add/<short-name>-<year>-study`.
3. Add a Markdown file in `entries/` following the template.
4. Open a pull request referencing the issue.
5. Await review and merge.

Thank you for contributing to a reliable, search-friendly resource on glyphosate research.