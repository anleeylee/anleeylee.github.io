---
layout: default
title: Anleey Lee — Estimating & Bioinformatics Tools
---

# Anleey Lee

**Developer of open-source desktop tools for estimating and bioinformatics** — Python CLI tooling around the [AsphaltCosts.com](https://asphaltcosts.com/) calculation engine (PDF/CAD quantity takeoff, specification checking, quote comparison, delivery-ticket reconciliation, audit-ready reports), TypeScript tooling around the [BoardFootCalc.net](https://boardfootcalc.net/) lumber calculator (cut-list optimization, tally auditing, cutting layouts, inventory, quote estimating), and local-first sequence analysis for [BioSyn](https://biosyn-inc.com/) (batch FASTA QC, GC%, molecular weight, pI).

## Featured project — Asphalt Desktop Intelligence

[**Asphalt Desktop Intelligence**](https://github.com/anleeylee/asphalt-desktop-intelligence) is a Python toolkit (scripts S01–S10) that turns plan PDFs, CAD drawings, specifications, contractor quotes, delivery tickets, supplier prices and site photos into **audit-ready asphalt estimates**.

- **Documentation site:** [anleeylee.github.io/asphalt-desktop-intelligence](https://anleeylee.github.io/asphalt-desktop-intelligence/) — architecture & per-script specifications
- **AsphaltCosts.com:** the deterministic calculation engine (area → compacted volume → net tons → order tons → truckloads → material cost)

## Standalone tools

Each business scenario ships as its own self-contained GitHub repository:

| Tool | What it does |
|---|---|
| [asphalt-pdf-plan-takeoff](https://github.com/anleeylee/asphalt-pdf-plan-takeoff) | Extract paving quantities (area, tons, truckloads) from civil plan PDFs |
| [asphalt-specification-checker](https://github.com/anleeylee/asphalt-specification-checker) | Structured specification requirements & plan/spec/bid conflict detection |
| [asphalt-quote-comparator](https://github.com/anleeylee/asphalt-quote-comparator) | Normalize contractor bids into comparable tables with $/SF, $/ton & scope flags |
| [asphalt-delivery-ticket-reconciler](https://github.com/anleeylee/asphalt-delivery-ticket-reconciler) | Reconcile asphalt delivery tickets against the estimate (CSV/PDF/photo) |
| [asphalt-supplier-quote-normalizer](https://github.com/anleeylee/asphalt-supplier-quote-normalizer) | Evidence-backed supplier material price datasets with validity windows |
| [asphalt-weather-compaction-planner](https://github.com/anleeylee/asphalt-weather-compaction-planner) | HMA cooling/compaction window planning from a lumped thermal model |
| [asphalt-field-photo-analyzer](https://github.com/anleeylee/asphalt-field-photo-analyzer) | Pavement distress screening (potholes, cracking, rutting) from site photos |
| [asphalt-estimate-report-builder](https://github.com/anleeylee/asphalt-estimate-report-builder) | Audit-ready estimate reports (JSON / Markdown / XLSX / PDF) |

## Woodworking & lumber — BoardFootCalc

[**boardfootcalc-cut-list-optimizer**](https://github.com/anleeylee/boardfootcalc-cut-list-optimizer) (`bfc-optimize`) turns a woodworking cut list into an optimized, **lowest-waste lumber purchase plan** — TypeScript CLI with board matching, existing-inventory reuse, kerf-aware placement, cost/waste/board-count strategies and printable purchase lists.

- **Live site:** [anleeylee.github.io/boardfootcalc-cut-list-optimizer](https://anleeylee.github.io/boardfootcalc-cut-list-optimizer/)
- **Lumber math source:** [BoardFootCalc.net](https://boardfootcalc.net/) — board foot calculators and guides

[**lumber-tally-auditor**](https://github.com/anleeylee/lumber-tally-auditor) (`bfc-audit`) audits lumber yard tallies and invoices line-by-line against 8 billing profiles — catch rounding overcharges and export a printable PDF audit report.

[**board-cutting-optimizer**](https://github.com/anleeylee/board-cutting-optimizer) generates real 2D guillotine cutting layouts for every board — grain, kerf and defect aware, with SVG / PDF cutting sheets and CSV exports.

[**lumber-inventory-manager**](https://github.com/anleeylee/lumber-inventory-manager) is an offline-first SQLite lumber inventory with a full transaction ledger — natural-language search, project allocation, consumption and automatic offcut re-entry.

[**quote-project-estimator**](https://github.com/anleeylee/quote-project-estimator) estimates lumber quotes from a cut list — net, gross and charged board feet, 8 billing profiles, species price lists, markup, tax and a shareable HTML quote.

- Companion tools in the same family (sharing one lumber calculation engine): tally & invoice auditing, 2D board cutting layouts, offline lumber inventory and quote/project estimating

## Bioinformatics — BioSyn

[**biosyn-fasta-batch-analyzer**](https://github.com/anleeylee/biosyn-fasta-batch-analyzer) is a **local-first batch FASTA sequence analyzer** for DNA, RNA and protein — Python CLI that computes GC%, length, base/amino-acid composition, molecular weight, reverse complement and isoelectric point (pI) across hundreds of sequences in one run, with PASS / REVIEW / INVALID quality-control classification and CSV / XLSX / HTML report export. All computation stays offline.

- **Online counterpart:** [BioSyn FASTA sequence analyzer](https://biosyn-inc.com/tools/fasta-sequence-analyzer) — single-sequence web tool

[**biosyn-primer-batch-qc**](https://github.com/anleeylee/biosyn-primer-batch-qc) is a **batch primer QC tool** — Tm, GC%, hairpin and dimer detection for thousands of primers from CSV/XLSX, fully offline Python CLI.

[**biosyn-qpcr-csv-analyzer**](https://github.com/anleeylee/biosyn-qpcr-csv-analyzer) is a **qPCR CSV analyzer** — dCt/ddCt/fold change, replicate QC and standard curves from instrument exports, fully offline Python CLI.

[**biosyn-serial-dilution-planner**](https://github.com/anleeylee/biosyn-serial-dilution-planner) is a **serial dilution planner** — multi-tube dilution schemes with pipetting volumes and safety checks, XLSX/CSV export, fully offline Python tool.

[**biosyn-solution-preparation**](https://github.com/anleeylee/biosyn-solution-preparation) is a **batch solution preparation calculator** — molar, stock dilution, mass concentration and percentage modes with purity correction, fully offline Python tool.

- Companion tools in the same family: multi-sequence alignment, primer design and genome feature analysis

## Why these tools

Manual takeoff, estimating and sequence analysis is slow and error-prone — in asphalt paving (dimensions hide inside PDF plans and CAD drawings, requirements hide in long specification documents, delivery tickets rarely match the estimate), in woodworking (cut lists waste board, dealer tallies go unchecked), and in the lab (web tools handle one sequence at a time; hundreds of FASTA records cannot be pasted by hand). Every tool follows the same principles:

- **Deterministic math** — numbers come from a documented engine or standard library, never re-implemented ad hoc
- **Evidence-backed values** — every result carries source, method, confidence and verification state
- **No silent fixes** — low-confidence values and conflicts land in a review queue
- **Audit-ready** — every run records inputs, hashes, version and outputs
- **Privacy-first** — local files and sequences stay local; nothing is uploaded by default

## About

This GitHub Pages profile aggregates open-source projects by Anleey Lee. All projects are MIT-licensed planning tools — they estimate, they never approve construction.
