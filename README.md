# FactNotebook × NeoMundi

**Independent evidence reconstruction from NeoMundi runtime measurements — PubMedQA pilot.**

[🇫🇷 Lire en français](#version-française)

---

# English

## What happened here?

NeoMundi measured the runtime behavior of **5 GPT-4o generations on PubMedQA**.

Those runtime observations were exported in JSONL and independently ingested by **FactNotebook**, which used them to reconstruct evidence objects.

### What this shows

This pilot provides evidence that:

- a third-party infrastructure can consume NeoMundi runtime measurements;
- the downstream system does not need to reproduce NeoMundi's measurement function;
- NeoMundi and FactNotebook can remain technically and functionally independent;
- runtime observations can become an independent evidence source for downstream governance.

**In simple terms: NeoMundi measures. FactNotebook reconstructs evidence. A human authority decides.**

FactNotebook's role is described here in terms of **evidence and evidence objects**, with assurance remaining a distinct downstream decision layer.

This is a completed interoperability pilot, not a claim of universal interoperability.

---

## Overview

This repository documents a completed interoperability pilot between **NeoMundi ControlTower** and **FactNotebook**.

The experiment examines whether runtime observations produced by NeoMundi can be consumed by an independent third-party infrastructure to reconstruct evidence objects while preserving a clear separation of responsibilities.

The pilot covers **5 PubMedQA generations produced with GPT-4o-2024-11-20**.

## Architecture

    AI generation
          ↓
    NeoMundi ControlTower
    runtime measurement
          ↓
    JSONL export
          ↓
    FactNotebook
    evidence reconstruction
          ↓
    assurance interpretation
          ↓
    human authority

**NeoMundi measures runtime behavior.**

**FactNotebook reconstructs what a third party can legitimately establish from the available observations.**

The final assurance decision remains outside both measurement and evidence reconstruction.

## Use case

FactNotebook reconstructs evidence and assurance objects from available evidence.

Without an independent runtime source, this reconstruction would rely primarily on information reported by the system being evaluated.

In this pilot, NeoMundi supplied runtime observations that FactNotebook could ingest as an independent evidence source.

The objective was not to merge both infrastructures, but to test whether they could interoperate while retaining distinct functions and responsibilities.

## Experiment

- **Partner infrastructure:** FactNotebook
- **Measurement layer:** NeoMundi ControlTower
- **Dataset:** PubMedQA mini-panel
- **Model:** GPT-4o-2024-11-20
- **Cases:** 5
- **Workflow:** `stream_then_govern_v3`
- **Successful observations:** 5 / 5
- **Error rows:** 0
- **Export format:** JSONL
- **Integration:** dedicated FactNotebook connector

The JSONL export contained runtime signals, runtime outputs, trace identifiers, timestamps and associated metadata.

FactNotebook reported that ingestion was deterministic and required no manual reprocessing.

## Responsibility separation

| Layer | Responsibility |
|---|---|
| AI system | Produces the generation |
| NeoMundi | Measures and reports runtime behavior |
| FactNotebook | Reconstructs evidence objects |
| Human authority | Makes the final assurance decision |

Runtime measurement reports what was observed.

It does not, by itself, constitute a final verdict.

## Observed interoperability

The pilot showed that:

- NeoMundi runtime exports could be ingested by an independent infrastructure;
- observations could be associated with individual generations;
- FactNotebook could reconstruct evidence objects without producing the runtime measurements itself;
- NeoMundi and FactNotebook retained distinct functional roles;
- runtime observations could contribute an independent evidence source beyond model self-reporting.

FactNotebook estimated that **8/9 (89%) of the evidentiary weight** used in its reconstruction came from an independent witness rather than model self-reporting.

## Concrete example

A NeoMundi overclaim flag was consumed by FactNotebook as an independent runtime observation.

FactNotebook used this observation when reconstructing an Article 15-related governance tension without implementing its own runtime detector.

> **NeoMundi produces behavioral observations. FactNotebook transforms observations into evidence objects.**

## What this pilot does — and does not — establish

### It establishes, within this experiment

- successful ingestion of NeoMundi runtime exports by FactNotebook;
- deterministic downstream processing without manual reprocessing;
- preservation of distinct functional responsibilities;
- use of NeoMundi runtime observations as an independent evidentiary source;
- technical articulation between measurement and downstream evidence reconstruction.

### It does not establish

- universal interoperability across all infrastructures;
- universal validity of the NeoMundi measurement layer;
- independent confirmation of every metadata field;
- a final assurance verdict produced by NeoMundi;
- generalisation beyond this pilot without further replication.

## Limitations

The experiment identified several limitations:

- model identity was declared but not independently confirmed;
- some field semantics still required interpretation;
- `severity`, `category` and certain thresholds required clearer documentation;
- no downstream human-supervision event was included in the runtime export;
- some timestamps could be absent;
- a versioned interoperability schema was still required at the time of the pilot.

The pilot should therefore be interpreted as a completed integration experiment requiring further replication before broader generalisation.

## Repository contents

    .
    ├── README.md
    ├── data/
    │   ├── README.md
    │   ├── panel/
    │   │   ├── README.md
    │   │   └── PubMedQA pilot input files
    │   └── runtime/
    │       ├── README.md
    │       ├── results.csv
    │       ├── results.jsonl
    │       └── summary.json
    └── docs/
        ├── README.md
        └── neomundi_pilot_integration_feedback.pdf

The repository is intended to make the experiment **inspectable**, not to expose NeoMundi's proprietary internal measurement mechanisms.

## Public reports

### FactNotebook

**Patrick Juvet Etoua** — Researching evidence-based AI governance. Building FactNotebook. Author of Governance Falsifiability Infrastructure.  
[LinkedIn](https://www.linkedin.com/in/patrick-juvet-etoua-697847a3/)

- [Public report — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/)
- [Public report — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/index.fr.html)
- [Detailed evidence review — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.html)
- [Revue détaillée — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.fr.html)

### NeoMundi

- [NeoMundi Research](https://neomundi.org)
- [ControlTower](https://controltower.neomundi.io/welcome)
- [Runtime Interoperability Contract](https://github.com/neomundi-io/runtime-interoperability-contract)
- [NeoMundi AI Observatory](https://github.com/neomundi-io/neomundi-ai-observatory)

## Status

**Completed and publicly documented interoperability pilot.**

The results provide evidence that an independent third-party infrastructure can consume NeoMundi runtime observations while both systems retain their own architecture, function and authority.

Further replication is required before broader generalisation.

---

# Version française

[🇬🇧 Back to English](#english)

## Qu’est-ce qui a été fait ici ?

NeoMundi a mesuré le comportement runtime de **5 générations GPT-4o sur PubMedQA**.

Ces observations runtime ont été exportées en JSONL puis ingérées indépendamment par **FactNotebook**, qui les a utilisées pour reconstruire des objets de preuve.

### Ce que cela montre

Ce pilote apporte des éléments montrant que :

- une infrastructure tierce peut consommer les mesures runtime NeoMundi ;
- le système en aval n’a pas besoin de reproduire la fonction de mesure de NeoMundi ;
- NeoMundi et FactNotebook peuvent rester techniquement et fonctionnellement indépendants ;
- les observations runtime peuvent devenir une source de preuve indépendante pour des fonctions de gouvernance en aval.

**En termes simples : NeoMundi mesure. FactNotebook reconstruit la preuve. Une autorité humaine décide.**

Le rôle de FactNotebook est décrit ici en termes de **preuve et d’objets de preuve**, l’assurance restant une couche de décision distincte en aval.

Il s’agit d’un pilote d’interopérabilité terminé, et non d’une démonstration d’interopérabilité universelle.

---

## Vue d’ensemble

Ce dépôt documente un pilote d’interopérabilité terminé entre **NeoMundi ControlTower** et **FactNotebook**.

L’expérience examine si des observations runtime produites par NeoMundi peuvent être consommées par une infrastructure tierce indépendante afin de reconstruire des objets de preuve, tout en maintenant une séparation claire des responsabilités.

Le pilote porte sur **5 générations PubMedQA produites avec GPT-4o-2024-11-20**.

## Architecture

    Génération IA
          ↓
    NeoMundi ControlTower
    mesure runtime
          ↓
    export JSONL
          ↓
    FactNotebook
    reconstruction d’évidence
          ↓
    interprétation d’assurance
          ↓
    autorité humaine

**NeoMundi mesure le comportement runtime.**

**FactNotebook reconstruit ce qu’un tiers peut légitimement établir à partir des observations disponibles.**

La décision finale d’assurance reste distincte de la mesure et de la reconstruction d’évidence.

## Cas d’usage

FactNotebook reconstruit des objets de preuve et d’assurance à partir des éléments de preuve disponibles.

Sans source runtime indépendante, cette reconstruction reposerait principalement sur les informations déclarées par le système évalué.

Dans ce pilote, NeoMundi a fourni des observations runtime que FactNotebook a pu ingérer comme source d’information indépendante.

L’objectif n’était pas de fusionner les deux infrastructures, mais de tester leur capacité à s’articuler tout en conservant des fonctions et responsabilités distinctes.

## Expérience

- **Infrastructure partenaire :** FactNotebook
- **Couche de mesure :** NeoMundi ControlTower
- **Dataset :** mini-panel PubMedQA
- **Modèle :** GPT-4o-2024-11-20
- **Cas :** 5
- **Workflow :** `stream_then_govern_v3`
- **Observations réussies :** 5 / 5
- **Lignes en erreur :** 0
- **Format d’export :** JSONL
- **Intégration :** connecteur FactNotebook dédié

L’export JSONL contenait des signaux runtime, des sorties runtime, des identifiants de trace, des horodatages et les métadonnées associées.

FactNotebook indique que l’ingestion a été déterministe et n’a nécessité aucun retraitement manuel.

## Séparation des responsabilités

| Couche | Responsabilité |
|---|---|
| Système IA | Produit la génération |
| NeoMundi | Mesure et rapporte le comportement runtime |
| FactNotebook | Reconstruit des objets de preuve |
| Autorité humaine | Prend la décision finale d’assurance |

La mesure runtime rapporte ce qui a été observé.

Elle ne constitue pas, à elle seule, un verdict final.

## Interopérabilité observée

Le pilote montre que :

- les exports runtime NeoMundi ont pu être ingérés par une infrastructure indépendante ;
- les observations ont pu être rattachées à des générations individuelles ;
- FactNotebook a pu reconstruire des objets de preuve sans produire lui-même les mesures runtime ;
- NeoMundi et FactNotebook ont conservé des rôles fonctionnels distincts ;
- les observations runtime ont pu constituer une source d’information indépendante au-delà de l’auto-déclaration du modèle.

FactNotebook estime que **8/9 (89 %) du poids probatoire** utilisé dans sa reconstruction provenait d’un témoin indépendant plutôt que de l’auto-déclaration du modèle.

## Exemple concret

Un flag NeoMundi de sur-affirmation a été consommé par FactNotebook comme observation runtime indépendante.

FactNotebook a utilisé cette observation pour reconstruire une tension liée à l’Article 15 sans implémenter son propre détecteur runtime.

> **NeoMundi produit des observations comportementales. FactNotebook transforme ces observations en objets de preuve.**

## Ce que ce pilote établit — et n’établit pas

### Il établit, dans le périmètre de cette expérience

- l’ingestion réussie des exports runtime NeoMundi par FactNotebook ;
- un traitement aval déterministe sans retraitement manuel ;
- le maintien de responsabilités fonctionnelles distinctes ;
- l’utilisation des observations runtime NeoMundi comme source probatoire indépendante ;
- une articulation technique entre mesure et reconstruction de preuve en aval.

### Il n’établit pas

- une interopérabilité universelle entre toutes les infrastructures ;
- une validité universelle de la couche de mesure NeoMundi ;
- la confirmation indépendante de chaque métadonnée ;
- un verdict final d’assurance produit par NeoMundi ;
- une généralisation au-delà de ce pilote sans réplications supplémentaires.

## Limites

L’expérience a identifié plusieurs limites :

- l’identité du modèle était déclarée mais non confirmée indépendamment ;
- certains champs nécessitaient encore une interprétation ;
- la sémantique de `severity`, `category` et de certains seuils nécessitait une documentation plus explicite ;
- aucun événement de supervision humaine en aval n’était inclus dans l’export runtime ;
- certains horodatages pouvaient être absents ;
- un schéma d’interopérabilité versionné restait nécessaire au moment du pilote.

Le pilote doit donc être interprété comme une expérience d’intégration terminée nécessitant des réplications supplémentaires avant toute généralisation plus large.

## Contenu du dépôt

    .
    ├── README.md
    ├── data/
    │   ├── README.md
    │   ├── panel/
    │   │   ├── README.md
    │   │   └── fichiers d’entrée du pilote PubMedQA
    │   └── runtime/
    │       ├── README.md
    │       ├── results.csv
    │       ├── results.jsonl
    │       └── summary.json
    └── docs/
        ├── README.md
        └── neomundi_pilot_integration_feedback.pdf

Le dépôt vise à rendre l’expérience **inspectable**, sans exposer les mécanismes internes propriétaires de mesure de NeoMundi.

## Rapports publics

### FactNotebook

**Patrick Juvet Etoua** — Researching evidence-based AI governance. Building FactNotebook. Author of Governance Falsifiability Infrastructure.  
[LinkedIn](https://www.linkedin.com/in/patrick-juvet-etoua-697847a3/)

- [Rapport public — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/)
- [Rapport public — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/index.fr.html)
- [Detailed evidence review — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.html)
- [Revue détaillée — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.fr.html)

### NeoMundi

- [NeoMundi Research](https://neomundi.org)
- [ControlTower](https://controltower.neomundi.io/welcome)
- [Runtime Interoperability Contract](https://github.com/neomundi-io/runtime-interoperability-contract)
- [NeoMundi AI Observatory](https://github.com/neomundi-io/neomundi-ai-observatory)

## Statut

**Pilote d’interopérabilité terminé et documenté publiquement.**

Les résultats apportent des éléments montrant qu’une infrastructure tierce indépendante peut consommer des observations runtime NeoMundi tout en maintenant, de part et d’autre, une architecture, une fonction et une autorité distinctes.

Des réplications supplémentaires sont nécessaires avant toute généralisation plus large.
