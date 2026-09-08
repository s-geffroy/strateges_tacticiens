---
layout: page
permalink: /matrice/
title: Matrice croisée
titre_long: Stratégie contre tactique
chapeau: >-
  Les deux classements superposés, personnage par personnage. Trente-six noms,
  quarante places : quatre hommes seulement occupent une place dans chaque
  discipline.
description: >-
  Tableau croisé des deux classements : rang stratégique et rang tactique de
  chacun des trente-six personnages, et ce que la comparaison révèle.
---

<div class="debord">
<table class="tableau matrice">
  <caption>Construit à partir des deux classements. Un rang en gris désigne un
  prétendant immédiat, hors du Top 12. Chaque rang conduit au dossier
  correspondant.</caption>
  <thead>
    <tr>
      <th scope="col">Personnage</th>
      <th scope="col" class="col-rang">Stratégie</th>
      <th scope="col" class="col-rang">Tactique</th>
      <th scope="col">Ce que dit la comparaison</th>
    </tr>
  </thead>

  {%- assign S = '/dossiers-strateges/' | relative_url -%}
  {%- assign T = '/dossiers-tacticiens/' | relative_url -%}

  <tbody>
    <tr class="rubrique"><th colspan="4" scope="colgroup">Classés dans les deux disciplines</th></tr>
    {%- for s in site.data.strateges -%}
      {%- assign t = site.data.tacticiens | where: 'nom', s.nom | first -%}
      {%- if t %}
    <tr>
      <th scope="row">{{ s.nom }}</th>
      <td class="col-rang"><a class="{% if s.rang > 12 %}hors{% endif %}" href="{{ S }}#{{ s.slug }}">{{ s.rang }}<sup>e</sup></a></td>
      <td class="col-rang"><a class="{% if t.rang > 12 %}hors{% endif %}" href="{{ T }}#{{ t.slug }}">{{ t.rang }}<sup>e</sup></a></td>
      <td>{{ s.croise | default: t.croise }}</td>
    </tr>
      {%- endif -%}
    {%- endfor %}
  </tbody>

  <tbody>
    <tr class="rubrique"><th colspan="4" scope="colgroup">Classés en stratégie seulement</th></tr>
    {%- for s in site.data.strateges -%}
      {%- assign t = site.data.tacticiens | where: 'nom', s.nom | first -%}
      {%- unless t %}
    <tr>
      <th scope="row">{{ s.nom }}</th>
      <td class="col-rang"><a class="{% if s.rang > 12 %}hors{% endif %}" href="{{ S }}#{{ s.slug }}">{{ s.rang }}<sup>e</sup></a></td>
      <td class="col-rang vide" aria-label="non classé">—</td>
      <td>{{ s.croise }}</td>
    </tr>
      {%- endunless -%}
    {%- endfor %}
  </tbody>

  <tbody>
    <tr class="rubrique"><th colspan="4" scope="colgroup">Classés en tactique seulement</th></tr>
    {%- for t in site.data.tacticiens -%}
      {%- assign s = site.data.strateges | where: 'nom', t.nom | first -%}
      {%- unless s %}
    <tr>
      <th scope="row">{{ t.nom }}</th>
      <td class="col-rang vide" aria-label="non classé">—</td>
      <td class="col-rang"><a class="{% if t.rang > 12 %}hors{% endif %}" href="{{ T }}#{{ t.slug }}">{{ t.rang }}<sup>e</sup></a></td>
      <td>{{ t.croise }}</td>
    </tr>
      {%- endunless -%}
    {%- endfor %}
  </tbody>
</table>
</div>

## Ce que le tableau donne à voir

Deux hommes seulement figurent dans les **deux Top 12** : Napoléon Bonaparte,
quatrième stratège et deuxième tacticien, et Scipion l’Africain, cinquième dans
les deux listes. Deux autres apparaissent des deux côtés sans être admis
partout : Alexandre le Grand, premier tacticien mais seulement dix-septième
stratège, et Frédéric II de Prusse, écarté de justesse dans les deux
disciplines.

Trente-deux noms sur trente-six ne figurent donc que d’un seul côté. Ce faible
recouvrement n’est pas un défaut de construction, c’est le résultat.

> La capacité à gagner des batailles et la capacité à gagner politiquement une
> guerre ne sont pas la même compétence.

## Le niveau qui n’a pas de colonne

Trois noms occupent une case par défaut plutôt que par mérite : Helmuth von
Moltke l’Ancien est rangé en stratégie, Subutaï et Konstantin Rokossovski en
tactique, alors que leur génie est **opératif** — organiser des opérations en
campagnes. Le corpus a délibérément refusé d’en faire un troisième classement
et s’en sert comme catégorie de contrôle. Leur position dans ce tableau montre
ce que ce choix coûte, et pourquoi la séparation des niveaux reste nécessaire :
on peut être extraordinairement important sans appartenir au Top 12 de l’une ou
l’autre discipline.

## Les cases vides

Une case vide dans la colonne « Ce que dit la comparaison » n’est pas un oubli.
Le corpus ne commente au niveau croisé que vingt-quatre des quarante dossiers ;
pour les seize autres, il ne dit rien, et rien n’a été ajouté ici.
