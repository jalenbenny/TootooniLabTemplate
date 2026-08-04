# Contributing to Tootooni Lab Repositories

This repo is the starting point for every research project in the lab.
Fork or use it as a template, then follow the layout below.

## Getting started

1. Click **"Use this template"** on GitHub (or fork it).
2. Rename the repo to `topic-shortname` — all lowercase, kebab-case
   (e.g. `stroke-triage-nlp`, `precision-dosing-model`).
3. Fill in `README.md` — see the template already in this repo.
4. Delete this `CONTRIBUTING.md` from your copy, or leave it; either is fine.

## Layout

```
project-name/
├── README.md
├── data/
│   ├── raw/          gitignored — never commit real data here
│   └── processed/    synthetic or de-identified samples only
├── notebooks/         exploratory work
├── src/                pipeline code
├── results/            figures, tables, output
├── docs/                methods notes, IRB reference, data dictionary
├── environment.yml
├── LICENSE
└── CITATION.cff
```

## Data rules (non-negotiable)

- `data/raw/` is gitignored by default in this template. Do not remove
  that line from `.gitignore`.
- `data/processed/` holds only synthetic or de-identified sample data —
  enough to prove the pipeline runs, nothing patient-identifiable.
- The README's **Data Availability** section must say where the real
  data lives and who to contact for access.

## Projects without code

Not every project has code. If yours doesn't, you don't need this repo
at all — send a short write-up (same fields as the README: title,
status, tags, summary, contact) to whoever maintains
[TootooniLab.github.io](https://github.com/TootooniLab/TootooniLab.github.io)
and it'll be added to the Research page directly.

## Tags

Add tags to your README's front section and to the site listing.
Projects that span more than one area (e.g. `stroke`, `nlp`) should
carry all relevant tags — that's what lets them show up under each.
