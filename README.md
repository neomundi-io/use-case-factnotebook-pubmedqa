# FactNotebook × NeoMundi — Bounded evidence reconstruction

**Five runtime observations. One independent reconstruction. Separate authority.**

NeoMundi measured five requested GPT-4o generations on a PubMedQA mini-panel and exported the runtime records as JSONL. FactNotebook ingested those records and reconstructed what the available observations could support.

> **NeoMundi measures. FactNotebook reconstructs evidence. An accountable human authority decides.**

[Français](#version-française)

## Explore NeoMundi

[![Station — Observe & experiment](https://img.shields.io/badge/Station-Observe_%26_experiment-7c3aed?style=flat-square)](https://github.com/neomundi-io/neomundi-station-public)
[![Runtime Measurement — Measure & integrate](https://img.shields.io/badge/Runtime_Measurement-Measure_%26_integrate-2563eb?style=flat-square)](https://github.com/neomundi-io/neomundi-runtime-measurement)
[![Use Cases — Applications, pilots & evidence](https://img.shields.io/badge/Use_Cases-Applications%2C_pilots_%26_evidence-059669?style=flat-square)](https://github.com/neomundi-io/neomundi-use-cases)
[![Create an Account — ControlTower](https://img.shields.io/badge/Create_an_Account-ControlTower-ea580c?style=flat-square)](https://controltower.neomundi.io/welcome)

# English

## At a glance

| Question | Answer |
| --- | --- |
| What did NeoMundi measure? | Runtime behavior for five requested GPT-4o-2024-11-20 generations on a five-case PubMedQA mini-panel. |
| What was exported? | Five successful JSONL runtime records; zero error rows were recorded. |
| What did FactNotebook do? | It ingested the export and produced an independent retrospective evidence reconstruction. |
| Who decides? | Neither measurement nor reconstruction grants authority. The accountable human authority decides. |
| Status | Completed, bounded historical interoperability experiment. Further replication is required. |

## Historical experiment

The preserved run used five PubMedQA cases, requested model GPT-4o-2024-11-20, workflow **stream_then_govern_v3**, and CSV/JSONL exports. Five rows were saved successfully and no error row was recorded. The artifact name dates the run to 25 July 2026.

The requested model identity was declared but not independently confirmed. This repository preserves the experiment as run; it does not retroactively apply later RGC contracts or semantics.

## Responsibility boundaries

| Layer | Responsibility |
| --- | --- |
| AI system | Produces the generation. |
| NeoMundi | Measures and reports runtime behavior. |
| FactNotebook | Reconstructs what the available observations permit a third party to establish. |
| Accountable human authority | Interprets the evidence and makes any assurance or governance decision. |

## What the five observations demonstrate

Within this experiment, the public artifacts show that five NeoMundi runtime records were produced, associated with the five panel cases and exported as JSONL. The dedicated FactNotebook integration consumed that export without reproducing NeoMundi's measurement function. Both systems retained separate functions and authority.

This demonstrates a bounded interoperability path—not universal interoperability, measurement validity or production readiness.

## What the partner reconstruction adds

FactNotebook published the specific entry [**FN-NEOMUNDI-CTPUBMEDQA-001**](https://github.com/factnotebook/public-reconstructions/tree/main/FN-NEOMUNDI-CTPUBMEDQA-001).

It adds a retrospective declared-versus-observed reconstruction, preserves **NOT ASSESSABLE** when no observation channel exists, publishes SHA-256 commitments for non-public package content, and provides RFC-3161 timestamp tokens for the ingest boundary and manifest.

FactNotebook's historical **8/9 (89%) evidentiary-weight estimate** belongs to FactNotebook's reconstruction methodology. It is not a NeoMundi metric, score or measurement result. The linked entry—not the whole partner registry—is the relevant partner evidence.

## Inspectable evidence

### NeoMundi repository

- [Five-case panel](./data/panel/)
- [Runtime exports](./data/runtime/)
- [Run summary](./data/runtime/openai_gpt-4o-2024-11-20_factnotebook_pubmedqa_pilot_v01_20260725T181548Z_summary.json)
- [Integration feedback](./docs/neomundi_pilot_integration_feedback.pdf)
- [Data guide](./data/README.md)
- [Documentation guide](./docs/README.md)

### Partner entry

The partner entry exposes its README, manifest, SHA256SUMS, and the **ingest.tsr** and **manifest.tsr** RFC-3161 tokens. It publishes reconstruction outputs and commitments, not its reconstruction engine, models or reading rules. The complete FactNotebook reconstruction therefore cannot be rerun independently from the published materials.

## Integrity and timestamp limits

The partner manifest is explicitly **unsigned**. Hashes of non-public artifacts are commitments, not disclosures. RFC-3161 attests that a blob existed at a time—not what it means or whether its claims are true. The published package establishes neither immutability nor counter-signature, and its stated integrity begins only from generation time.

## What this does not establish

The pilot does not establish medical truth, general model validity, independent confirmation of every metadata field, universal validity of NeoMundi measurements, independent reproducibility of FactNotebook's reconstruction, certification, regulatory compliance, assurance, production readiness, or execution permission. Later RGC contracts are not applied retroactively.

## Reports

- [Partner reconstruction entry](https://github.com/factnotebook/public-reconstructions/tree/main/FN-NEOMUNDI-CTPUBMEDQA-001)
- [Public report — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/)
- [Rapport public — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/index.fr.html)
- [Detailed review — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.html)
- [Revue détaillée — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.fr.html)

---

# Version française

## En bref

| Question | Réponse |
| --- | --- |
| Qu'a mesuré NeoMundi ? | Le comportement runtime de cinq générations demandées à GPT-4o-2024-11-20 sur un mini-panel PubMedQA de cinq cas. |
| Qu'est-ce qui a été exporté ? | Cinq enregistrements runtime JSONL réussis ; aucune ligne en erreur n'a été enregistrée. |
| Qu'a fait FactNotebook ? | FactNotebook a ingéré l'export et produit une reconstruction rétrospective indépendante de la preuve. |
| Qui décide ? | Ni la mesure ni la reconstruction n'accordent d'autorité. L'autorité humaine responsable décide. |
| Statut | Expérience historique d'interopérabilité terminée et bornée. Des réplications restent nécessaires. |

## Expérience historique

Le run conservé utilisait cinq cas PubMedQA, le modèle demandé GPT-4o-2024-11-20, le workflow **stream_then_govern_v3**, et des exports CSV/JSONL. Cinq lignes ont été sauvegardées avec succès et aucune ligne en erreur n'a été enregistrée. Le nom de l'artefact date le run du 25 juillet 2026.

L'identité du modèle demandé était déclarée mais n'a pas été confirmée indépendamment. Ce dépôt conserve l'expérience telle qu'elle a été exécutée ; il ne lui applique pas rétroactivement les contrats ou la sémantique RGC ultérieurs.

## Frontières de responsabilité

| Couche | Responsabilité |
| --- | --- |
| Système IA | Produit la génération. |
| NeoMundi | Mesure et rapporte le comportement runtime. |
| FactNotebook | Reconstruit ce que les observations disponibles permettent à un tiers d'établir. |
| Autorité humaine responsable | Interprète les preuves et prend toute décision d'assurance ou de gouvernance. |

## Ce que démontrent les cinq observations

Dans cette expérience, les artefacts publics montrent que cinq enregistrements runtime NeoMundi ont été produits, associés aux cinq cas du panel et exportés en JSONL. L'intégration FactNotebook dédiée a consommé cet export sans reproduire la fonction de mesure NeoMundi. Les deux systèmes ont conservé des fonctions et une autorité distinctes.

Cela démontre un chemin d'interopérabilité borné, et non une interopérabilité universelle, une validité générale de la mesure ou une préparation à la production.

## Ce qu'ajoute la reconstruction partenaire

FactNotebook a publié l'entrée précise [**FN-NEOMUNDI-CTPUBMEDQA-001**](https://github.com/factnotebook/public-reconstructions/tree/main/FN-NEOMUNDI-CTPUBMEDQA-001).

Elle ajoute une reconstruction rétrospective confrontant le déclaré et l'observé, conserve **NOT ASSESSABLE** en l'absence de canal d'observation, publie des engagements SHA-256 pour le contenu non public du paquet et fournit des jetons RFC-3161 pour la frontière d'ingestion et le manifeste.

L'estimation historique **8/9 (89 %) du poids probatoire** appartient à la méthodologie de reconstruction FactNotebook. Ce n'est ni une métrique, ni un score, ni un résultat de mesure NeoMundi. L'entrée liée, et non l'ensemble du registre partenaire, constitue la preuve partenaire pertinente.

## Preuves examinables

### Dépôt NeoMundi

- [Panel de cinq cas](./data/panel/)
- [Exports runtime](./data/runtime/)
- [Résumé du run](./data/runtime/openai_gpt-4o-2024-11-20_factnotebook_pubmedqa_pilot_v01_20260725T181548Z_summary.json)
- [Retour d'intégration](./docs/neomundi_pilot_integration_feedback.pdf)
- [Guide des données](./data/README.md)
- [Guide documentaire](./docs/README.md)

### Entrée partenaire

L'entrée expose son README, son manifeste, SHA256SUMS et les jetons RFC-3161 **ingest.tsr** et **manifest.tsr**. Elle publie les sorties et engagements de la reconstruction, pas son moteur, ses modèles ou ses règles de lecture. La reconstruction FactNotebook complète ne peut donc pas être réexécutée indépendamment à partir des seuls matériaux publiés.

## Limites d'intégrité et d'horodatage

Le manifeste partenaire est explicitement **non signé**. Les hash d'artefacts non publics sont des engagements, pas des divulgations. RFC-3161 atteste qu'un blob existait à un instant, et non ce qu'il signifie ou si ses affirmations sont vraies. Le paquet publié n'établit ni immutabilité ni contre-signature, et son intégrité déclarée ne commence qu'au moment de la génération.

## Ce que cela n'établit pas

Le pilote n'établit ni vérité médicale, ni validité générale du modèle, ni confirmation indépendante de chaque métadonnée, ni validité universelle des mesures NeoMundi, ni reproductibilité indépendante de la reconstruction FactNotebook, ni certification, conformité réglementaire, assurance, préparation à la production ou permission d'exécution. Les contrats RGC ultérieurs ne sont pas appliqués rétroactivement.

## Rapports

- [Entrée de reconstruction partenaire](https://github.com/factnotebook/public-reconstructions/tree/main/FN-NEOMUNDI-CTPUBMEDQA-001)
- [Public report — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/)
- [Rapport public — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/index.fr.html)
- [Detailed review — English](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.html)
- [Revue détaillée — Français](https://factnotebook.com/audits/neomundi/neomundi-controltower-pubmedqa-pilot-v01/review.fr.html)
