---
title: "COP Accounting C.O.R.S.I.C.A. — contributions volontaires en nature"
date: "2026-10-09"
language: fr
document_role: operational
document_kind: accounting-evidence-policy
visibility: public
lifecycle_state: working
status: working-paper
update_policy: UP-DEFAULT-REVIEWED
review:
  status: unreviewed
  reviewed_by: []
provenance:
  origin_type: conversation-and-regulatory-research
  origin_date: "2026-10-09"
  derived_from:
    - "https://github.com/acorsica/gouvernance/issues/2"
    - "https://associations.gouv.fr/la-valorisation-comptable-du-benevolat"
    - "https://www.anc.gouv.fr/files/anc/files/1_Normes_fran%C3%A7aises/Reglements/2018/Reglt_2018_06/Reglt_2018-06_Association.pdf"
---

# COP Accounting — CVN et ressources privées mises à disposition de C.O.R.S.I.C.A.

**État : déclaré, non chiffré, non comptabilisé.** Le responsable indique mettre gratuitement à disposition de l'association : temps bénévole, accès Internet privé, abonnements et outils IA personnels, possiblement matériels/équipements. Cette contribution ne transforme pas le futur fonds de dotation Barons Mariani en personne morale, et n'atteste ni leur valeur ni leur affectation intégrale à l'association.

## Cadre applicable

Le règlement ANC 2018-06 et les références officielles du ministère chargé des associations permettent de documenter et, si mesure/évaluation fiable et méthode retenue, de présenter les contributions volontaires en nature (CVN) en classes **86** (emplois) et **87** (ressources), notamment **864/875** pour le bénévolat ; **861/871 ou 862/871** selon la nature précise des services / mises à disposition ; vérifier la correspondance des sous-comptes lors de la production. La reconnaissance est sans contrepartie monétaire et n'augmente pas la trésorerie ou le résultat ordinaire. À défaut de chiffrage suffisamment fiable, fournir description qualitative et raisons de la non-valorisation en annexe.

Sources :
- [Ministère — valorisation comptable du bénévolat](https://associations.gouv.fr/la-valorisation-comptable-du-benevolat)
- [ANC 2018-06](https://www.anc.gouv.fr/files/anc/files/1_Normes_fran%C3%A7aises/Reglements/2018/Reglt_2018_06/Reglt_2018-06_Association.pdf)
- [HCVA — valorisation 2026](https://associations.gouv.fr/sites/default/files/2026-04/HCVA%20-%20Valorisation%20comptable%20du%20b%C3%A9n%C3%A9volat%20-%2020%20avril%202026.pdf)

## Registre des contributions — informations à rechercher

| ID | Catégorie | Source / preuve à obtenir | Hypothèse de valorisation | État |
|---|---|---|---|---|
| CVN-001 | Temps bénévole de direction, technique, rédaction, recherche et gestion | Relevé de temps daté : tâche, projet, début/fin ou durée, lien à une trace (commit, document, décision), revue par un autre responsable si possible | Heures multipliées par un taux raisonnable, politique cohérente votée/documentée (SMIC, salaire de remplacement, coût de prestation comparable), méthode décrite | **Non chiffré** |
| CVN-002 | Accès Internet personnel utilisé par l'association | Factures nominatives sous contrôle privé, période, part d'usage associative raisonnablement mesurable, éventuel accord de mise à disposition | Coût évité / quote-part causale raisonnable, pas 100 % de l'abonnement personnel sans fondement | **Non chiffré** |
| CVN-003 | Abonnements et outils IA personnels | Factures, conditions d'utilisation/partage, tâche/projet associatif, journaux d'usage possibles sans contenu sensible | Coût de remplacement associatif ou quote-part justifiée ; ne pas déduire automatiquement que l'association dispose d'un droit contractuel sur un compte personnel | **Non chiffré** |
| CVN-004 | Ordinateur, matériel et éventuel local privé | Identité du propriétaire, dates/modes d'utilisation, durée, preuve des coûts comparables, autorisation et conditions | Valeur de la mise à disposition (non valeur totale du bien, sauf véritable don avec transfert) | **Non chiffré** |
| CVN-005 | Dépenses privées payées pour l'association | Pièce originale, titulaire réel, relevé de paiement, décision de remboursement/renonciation | Dépense/avance/abandon de remboursement/CVN selon nature et faits ; jamais classer d'office une avance en don | **À qualifier** |

## Contrôles COP stricts

- Séparer **cash_ledger** (encaissements, dépenses, dettes, avances), **cvn_ledger** (ressources gratuites/emplois symétriques) et **analytic_project** (dont Barons Mariani) ; ne pas combler artificiellement le cash.
- Une contribution de temps comporte `contribution_id`, `contributor_ref`, `legal_entity_ref`, `project_ref`, `period`, `hours_exact`, `work_description`, `proof_refs`, `valuation_method`, `rate_source`, `amount_exact`, `review_status`; pas de valeur financière définitive avant validation.
- Exiger l'indépendance autant que possible de la validation lorsque le contributeur est également dirigeant ; documenter conflits d'intérêt et ratification des règles internes.
- Interdire le double comptage (par exemple heures bénévoles déjà comprises dans une prestation comptée, accès Internet à la fois remboursé et déclaré CVN).
- Ne pas assimiler valorisation bénévole et facture due ou don fiscalement déductible : bénéfice fiscal et émission de reçu nécessitent vérifications distinctes.
- Pour une déclaration rétroactive de temps, l'étiqueter comme **reconstitution** et préciser les bornes, sources et incertitudes ; ne jamais prétendre à un pointage contemporain.
- Vérifier les politiques de licences des abonnements IA : usage personnel et professionnel/association ne sont pas nécessairement interchangeables.

## Premier test du réel proposé

1. Choisir un mois récent et 5 à 10 actions associatives vérifiables (commits, comptes rendus, échanges).
2. Établir un journal de temps estimé/documenté, avec distinction du temps purement personnel ou politique.
3. Proposer une méthode conservatrice de valorisation, approuvée ou revue, mais garder valeur **provisoire**.
4. Rapprocher factures Internet/IA avec l'usage associatif et contrôler les paiements personnels.
5. Présenter deux états **séparés** : flux bancaires de l'association et CVN, sans addition trompeuse des deux en chiffre d'affaires ni en trésorerie.

L'absence de recettes monétaires reste une **déclaration à vérifier par les relevés SG**, et ne doit pas être convertie en certitude à partir des CVN.
