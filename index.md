---
layout: default
title: Anleey Lee — Asphalt & Construction Estimating Tools
---

# Anleey Lee

**Developer of open-source desktop estimating tools for the asphalt & paving industry** — Python CLI tooling built around the [AsphaltCosts.com](https://asphaltcosts.com/) calculation engine: PDF/CAD quantity takeoff, specification checking, contractor quote comparison, delivery-ticket reconciliation and audit-ready estimate reports.

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

## Why these tools

Manual asphalt takeoff is slow and error-prone: dimensions hide inside PDF plans and CAD drawings, requirements hide in long specification documents, and delivery tickets rarely match the estimate. Every tool follows the same principles:

- **Deterministic math** — tons, volume, coverage, truckloads and material cost come from the AsphaltCosts engine, never re-implemented
- **Evidence-backed values** — every number carries source, method, confidence and verification state
- **No silent fixes** — low-confidence values and conflicts land in a review queue
- **Audit-ready** — every run records inputs, hashes, engine version and outputs

## About

This GitHub Pages profile aggregates open-source projects by Anleey Lee. All projects are MIT-licensed planning tools — they estimate, they never approve construction.
