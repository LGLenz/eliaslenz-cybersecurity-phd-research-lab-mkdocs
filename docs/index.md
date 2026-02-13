# Cybersecurity PhD Research Lab

Welcome to the documentation hub for my part-time PhD in Cyber Security
(University of Plymouth).

The overarching theme is:

> **Human-centric policy-as-code (PaC) guardrails for PaaS/IaaS environments
> in regulated contexts (Germany–UK).**

This site tracks:

- the current **research questions**
- **literature review** strands and mapping work
- **methodology and design** decisions
- early **prototypes and tooling**
- how these ideas are explored in a small, real-world **consulting practice**

---

## Quick links

- [Research questions](research/questions.md)
- [Literature review](literature/index.md)
- [Methodology & design](methodology/index.md)
- [Prototypes & tooling](artefacts/prototypes.md)
- [Consulting bridge](practice/consulting-bridge.md)

> **Preprint 1 – CPS cybersecurity (HTML)**
>
> - Local copy in this repo/site: [Open](papers/preprint-1.html)
> - External copy (consulting site):
>   https://elb-consulting-tech.github.io/eliaslenz-secure-consulting/papers/preprint-1.html

---

## Relation to practice

Alongside this PhD, I work full-time in the German public sector as an IT
coordinator and information security practitioner, and run a small, research-
aligned freelance practice:

- **Freelance consulting site:**
  https://elb-consulting-tech.github.io/eliaslenz-secure-consulting/

That site hosts:

- a public, anonymised **sample dashboard ("SecureLaunch WebHub")**
- the **HTML preprint** linked above
- descriptions of focused consulting services

The aim is to maintain a feedback loop between research questions and the
constraints of real systems and organisations.


## How to cite

This repository includes a `CITATION.cff` file (GitHub will show “Cite this repository”).
For page-level citations, use Zotero → BibTeX (`docs/references/library.bib`) and cite in Markdown like `[@Ali2025]`.

## Reproducible build

- Local: `pip install -r requirements.txt` then `mkdocs serve`
- CI: GitHub Actions builds with `mkdocs build --strict`
