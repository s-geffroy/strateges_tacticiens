---
layout: page
permalink: /a-propos/
title: À propos
titre_long: Ce que ce site publie
chapeau: >-
  Deux classements arrêtés, quarante dossiers, et une manière de les lire. Ce
  qui suit dit ce que ce travail prétend faire, ce qu’il refuse de faire, et
  comment la chose est fabriquée.
description: >-
  Ce que publie ce site, ce qu’il ne prétend pas établir, comment lire les
  rangs et la confiance, et comment le site est construit.
---

## Ce que vous lisez

Deux classements autonomes, construits selon une architecture parallèle : les
douze plus grands stratèges et les douze plus grands tacticiens, chacun suivi
de huit prétendants immédiats. Derrière chaque nom, un dossier comparatif
(quarante en tout) qui expose le profil, le cas maître, l’avantage décisif, la
limite, la part qui lui revient en propre et la qualité des sources.

La version a été arrêtée le 11 août 2026. Elle est fermée sur le fond.

## Ce que ce travail refuse de faire

**Publier un score.** Aucun total, aucune décimale. Les grilles à cent points
servent à structurer la comparaison, pas à produire un chiffre : les rangs
résultent d’un arbitrage ordinal et d’analyses de sensibilité. Un classement
qui affiche 87,4 contre 86,9 ment sur sa propre précision.

**Confondre les niveaux de guerre.** L’art opératif, qui organise les opérations
en campagnes, n’a pas de classement propre. Y exceller ne qualifie donc pour
aucune des deux listes, et trois grands noms en font les frais.

**Classer les conquérants.** Le rang stratégique récompense la transformation
de la puissance disponible en résultat politique, pas l’étendue des conquêtes.
C’est pourquoi Bismarck, qui n’a conduit aucune opération, devance Napoléon.

**Trancher moralement.** Staline est évalué sans complaisance et sans exclusion
automatique : ce sont ses erreurs et ses coûts qui lui interdisent un rang
élevé, pas sa nature. Symétriquement, l’incertitude documentaire d’une figure
antique ou médiévale pèse sur la **confiance dans son rang**, jamais comme une
pénalité de civilisation.

## Comment lire un rang

Trois choses accompagnent chaque nom et se lisent ensemble.

- **Les crans**, de un à cinq, disent la solidité du dossier, pas la valeur de
  l’homme. Un dernier rang peut en porter cinq, et un rang du milieu un
  seul.
- **La porte d’admissibilité**, entre la douzième et la treizième place, est un
  seuil et non une frontière de qualité. Les huit qui suivent sont des
  prétendants immédiats, pas des candidats inférieurs.
- **La bande estimée avant arbitrage** conserve la trace du raisonnement : elle
  montre dans quel intervalle le dossier flottait avant que les procès
  contradictoires ne le fixent.

Le détail des grilles, des portes et des corrections est dans la
[méthodologie]({{ '/methodologie/' | relative_url }}) ; les frontières encore
disputées sont plaidées dans les
[arbitrages]({{ '/arbitrages/' | relative_url }}).

## Contester un rang

La règle de stabilité est la contrepartie d’une liste arrêtée. Un rang ne se
rouvre qu’en présence d’un **élément documentaire nouveau**, d’une **erreur
factuelle identifiée** ou d’une **contradiction méthodologique démontrée**. Une
préférence pour un nom ou une école militaire ne suffit pas.

Les erreurs factuelles, elles, se corrigent sans discussion : elles se
signalent dans le [dépôt du site](https://github.com/s-geffroy/strateges_tacticiens).

## L’auteur

Le corpus est de **Sylvain Geffroy** : la méthodologie, les quarante dossiers,
les procès contradictoires des places de frontière et l’arrêt des listes. Le
site n’est que la mise en ligne de ce travail, par la même main.

Ce que cela implique se lit dans la règle de stabilité ci-dessus : les listes
sont fermées par leur auteur, et rouvertes aux mêmes conditions que pour
n’importe qui : un document nouveau, une erreur ou une contradiction.

## Comment le site est fabriqué

Les quarante dossiers vivent dans deux fichiers de données, et rien d’autre :
les classements, les pages de dossiers et la matrice croisée en sont trois vues
calculées. Aucun rang n’est recopié à la main, donc aucun ne peut diverger d’un
endroit à l’autre du site.

Le reste est délibérément simple. Jekyll construit les pages, sans thème :
les gabarits sont écrits pour ce site. Chaque poussée de code déclenche une
construction et une publication par GitHub Actions, et GitHub Pages sert le
résultat. Il n’y a ni base de données ni serveur d’application. Le seul script
chargé chez le visiteur est le bandeau commun de
[Ligne de crête](https://www.ligne-de-crete.fr/), la vitrine qui présente ce
travail parmi d’autres ; le site lui-même n’en exécute aucun. En plus des pages,
le navigateur télécharge une feuille de style et deux familles de caractères.

Le dépôt est public :
[s-geffroy/strateges_tacticiens](https://github.com/s-geffroy/strateges_tacticiens).
