# Data

This directory contains the input panel and NeoMundi runtime exports associated with the **FactNotebook × NeoMundi PubMedQA interoperability pilot**.

## Structure

    data/
    ├── README.md
    ├── panel/
    │   └── pubmedqa_mini_panel_5_cases.csv
    └── runtime/
        ├── results.jsonl
        ├── results.csv
        └── summary.json

## Panel

The `panel/` directory contains the **5 PubMedQA cases** used in the pilot.

## Runtime exports

The `runtime/` directory contains the NeoMundi ControlTower outputs generated during the experiment.

The pilot run used:

- **Model:** `gpt-4o-2024-11-20`
- **Workflow:** `stream_then_govern_v3`
- **Panel version:** `pubmedqa_mini_panel_5_cases_v1`
- **Successful rows:** `5/5`
- **Error rows:** `0`

The runtime exports include the experiment outputs used for the FactNotebook integration and subsequent evidence reconstruction.

## Purpose

These files are published to make the documented interoperability experiment inspectable and to support independent review of the pilot.

They allow a third party to examine:

- the input panel used for the experiment;
- the runtime records produced by NeoMundi;
- the structured summary of the run;
- the data surface consumed by the downstream FactNotebook integration.

## Scope

The files expose experiment inputs, outputs and interoperability-relevant fields.

They do **not** expose NeoMundi's internal measurement mechanisms, proprietary implementation logic, or internal computation methods.

## Related resources

- [FactNotebook public report — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/)
- [FactNotebook public report — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/index.fr.html)
- [Detailed evidence review — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.html)
- [Revue détaillée — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.fr.html)
