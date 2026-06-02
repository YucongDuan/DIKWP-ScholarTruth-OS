# DIKWP ScholarTruth OS

**DIKWP ScholarTruth OS** is an offline-first, GitHub-ready research integrity triage system for academic fraud risk analysis, evidence-ledger construction, and responsible correction workflows.

It does **not** automatically accuse authors, journals, institutions, or papers of fraud. It produces structured **risk signals**, **evidence ledgers**, **claim cards**, **review queues**, and **human escalation packets**.

## Core idea

Academic integrity failures are often not a single defect but a semantic-space mismatch across:

- Data: figures, tables, raw data statements, p-values, identifiers.
- Information: metadata, author graph, citation graph, trial registration, retraction status.
- Knowledge: method norms, disciplinary standards, known paper-mill indicators.
- Wisdom: proportionality, due process, reputational harm, non-accusatory wording.
- Purpose: protect the scholarly record while avoiding wrongful public accusation.
- Reliability: source custody, review level, residuals, and kill/recovery conditions.

## Quick start

```bash
pip install -e .
scholartruth analyze examples/sample_integrity_case.json --out outputs/demo
scholartruth static-audit src --out outputs/demo/static_boundary_audit_report.json
```

Outputs include `scholartruth_report.json`, `integrity_signal_matrix.csv`, `claim_cards.csv`, `evidence_ledger.json`, `author_network_review.csv`, `correction_workflow.md`, and `responsible_inquiry_letter.md`.

## Boundary

Use this system for research integrity triage, editorial preparation, institutional review preparation, and evidence organization. Do not use it for automated public accusations, harassment, defamation, doxxing, or bypassing journal/institutional procedures.
