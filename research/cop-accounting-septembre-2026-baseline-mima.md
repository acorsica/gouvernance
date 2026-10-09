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

## Scénario paramétré — septembre 2026 (simulation préparatoire)

**Hypothèses:** association employeuse, un salarié directeur soumis au droit commun et à l'assurance chômage, CDI hypothétique, 17 h 30 hebdomadaires (50 % de 35 h), 933,51 € brut mensuel au SMIC en vigueur depuis le 1er juin 2026, effectif hypothétique inférieur à 50, Fnal 0,10 %. **Ce n'est ni une embauche réelle ni une déclaration sociale.**

**Correction essentielle:** la réduction générale dégressive unique (RGDU) de 2026 utilise **le SMIC de référence gelé au 1er janvier 2026 (12,02 €/h, 1 823,03 € mensuels à temps plein)**, même si le salaire légal de septembre est de 12,31 €/h. Pour un mi-temps, la référence RGDU est proratisée. Ne pas simuler la réduction avec le SMIC de septembre par défaut ; le simulateur URSSAF 2026 indique intégrer la RGDU. [Service Public, 18 juin 2026](https://entreprendre.service-public.gouv.fr/actualites/A18966).

Valeurs fixées : 75,83 h/mois et 933,51 € brut/mois. **Coût employeur exact non calculé par le simulateur dans ce travail**, faute de paramétrage complet des taux AT/MP, statut conventionnel, complémentaire santé, prévoyance, versement mobilité éventuel, avantages et autres charges ; ne pas convertir les 933,51 € en coût employeur à l'aide d'un multiplicateur générique. Le coût employeur est supérieur ou égal au brut augmenté des cotisations patronales nettes dues, sous réserve d'éventuelles aides distinctes et de la définition retenue.

Mode opératoire de simulation à reproduire : [Simulateur officiel URSSAF](https://mon-entreprise.urssaf.fr/simulateurs/salaire-brut-net) : salarié, temps partiel 17 h 30/semaine, brut 933,51 €/mois, employeur de moins de 5 salariés, localité Corte (Haute-Corse), statut non-cadre à titre d'hypothèse mima, puis relever le coût total et les cotisations détaillées avec date et paramètres ; deuxième passe avec statut et salaire de **directeur** réellement comparables. Le statut cadre ne se présume pas. [Vérification Service Public](https://www.service-public.gouv.fr/particuliers/vosdroits/R45531).

**Sortie:** `mima_gross_eur=933.51`, `mima_employer_cost_eur=null`, `director_reference_employer_cost_eur=null`, `hours_effectively_worked=null`. Comparaisons préparées, pas de coût employeur ou CVN chiffrés comme certifiés.

## Estimation reproductible du coût employeur — 9 octobre 2026

La formule officielle RGDU 2026 est documentée par [Service Public](https://entreprendre.service-public.gouv.fr/actualites/A18966) et [Urssaf](https://www.urssaf.fr/accueil/employeur/beneficier-exonerations/reduction-generale-cotisation.html). Sous hypothèse **un salarié, moins de 50 salariés, FNAL 0,10 %, mi-temps constant, brut mensuel 933,51 €, année entière à rémunération constante**, SMIC de référence RGDU = 1 823,03 € * 0,5 = 911,515 € par mois :

`coefficient = 0.02 + 0.3781 * ((3*911.515/933.51 - 1)/2)^1.75 ≈ 0.3750` ; `allègement théorique mensuel ≈ 350,09 €` (à confirmer par assiette annuelle, régularisation et règles d'arrondi). Il ne s'agit **pas** du total des cotisations patronales : le coût final requiert leur assiette/taux avant réduction.

Pour visualiser la sensibilité, seulement comme **hypothèses mathématiques de taux patronal total avant réduction**, et non comme taux réglementaires validés :

| Taux global de charges avant allègement *supposé* | Coût = 933,51 × (1 + taux) − 350,09 |
|---|---:|
| 40 % | ≈ 956,82 €/mois |
| 42 % | ≈ 975,49 €/mois |
| 45 % | ≈ 1 003,50 €/mois |

Ces valeurs **ne sont pas** une simulation URSSAF complète, une fourchette de taux officielle, ni le montant prêt à comptabiliser. Mutuelle, prévoyance, taxe, AT/MP, fraction non allégeable, règles d'éligibilité, structure de salaire, avantages et convention collective peuvent faire varier le résultat. Les montants strictement calculables à ce stade sont le SMIC brut, le coefficient théorique et l'allègement théorique, **pas** le coût global réel.

### Baseline directeur : prochaine donnée manquante

Le taux d'un directeur salarié ne peut pas être assimilé au SMIC sans examen de la qualification, des responsabilités, de la convention collective potentiellement applicable et de références salariales pour un poste à 17 h 30/semaine. Il convient de construire une **seconde hypothèse de rémunération documentée**, de réappliquer la RGDU (qui diminue lorsque le salaire augmente), et d'afficher séparément coût employeur et contribution bénévole constatée. **Le statut de président bénévole ne doit pas être requalifié en contrat de travail fictif.**

## Comparatif directeur — scénarios exploratoires (9 octobre 2026)

La convention collective ne se déduit **pas** du seul statut associatif. Elle dépend de l'activité effective ; [Service Public, vérifié avril 2026](https://www.service-public.gouv.fr/particuliers/vosdroits/F2607). La branche [ÉCLAT](https://www.legifrance.gouv.fr/conv_coll/id/KALISCTA000005725513/) est une piste à examiner, non une classification affirmée de C.O.R.S.I.C.A. Sa classification et ses valeurs de point ne seront appliquées qu'une fois le périmètre professionnel confirmé.

Faute de grille de directeur confirmée, trois salaires **purement hypothétiques** de référence à temps plein sont proposés : 2 500, 3 000 et 3 500 € brut/mois. Sur 17 h 30 hebdomadaires, le salaire brut correspondant est la moitié. Hypothèse commune moins de 50 salariés, 2026, 1er janvier comme SMIC de calcul RGDU, salaire constant toute l'année, pas d'heures supplémentaires. Les coefficients suivent la [formule officielle 2026](https://www.economie.gouv.fr/entreprises/gerer-ses-ressources-humaines-et-ses-salaries/comment-fonctionne-la-reduction-generale-degressive-unique-rgdu-de-cotisations-patronales).

| Hypothèse | Brut temps plein | Brut mi-temps | RGDU théorique mi-temps/mois | Coût illustratif avec cotisations patronales supposées à 42 % avant RGDU |
|---|---:|---:|---:|---:|
| Mima | 1 867,02 € | 933,51 € | 350,07 € | 975,52 € |
| Directeur A | 2 500 € | 1 250 € | 214,88 € | 1 560,12 € |
| Directeur B | 3 000 € | 1 500 € | 149,85 € | 1 980,15 € |
| Directeur C | 3 500 € | 1 750 € | 106,93 € | 2 378,07 € |

**IMPORTANT :** 42 % est un **paramètre de sensibilité arbitraire** pour comparer les scénarios, **ni un taux vérifié ni une simulation URSSAF**. Chiffres arrondis, avant mutuelle, prévoyance, médecine du travail, AT/MP spécifique, formation et contributions éventuelles hors hypothèse. Le coût employeur réel n'est **pas** encore déterminé. Il ne faut pas utiliser le tableau comme budget de paie ou comme écriture de CVN. Les montants RGDU sont annualisés théoriquement puis divisés par 12, et pourraient différer de la paie réelle selon la régularisation et les paramètres.

**À trancher :** activité principale et convention éventuelle, niveau de responsabilité du poste fictif, référence externe de salaire de directeur, paramètres sociaux, nature de la durée de travail et justification des heures bénévoles effectives. Notre comparaison économique ne crée aucun contrat de travail.
