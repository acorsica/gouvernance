# Septembre 2026 — hypothèses comparatives de valorisation du bénévolat

Statut : hypothèses d'analyse, non heures constatées, non salaire, non dette, non écriture comptable approuvée.

## Repères

- Baseline d'activité : fonction de direction salariée de C.O.R.S.I.C.A. à mi-temps, soit 17 h 30 par semaine (75,83 heures mensuelles conventionnelles).
- « mima » : référence monétaire au SMIC brut applicable au mois étudié ; septembre 2026 : 12,31 euros/heure et 1 867,02 euros/mois à temps plein ; à mi-temps, **933,51 euros brut mensuels**.
- Référence de directeur salarié : autre montant à documenter par barème, convention ou étude de salaire comparable ; ne pas inventer un tarif de directeur réel.

Sources : [INSEE SMIC septembre 2026](https://www.insee.fr/fr/statistiques/1375188), [série mensuelle INSEE](https://www.insee.fr/fr/statistiques/serie/000822484).

## Règles de rapprochement

Le montant de 933,51 euros est un **repère salarial**, non un coût employeur et non une valeur comptable acquise. La baseline mi-temps exprime une capacité de travail normalisée, pas les heures réelles de septembre. Une valorisation de contributions volontaires en nature implique une définition précise du périmètre associatif, des heures bénévoles justifiées, une méthode d'évaluation et un contrôle des doublons avec les services/abonnements déjà comptés.

Comparer séparément : (A) valeur de référence mima d'un mi-temps conventionnel, (B) valeur de référence d'un directeur à mi-temps à déterminer, (C) bénévolat réellement justifié, encore inconnu. Ne jamais enregistrer un salaire, une dette salariale ou une charge monétaire sur la seule base de cette comparaison.

Lien : [Cognitive Packet COP Accounting C.O.R.S.I.C.A.](https://github.com/acorsica/gouvernance/issues/2).

## Correction réglementaire du 9 octobre 2026 — salaire chargé

**Décision méthodologique provisoire : comparer les contributions bénévoles au coût complet de remplacement pour l'association, et non au seul salaire net ou brut.** Ceci constitue une méthode choisie et justifiée, **pas un coefficient patronal uniforme imposé par le droit**.

### Deux repères à distinguer

1. **mima-brut** : 933,51 € bruts par mois pour le mi-temps conventionnel au SMIC de septembre 2026 (référence salariale uniquement).
2. **mima-chargé / coût de remplacement minimal** : salaire brut ci-dessus **plus cotisations patronales effectivement applicables après allègements**, plus coûts d'emploi pertinents et justifiables (mutuelle, prévoyance et éventuelles contributions spécifiques selon situation). **Montant en euros encore à calculer avec paramètres employeur** ; ne pas plaquer un forfait de 40 %.
3. **baseline-directeur-chargée** : référence d'un directeur salarié à mi-temps selon un salaire de marché ou grille documentée, **charges patronales et coûts connexes compris**, sous réserve du rattachement réel à C.O.R.S.I.C.A. et des conventions applicables.

Règle : comparer à durée identique ; conserver en parallèle les colonnes net, brut, contributions patronales, allègements, coût employeur et sources ; valorisation comptable définitive seulement sur temps bénévole et méthode vérifiés. Ni salaire dû, ni créance personnelle, ni mouvement bancaire n'en découlent.

### Sources et vérification

- [ANC règlement 2018-06](https://www.anc.gouv.fr/reglement-ndeg-2018-06-du-5-decembre-2018) — présentation des contributions volontaires en nature.
- [Ministère — valorisation du bénévolat](https://associations.gouv.fr/la-valorisation-comptable-du-benevolat) — choix de méthode documenté, sans tarif universel obligatoire.
- [HCVA 2026 — méthodes de valorisation](https://associations.gouv.fr/sites/default/files/2026-04/HCVA%20-%20Valorisation%20comptable%20du%20b%C3%A9n%C3%A9volat%20-%2020%20avril%202026.pdf) — coût de remplacement, opportunité, forfait horaire ; justification et constance.
- [Guide ministériel de valorisation](https://www.associations.gouv.fr/sites/default/files/2025-06/valorisation_comptable_benevolat_0.pdf) — exemples de SMIC chargé et taux différenciés selon fonctions, non normes impératives.
- [URSSAF — réduction générale dégressive unique 2026](https://www.urssaf.fr/accueil/employeur/beneficier-exonerations/reduction-generale-cotisation.html) — cotisations patronales allégées variables.
- [Simulateur URSSAF du coût d'embauche](https://www.service-public.gouv.fr/particuliers/vosdroits/R45531) — estimation paramétrée, à ne pas confondre avec un devis contractuel.

**Paramètres manquants** : convention collective applicable ou absence, régime de prévoyance et mutuelle, AT/MP, effectifs, implantation, situation du salarié type. Conserver `mima_charged_eur=null` tant que ces variables ne sont pas déterminées et la simulation documentée.
