---
layout: post_site
title: "1 - Visualiser un algorithme"
date: 2019-02-03 12:04:32 +0100
permalink: "/visualiser-un-algorithme"
---

# Il est difficile de visualiser une algorithme (ou de visualiser tout court)

La force de la visualisation de données réside dans la communication de connaissance par l'encodage visuel afin de transformer des données abstraites en des représentations pertinentes. [^2]

Pourquoi la visualisation de données est complexe

(cf conférence Mike Bostock)
(cf livre visualisation)

Pourquoi les algorithmes sont des

# Algorithmes en boites
Augmenter la compréhension d'un processus logique par la vue.

La classification suivante[^1] a été proposée par Mike Bostock, le créateur de D3.js, l'outil le plus avancé de visualisation de données. Elle distingue trois familles d'algorithme en fonction de leur opacité.

<div>
<img src="{{site.baseurl}}/assets/img/boites.png" style="display: block; margin-left: auto; margin-right: auto; width:80%">
<h5 style="text-align:center">Figure 1 : Algorithmes classés en boites et ce que leur visualisation permet.</h5>
</div>

Une boite noire permet d'évaluer la véracité des résultats de l'algorithme mais sont fonctionnement est totalement opaque. Une boite grise donne une idée du comportement de l'algorithme mais peut induire en erreur ou apporter plus de questions que de réponses. La boite blanche enfin, a l'avantage de potentiellement expliquer le fonctionnement de l'algorithme. Cependant, la boite blanche s'accompagne d'une complexité plus grande de l'information, liée à au nombre et aux relations entre les données.[^1] Il est aisé de se représenter les trois situations précédentes avec un exemple simple d'algorithme : le calcul du PGCD par l'algorithme d'Euclide.

# Exemple : calcul du PGCD par algorithme d'Euclide

Nous souhaitons illustrer la partie précédente avec un exemple connu de tous. L'algorithme étudié est l'algorithme d'Euclide permettant de déterminer le plus grand commun diviseur entre deux nombre entiers positifs. Cet algorithme peut facilement être implémenté avec un language informatique. Nous choisissons de montrer ce que l'algorithme d'Euclide nous dit traité comme une boite noire, grise ou blanche.

Les deux premiers exemples sont l'algorithme en version boite noire et grise. Dans le cas de la <b>boite noire</b>, le résultat final est bien connu, et oui, 2 est bien le PGCD de 72 et 26. Nous pouvons vérifier que l'algorithme fonctionne sur ce cas mais rien ne nous dit que l'algorithme fonctionnera sur d'autres cas car on ne peut dire ce qu'il s'y passe. Dans le cas de la <b>boite grise</b>, les valeurs successives de b sont renvoyées par le programme. Les valeurs sont rassurantes car elles permettent de voir que les étapes de l'algorithme implémenté sont bien conforme à la manière dont procèderait un humain. Cependant rien de m'assure que les résultats donnés par l'algorithme proviennent bien de divisions euclidiennes successives.

<div>
<img src="{{site.baseurl}}/assets/img/black_box.png" style="align:left; width:49%">
<img src="{{site.baseurl}}/assets/img/grey_box.png" style="align:left; width:49%">
<h5 style="text-align:center">Figure 2 : Une <b>boite noire</b> et une <b>boite grise</b> pour l'algorithme de calcul du PGCD d'Euclide.</h5>
</div>

Enfin, l'algorithme en boite blanche permet de s'assurer de la bonne implémentation de l'algorithme. Il est alors possible de suivre chaque étape du programme et d'en comprendre la logique.

<div>
<img src="{{site.baseurl}}/assets/img/white_box.png" style="display: block; margin-left: auto; margin-right: auto; width:80%">
<h5 style="text-align:center">Figure 3 : Une <b>boite blanche</b> pour l'algorithme de calcul du PGCD d'Euclide.</h5>
</div>

Cependant, les données renvoyées par l'algorithme en version boite blanche ne constituent pas de l'information. Nous devons lier ces données à des représentations afin de créer une visualisation du fonctionnement de l'algorithme. Cette partie est la plus difficile. En effet, le cas d'une boite blanche soulève de nombreuses questions :
 * Quelles données représenter ? Beaucoup de données sont renvoyées, toutes ne doivent pas être utilisées pour la visualisation sous peine d'obscurcir le sens de la visualisation.
 * Comment encoder visuellement l'information ? Notre cas demande de représenter des nombres, ils peuvent correspondre à une longueur, une aire, une couleur, un symbole, ...
 * Que signifient les données ? Dans notre cas, la réponse est simple, mais ce n'est pas toujours le cas pour les algorithmes d'apprentissage automatique.
 * Comment représenter le passage des étapes ?
 * Ma visualisation fonctionnera t-elle si les données d'entrée changent ?

Nous proposons la visualisation suivante pour l'algorithme d'Euclide, avec 72 et 26 en entrées :

<div>
<img src="{{site.baseurl}}/assets/img/pgcd_algorithm_visualization.gif" style="display: block; margin-left: auto; margin-right: auto; width:100%">
<h5 style="text-align:center">Figure 4 : Proposition de visualisation pour l'algorithme d'Euclide.</h5>
</div>

Nous espérons que cette première partie permet de montrer qu'il n'y a rien d'évident à visualiser un algorithme. Le cas traité est un cas facile comparé à d'autres algorithmes et en particulier à ceux d'apprentissage automatique. En effet, l'algorithme d'euclide implémenté est une transcription à l'identique d'une programme fait à la main. Autrement dit, nous savons résoudre le problème du PGCD sans ordinateurs. Il existe une autre classe d'algorithme moins conventionnels qui nous aide à répondre à des problèmes que nous ne savons pas résoudre, les algorithmes d'apprentissage automatique.


<a href="{{site.baseurl}}/{% post_url 2019-02-02-pourquoi-visualiser-l-apprentissage_automatique %}">Partie 2 : Pourquoi visualiser les algorithmes de machine learning ?</a>

## Références

[^1]: Mike Bostock, <https://bost.ocks.org/mike/algorithms/>
[^2]: Fred Hohman & al, <https://arxiv.org/pdf/1801.06889.pdf>
