# Runtime exports

This directory contains the NeoMundi ControlTower runtime outputs generated for the **FactNotebook × NeoMundi PubMedQA interoperability pilot**.

## Pilot run

- **Model:** `gpt-4o-2024-11-20`
- **Workflow:** `stream_then_govern_v3`
- **Panel version:** `pubmedqa_mini_panel_5_cases_v1`
- **Cases:** `5`
- **Successful rows:** `5/5`
- **Error rows:** `0`

## Files

This directory contains:

- `results.jsonl` — structured runtime records used for downstream ingestion;
- `results.csv` — tabular representation of the runtime outputs;
- `summary.json` — run-level metadata and execution summary.

## Role in the pilot

These exports form the data surface consumed by FactNotebook after NeoMundi runtime measurement.

The integration flow is:

    AI generation
          ↓
    NeoMundi ControlTower
    runtime measurement
          ↓
    runtime export
          ↓
    FactNotebook
    evidence reconstruction

FactNotebook reported that the exported records could be ingested deterministically through its dedicated connector without manual reprocessing.

## Scope

The files expose runtime outputs and interoperability-relevant metadata required to inspect the pilot.

They do not expose NeoMundi's internal measurement mechanisms, proprietary implementation logic, or internal computation methods.
