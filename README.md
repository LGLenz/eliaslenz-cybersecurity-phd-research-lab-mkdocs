[![Deploy MkDocs to GitHub Pages](https://github.com/LGLenz/eliaslenz-cybersecurity-phd-research-lab-mkdocs/actions/workflows/deploy-mkdocs.yml/badge.svg)](https://github.com/LGLenz/eliaslenz-cybersecurity-phd-research-lab-mkdocs/actions/workflows/deploy-mkdocs.yml)

# Cybersecurity PhD Research Lab (MkDocs)

This repository is the **MkDocs + Material for MkDocs** documentation site for my part-time PhD in Cyber Security (University of Plymouth).

Focus area:

> **Human-centric policy-as-code (PaC) guardrails for PaaS/IaaS environments in regulated contexts (Germany–UK).**

## What’s in here

- **MkDocs site** under `docs/`
- **Static research artefacts** under `docs/papers/` (HTML preprint, CSV, BibTeX)
- **GitHub Actions deployment** workflow for GitHub Pages under `.github/workflows/`

## Local dev (quick start)

```bash
python -m venv .venv
# Windows: .venv\Scripts\activate
source .venv/bin/activate

pip install -r requirements.txt
mkdocs serve
```

Then open the local preview at `http://127.0.0.1:8000/`.

## Deploying to GitHub Pages

This repo is set up to deploy via **GitHub Actions** whenever you push to `main`.

1. In GitHub, go to **Settings → Pages**.
2. Under **Build and deployment**, select **Source: GitHub Actions**.
3. Push to `main`.

The published site URL for a repo named `eliaslenz-cybersecurity-phd-research-lab-mkdocs` under the org `elb-consulting-tech` is typically:

- `https://lglenz.github.io/eliaslenz-cybersecurity-phd-research-lab-mkdocs/`

## Repository layout

```text
.
├── .github/workflows/          # CI/CD (GitHub Pages deploy)
├── docs/                       # MkDocs content (Markdown + static files)
│   ├── index.md
│   ├── research/
│   ├── literature/
│   ├── methodology/
│   ├── artefacts/
│   ├── practice/
│   └── papers/                 # HTML/CSV/BibTeX served as static files
├── mkdocs.yml                  # Site configuration
├── requirements.txt            # Python deps for build
├── CONTRIBUTING.md
└── .gitignore
```

## Related (external) site

Some artefacts are also mirrored on the separate consulting site:

- https://lglenz.github.io/eliaslenz-secure-consulting/


## References (Zotero → BibTeX)

- Source of truth: Zotero collection
- Export to: `docs/references/library.bib`
- Cite in Markdown using keys like `[@Ali2025]`

## Governance & security

- Security reporting: see `SECURITY.md`
- Dependency updates: Dependabot weekly
