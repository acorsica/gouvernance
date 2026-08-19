---
title: C.O.R.S.I.C.A. – Gouvernance
author: unknown
date: '2026-06-03'
document_role: source
document_kind: documentation
visibility: public
lifecycle_state: working
update_policy: UP-DEFAULT-REVIEWED
provenance:
  origin_type: repository
  origin_repository: acorsica/gouvernance
  origin_ref: b7e32dd
  origin_date: '2026-06-03'
  derived_from: []
review:
  status: unreviewed
  reviewed_by: []
---

# C.O.R.S.I.C.A. – Gouvernance

Ce dépôt contient les documents officiels de l’association **C.O.R.S.I.C.A.** (Corse Organisant la Réunion Sur Internet de Compétences Autonomes).

Il constitue le **registre public canonique des actes et documents de gouvernance de l’association**. Les documents qu’il contient constituent la référence de sa gouvernance, sous réserve de la valeur juridique propre des versions signées lorsqu’elles existent.

## Contenu

- identité administrative et implantation ;
- statuts ;
- règlements intérieurs ;
- procès-verbaux d’assemblées générales ;
- convocations ;
- documents relatifs à l’intérêt général ;
- registre des produits, services et publications ;
- documents de séparation institutionnelle, politique, patrimoniale, entrepreneuriale ou technique ;
- cartographie des dépôts liés ;
- état synthétique du corpus ;
- audits de l’organisation GitHub et du corpus public.

## Documents structurants

- [`identite-administrative.md`](identite-administrative.md) — identité publique de l’association, bureaux opérationnels actuels et distinction avec les modifications statutaires en cours.
- [`langue-de-reference.md`](langue-de-reference.md) — langue française comme source normative des documents de gouvernance.
- [`interet-general-et-separation-politique.md`](interet-general-et-separation-politique.md) — intérêt général, égalité politique, DHITL, communs démocratiques et séparation politique.
- [`produits-et-publications.md`](produits-et-publications.md) — registre canonique des produits, services et publications édités ou portés institutionnellement par C.O.R.S.I.C.A., dont Olé Olé.
- [`cartographie-du-corpus.md`](cartographie-du-corpus.md) — cartographie des dépôts liés à C.O.R.S.I.C.A., à l’Institut Mariani et au corpus personnel de Jean Hugues Noël Robert.
- [`etat-du-corpus.md`](etat-du-corpus.md) — état synthétique des dépôts, fonctions, documents de liaison et points à qualifier.
- [`audit-organisation-2026-06-03.md`](audit-organisation-2026-06-03.md) — audit de l’organisation GitHub `acorsica` et des corrections réalisées le 3 juin 2026.
- [`LICENSING.md`](LICENSING.md) — politique de licences pour contenus documentaires, logiciels et données ouvertes.

## Principe

Toute décision ou action significative est documentée.

La gouvernance repose sur un principe simple :

> un acte n’existe que s’il laisse une trace

Git est utilisé comme support de traçabilité :

- historisation des modifications ;
- horodatage ;
- transparence.

## Organisation

```text
gouvernance/
├── statuts/
├── reglement_interieur/
├── assemblees_generales/
├── identite-administrative.md
├── langue-de-reference.md
├── interet-general-et-separation-politique.md
├── produits-et-publications.md
├── cartographie-du-corpus.md
├── etat-du-corpus.md
└── audit-organisation-2026-06-03.md
```

Chaque assemblée générale fait l’objet d’un dossier daté.

## Processus

1. Préparation des documents (convocation, projets).
2. Tenue de l’assemblée.
3. Rédaction et validation du procès-verbal.
4. Archivage dans ce dépôt.
5. Signature et conservation des versions PDF.

## Valeur des documents

- Les documents Markdown constituent la version de travail et d’archive.
- Les versions signées (PDF) font foi juridiquement.
- La version française prévaut, sauf décision explicite contraire régulièrement documentée.

## Dépôts liés

- [`acorsica/.github`](https://github.com/acorsica/.github) — profil public GitHub de l’organisation.
- [`acorsica/institut-mariani`](https://github.com/acorsica/institut-mariani) — émanation R&D de C.O.R.S.I.C.A.
- [`acorsica/privai`](https://github.com/acorsica/privai) — initiative PrivAI, en développement au sein de l’Institut Mariani.

## Principe de séparation

Les liens entre dépôts expriment des relations documentaires, doctrinales, historiques ou techniques.

Ils ne valent ni fusion institutionnelle, ni portage juridique, ni financement, ni endorsement politique.

> L’interconnexion documentaire ne vaut pas confusion institutionnelle.

## Licences

- contenus documentaires originaux : **CC BY 4.0** par défaut ;
- logiciels originaux : **MIT** par défaut ;
- jeux de données intentionnellement publiés comme Open Data : **Licence Ouverte 2.0 / Etalab** par défaut.

Voir [`LICENSE`](LICENSE) et [`LICENSING.md`](LICENSING.md). Les droits de tiers, la vie privée, la confidentialité et les restrictions légales prévalent sur ces règles par défaut.

## Évolution

Le présent dépôt est évolutif.

Le règlement intérieur peut être modifié sans modification des statuts.

## Finalité

Ce dépôt constitue :

- une mémoire ;
- un outil de coordination ;
- un support de transparence ;
- un support d’étanchéité institutionnelle ;
- le registre canonique des actes, produits et publications institutionnellement portés par C.O.R.S.I.C.A.

Il peut servir de base à des systèmes de gouvernance distribuée.
