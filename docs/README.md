# Documentation

Supporting documentation for the **FactNotebook × NeoMundi PubMedQA interoperability pilot**.

[🇫🇷 Lire en français](#version-française)

---

## English

### Integration feedback

This directory contains supporting documentation related to the completed interoperability pilot between **NeoMundi ControlTower** and **FactNotebook**.

The main document is:

- `neomundi_pilot_integration_feedback.pdf`

It contains FactNotebook's technical feedback on the NeoMundi ControlTower runtime export used during the PubMedQA pilot.

### Covered topics

The document addresses:

- JSONL structure and ingestion;
- deterministic integration through a dedicated connector;
- traceability of individual generations;
- useful runtime signals and metadata;
- remaining ambiguities in field semantics;
- the role of independent runtime measurement;
- separation between runtime observation, evidence reconstruction and final assurance authority;
- limitations identified during the experiment;
- requirements for stronger versioned interoperability.

### Responsibility separation

The pilot documents three distinct functions:

**NeoMundi ControlTower**  
→ produces and reports runtime behavioral observations.

**FactNotebook**  
→ consumes available observations and reconstructs evidence and governance objects under a declared policy.

**Human authority**  
→ retains the final assurance decision.

The runtime measurement is therefore an observation layer, not a final verdict.

### Scope

This documentation describes the **integration experience, exported data surface and downstream reconstruction**.

It does not disclose NeoMundi's internal measurement mechanisms, proprietary implementation logic or internal computation methods.

### Related resources

- [FactNotebook public report — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/)
- [FactNotebook public report — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/index.fr.html)
- [Detailed evidence review — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.html)
- [Revue détaillée — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.fr.html)

---

# Version française

[🇬🇧 Back to English](#english)

## Retour d'intégration

Ce dossier contient la documentation associée au pilote d'interopérabilité terminé entre **NeoMundi ControlTower** et **FactNotebook**.

Le document principal est :

- `neomundi_pilot_integration_feedback.pdf`

Il contient le retour technique de FactNotebook sur l'export runtime NeoMundi ControlTower utilisé pendant le pilote PubMedQA.

## Points documentés

Le document traite notamment :

- de la structure JSONL et de son ingestion ;
- de l'intégration déterministe via un connecteur dédié ;
- de la traçabilité des générations individuelles ;
- des signaux runtime et métadonnées les plus utiles ;
- des ambiguïtés restantes dans la sémantique de certains champs ;
- du rôle d'une mesure runtime indépendante ;
- de la séparation entre observation runtime, reconstruction d'évidence et autorité finale d'assurance ;
- des limites identifiées pendant l'expérience ;
- des besoins liés à une interopérabilité versionnée plus robuste.

## Séparation des responsabilités

Le pilote documente trois fonctions distinctes :

**NeoMundi ControlTower**  
→ produit et rapporte des observations comportementales runtime.

**FactNotebook**  
→ consomme les observations disponibles et reconstruit des objets de preuve et de gouvernance sous politique déclarée.

**Autorité humaine**  
→ conserve la décision finale d'assurance.

La mesure runtime constitue donc une couche d'observation, et non un verdict final.

## Périmètre

Cette documentation décrit **l'expérience d'intégration, la surface de données exportée et la reconstruction réalisée en aval**.

Elle ne décrit pas les mécanismes internes de mesure de NeoMundi, sa logique d'implémentation propriétaire ni ses méthodes internes de calcul.

## Ressources associées

- [Rapport public — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/)
- [Rapport public — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/index.fr.html)
- [Detailed evidence review — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.html)
- [Revue détaillée — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.fr.html)
