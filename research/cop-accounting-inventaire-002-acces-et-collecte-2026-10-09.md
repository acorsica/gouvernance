---
title: "COP Accounting — INV-002, frontières d'accès et plan de collecte"
date: "2026-10-09"
language: fr
document_role: operational
document_kind: continuation-report
visibility: public
lifecycle_state: working
status: working-paper
update_policy: UP-DEFAULT-REVIEWED
review:
  status: unreviewed
  reviewed_by: []
provenance:
  origin_type: repository-inspection
  origin_date: "2026-10-09"
  derived_from:
    - "https://github.com/acorsica/gouvernance/issues/2"
    - "https://github.com/JeanHuguesRobert/inseme/issues/120"
    - "https://github.com/JeanHuguesRobert/inseme/issues/121"
---

# INV-002 — Recherche, frontière d'accès et collecte contrôlée

## Réalisation observée

Inspection des racines des dépôts [gouvernance](https://github.com/acorsica/gouvernance), [acorsica.org](https://github.com/acorsica/acorsica.org), [institut-mariani](https://github.com/acorsica/institut-mariani) et des fichiers d'orientation du corpus au 9 octobre 2026.

Des documents **institutionnels** sont accessibles, notamment [identité administrative](https://github.com/acorsica/gouvernance/blob/main/identite-administrative.md), [état du corpus](https://github.com/acorsica/gouvernance/blob/main/etat-du-corpus.md), [cartographie](https://github.com/acorsica/gouvernance/blob/main/cartographie-du-corpus.md). Aucun relevé bancaire, journal comptable, facture ou balance **réellement examiné** dans cette passe. Cela n'atteste ni leur absence réelle, ni leur indisponibilité ailleurs, ni l'absence de comptabilité.

## Classement des besoins : source / accès / décision

| Identifiant | Élément demandé | Statut de preuve à ce stade | Mode de collecte proposé |
|---|---|---|---|
| COL-01 | Statuts à jour, déclaration, PV et délégations financières | Documents signés non examinés | Pièces signées avec dates et décisions, accès contrôlé |
| COL-02 | Exercice(s), plan comptable, grand livre, balance, comptes approuvés | Aucun fichier comptable lu | Exports natifs du logiciel comptable avec empreinte et provenance |
| COL-03 | Inventaire des comptes bancaires et relevés complets par exercice | Aucun accès bancaire ; non examiné | Transmission sécurisée de relevés, jamais dans GitHub public |
| COL-04 | Factures émises/reçues, avoirs, paiements, dépenses | Pièces non examinées | Registre pièce-ID / date / montant / émetteur / contrepartie / projet |
| COL-05 | Dons, cotisations, subventions, conventions, ressources affectées | Pièces non examinées | Distinguer engagement, encaissement et affectation imposée |
| COL-06 | Dettes, créances, charges à payer, produits à recevoir | Soldes non examinés | Échéanciers et preuves, sans solde présumé |
| COL-07 | Actifs immobilisés, contrats, valorisations | Pièces non examinées | Inventaire, titre, prix, amortissement ou règle applicable |
| COL-08 | Affectations analytiques liées à Barons Mariani | Aucune transaction attribuable vérifiée | Preuve de rattachement associatif et autorisation |
| COL-09 | Statut fiscal et obligations légales de C.O.R.S.I.C.A. | Régime non qualifié | Examen statuts, activités réelles, situation administrative, avis professionnel |

## Schéma minimal d'entrée, sans ingestion réelle

Pour toute pièce comptable, stocker séparément : `source_id`, `legal_entity_id`, `period`, `source_type`, `record_date`, `content_sha256`, `access_class`, `retrieval_ref`, `verified_by`, `verification_status`, `analytic_project_id` (facultatif), `related_decision_ref` (si pertinent). La référence publique ne doit pas révéler le contenu privé.

Pour toute opération, ajouter `amount_exact`, `currency`, `accounting_entry_ref`, `settlement_ref`, `reconciliation_status`, `exception_ids` ; valeurs inconnues **nulles/inconnues, jamais inventées**. Les références à un document constituent des indices, pas une preuve de validation.

## Contrôles avant traitement des données réelles

- Établir l'autorité et la base d'accès ; désigner la personne habilitée à transmettre.
- Protéger les données bancaires et personnelles ; éviter toute publication de données réelles sur GitHub public.
- Conserver copie originale, empreinte de contenu, historique des imports, provenance et contrôle des doublons.
- Projeter les anomalies séparément, sans écriture corrective non autorisée.
- Ne produire de comptes définitifs qu'après qualification de l'entité et rapprochements contradictoires.

## Alignement effectif au modèle COP

- [#120](https://github.com/JeanHuguesRobert/inseme/issues/120) : GitHub est actuellement notre support de **demande, code et preuve durable** ; les résultats de CI sont observables. Cela ne démontre pas l'exécution d'un véritable `compute.batch` au travers du webhook/COP dans cette passe.
- [#121](https://github.com/JeanHuguesRobert/inseme/issues/121) : branche + PR + SHA protègent les modifications GitHub ; la politique de claim/lease/fencing **sur Packet** n'est pas attestée par ce seul travail.
- [#122](https://github.com/JeanHuguesRobert/inseme/issues/122) : aucune découverte de capacité distante nouvelle n'est revendiquée.
- Continuation suivant ce résultat : **INV-003 / preuves financières réelles** — bloquée par l'accès aux justificatifs et la validation des droits ; les tests synthétiques continuent séparément.

## Sortie actuelle

`state=awaiting_authorized_sources`; `real_financial_rows_verified=0`; `real_amounts_reconciled=0`; `filed_documents=0`. Il s'agit de métriques de **cette passe**, pas d'une assertion sur la comptabilité de l'association.
