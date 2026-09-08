---
layout: page
permalink: /matrice/
title: Matrice croisée
titre_long: Stratégie contre tactique
chapeau: >-
  Ce que donne la superposition des deux listes : très peu de recouvrement, et
  c’est le résultat le plus intéressant du travail.
description: >-
  Lecture croisée des deux classements : qui figure dans les deux Top 12, qui
  domine d’un côté seulement, et les maîtres de l’art opératif.
---

<h2>Présents dans les deux Top 12</h2>

<div class="debord">
<table class="tableau">
  <caption>Calculé à partir des deux classements : sont retenus les noms qui figurent dans les douze premiers des deux listes.</caption>
  <thead>
    <tr><th>Personnage</th><th>Stratégie</th><th>Tactique</th><th>Lecture</th></tr>
  </thead>
  <tbody>
  {%- for s in site.data.strateges -%}
    {%- if s.rang <= 12 -%}
      {%- for t in site.data.tacticiens -%}
        {%- if t.rang <= 12 and t.nom == s.nom -%}
    <tr>
      <td>{{ s.nom }}</td>
      <td>{{ s.rang }}<sup>e</sup></td>
      <td>{{ t.rang }}<sup>e</sup></td>
      <td>{% if s.nom contains "Napoléon" %}Maître complet, mais tacticien supérieur à son bilan final de grande stratégie.{% else %}Le profil le plus équilibré du corpus entre apprentissage, campagne, bataille et résultat politique.{% endif %}</td>
    </tr>
        {%- endif -%}
      {%- endfor -%}
    {%- endif -%}
  {%- endfor -%}
  </tbody>
</table>
</div>

<p>Deux noms sur vingt-quatre places. Le reste des deux Top 12 ne se recoupe
pas du tout, et la matrice ci-dessous dit dans quel sens penche chacun.</p>

<h2>Stratèges nettement supérieurs à leur profil tactique</h2>

- **Gengis Khan** — système impérial et organisation de la guerre.
- **Otto von Bismarck** — choix et limitation des guerres, diplomatie et ordre politique.
- **Mao Zedong** — mobilisation politique et temporalité révolutionnaire.
- **Tokugawa Ieyasu** — coalition, patience et stabilisation.
- **Auguste** — institutionnalisation de la victoire.
- **Carl von Clausewitz** — puissance théorique.
- **Sun Tzu** — corpus stratégique.
- **George C. Marshall** — construction d’un appareil de guerre global.
- **Võ Nguyên Giáp** — articulation politico-militaire de l’asymétrie et du temps.

<h2>Tacticiens nettement supérieurs à leur profil de grande stratégie</h2>

- **Alexandre le Grand** — premier tacticien, mais dix-septième stratège en raison de la succession et de la stabilisation.
- **Hannibal Barca** — pic tactique immense, incapacité à convertir ses victoires en décision politique contre Rome.
- **Jules César** — tacticien de premier ordre ; sa carrière politico-stratégique n’a pas été retenue parmi les vingt finalistes stratégiques.
- **Yi Sun-sin** — tactique navale exceptionnelle, rôle stratégique plus spécialisé.
- **Horatio Nelson** — rupture tactique navale, stratégie nationale définie au-dessus de lui.
- **Épaminondas** — innovation de bataille majeure, échantillon stratégique plus limité.
- **Alexandre Souvorov** — commandement tactique et opératif supérieur à sa contribution de grande stratégie.
- **John Churchill, duc de Marlborough** — grand commandant de coalition, mais non auteur principal des finalités politiques britanniques.
- **Arthur Wellesley, duc de Wellington** — robustesse tactique exceptionnelle ; profil politico-stratégique moins transformateur.
- **Bélisaire** — économie des moyens et adaptation sous contraintes.

<h2>Maîtres de l’art opératif, identifiés mais non classés comme tels</h2>

- **Helmuth von Moltke l’Ancien** — dix-huitième stratège.
- **Subutaï** — dix-neuvième tacticien.
- **Konstantin Rokossovski** — vingtième tacticien.

Leur position montre pourquoi la séparation des niveaux est nécessaire : on peut
être extraordinairement important sans être automatiquement dans le Top 12 de
l’une ou l’autre discipline.

<h2>Conclusion</h2>

> La capacité à gagner des batailles et la capacité à gagner politiquement une
> guerre ne sont pas la même compétence.

Le faible recouvrement des deux listes n’est pas un défaut de construction. Il
est le résultat.
