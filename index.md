---
layout: default
title: Accueil
description: >-
  Les douze plus grands stratèges et les douze plus grands tacticiens, classés
  par arbitrage multicritère, chaque rang accompagné de la confiance qu’on peut
  lui accorder.
---

{% include titre-page.html texte="Douze stratèges, douze tacticiens" %}

<p class="chapeau">Gagner des batailles et gagner politiquement une guerre ne
sont pas la même compétence. Ce site tient donc deux listes séparées, arrêtées
le 11 août 2026, et ne publie aucun score : à la place, chaque rang porte la
confiance qu’il mérite.</p>

<div class="pivot">
  <section class="definition">
    <h2>Le stratège</h2>
    <p>Il convertit en résultat politique des moyens qui ne sont pas seulement
    militaires : l’économie et le temps en font partie. Il choisit ses objectifs
    et ajuste les fins aux moyens ; il tient une coalition, puis organise
    l’après-guerre.</p>
    <a class="conduit" href="{{ '/strateges/' | relative_url }}">Les douze stratèges</a>
  </section>

  <div class="pivot-filet"></div>

  <section class="definition">
    <h2>Le tacticien</h2>
    <p>Il transforme une situation de combat en avantage militaire décisif. Il
    conçoit l’engagement en lisant le terrain et l’adversaire ; il place ses
    réserves, et improvise quand le plan cède.</p>
    <a class="conduit" href="{{ '/tacticiens/' | relative_url }}">Les douze tacticiens</a>
  </section>
</div>

<figure class="figure">
  <div class="debord">
    {% include croisement.html %}
  </div>
  <figcaption>
    Les deux classements face à face, et les quatre seules liaisons qui existent
    entre eux. Deux hommes figurent dans les <strong>deux Top 12</strong> :
    <a href="{{ '/dossiers-strateges/' | relative_url }}#napoleon-bonaparte">Napoléon
    Bonaparte</a>, quatrième stratège et deuxième tacticien, et
    <a href="{{ '/dossiers-strateges/' | relative_url }}#scipion-l-africain">Scipion
    l’Africain</a>, cinquième des deux côtés. Deux autres apparaissent des deux
    côtés sans être admis nulle part :
    <a href="{{ '/dossiers-tacticiens/' | relative_url }}#alexandre-le-grand">Alexandre
    le Grand</a>, premier tacticien mais seulement dix-septième stratège, et
    <a href="{{ '/dossiers-strateges/' | relative_url }}#frederic-ii-de-prusse">Frédéric
    II de Prusse</a>, écarté de justesse deux fois. Les trente-deux autres noms
    n’existent que d’un seul côté. Chaque nom de la figure ouvre la fiche du
    personnage : sa biographie, son portrait, et de quoi aller plus loin.
  </figcaption>
</figure>

<div class="prose">

<h2>Ce que mesure l’échelle de gauche</h2>

<p>Un classement qui affiche un score au dixième de point ment sur sa propre
précision. Celui-ci refuse le score et déclare autre chose : pour chaque nom,
la solidité du dossier. Les cinq crans portés dans la marge des deux listes se
lisent ainsi.</p>

<div class="legende">
  {% include cran.html cran=5 libelle="Très élevée" decor=true %}
  <p><strong>Très élevée.</strong> Documentation abondante, attribution nette, aucune place sérieusement contestable.</p>
  {% include cran.html cran=4 libelle="Élevée" decor=true %}
  <p><strong>Élevée.</strong> Le dossier tient ; l’écart avec les rangs voisins reste discutable.</p>
  {% include cran.html cran=3 libelle="Moyenne à élevée" decor=true %}
  <p><strong>Moyenne à élevée.</strong> Une dimension du dossier (sources, attribution ou échantillon) reste ouverte.</p>
  {% include cran.html cran=2 libelle="Moyenne" decor=true %}
  <p><strong>Moyenne.</strong> Le rang est un arbitrage assumé, pas une évidence.</p>
  {% include cran.html cran=1 libelle="Faible à moyenne" decor=true %}
  <p><strong>Faible à moyenne.</strong> Le talent est plausible, les sources ne permettent pas de le situer.</p>
</div>

<p>Le cran ne juge pas l’homme, il juge la preuve. <a href="{{ '/dossiers-tacticiens/' | relative_url }}#konstantin-rokossovski">Konstantin Rokossovski</a> est
vingtième des tacticiens avec une confiance maximale, parce qu’on sait
précisément ce qu’il a fait et que cela relève de l’art opératif. <a href="{{ '/dossiers-tacticiens/' | relative_url }}#khalid-ibn-al-walid">Khalid ibn
al-Walid</a> est quinzième avec la confiance la plus basse : c’est la résolution
documentaire qui lui interdit le Top 12, pas une infériorité démontrée.</p>

<h2>Un troisième niveau, mais pas un troisième classement</h2>

<p>Entre la bataille et la guerre, l’art opératif organise les opérations en
campagnes. Le site ne lui consacre pas de liste : il s’en sert pour tenir les
deux autres. Briller dans la conduite des campagnes ne suffit pas à entrer dans
l’un ou l’autre Top 12, et trois grands noms restent ainsi parmi les
prétendants : <a href="{{ '/dossiers-strateges/' | relative_url }}#helmuth-von-moltke-l-ancien">Helmuth von Moltke l’Ancien</a>, <a href="{{ '/dossiers-tacticiens/' | relative_url }}#subutai">Subutaï</a> et <a href="{{ '/dossiers-tacticiens/' | relative_url }}#konstantin-rokossovski">Rokossovski</a>.</p>

<h2>Le reste des correspondances</h2>

<p>Le tableau croisé prend les trente-six personnages un par un : leur rang et
leur confiance dans chaque discipline, et ce que la comparaison révèle de chacun :
<a href="{{ '/matrice/' | relative_url }}">voir la matrice croisée</a>.</p>

</div>
