---
layout: post_site
title: "Introduction"
date: 2019-02-04 12:04:32 +0100
permalink: "/introduction"
---
## Pourquoi ce blog ?

# Visualisation de données

Un artéfact est un objet auquel l'humain a donné forme. Par extension, il "amplifie les aptitudes humaines"[^1]. Dans la représentation ci-dessous, les constructeurs de cathédrales utilisent une échelle, une poulie, un
marteau et un burrin pour réaliser leur tâche. Ce sont autant d'artéfacts qui leur permettent de faire plus que ce à quoi les limitent leurs membres corporels.

<div>
<img src="{{site.baseurl}}/assets/img/artefacts_cathedral.png" style="display: block; margin-left: auto; margin-right: auto; width:50%">
<h5 style="text-align:center">Figure 1 : Constructeurs de cathédral et leurs artéfacts</h5>
</div>

Les artéfacts mentionnés sont physiques, ils changent l'intéraction de l'humain avec la
matière. Qu'en est-il de l'information ? Une sous-famille d'artéfacts dit "cognitifs" permettent d'aider l'humain dans son traitement de l'information.

<p style="text-align: center">
  <i>"Un artefact cognitif est un outil artificiel conçu pour conserver, exposer et traiter l'information dans le but de satisfaire une fonction représentationnelle." </i>[^1]
</p>

C'est dans ce sens que nous définirons ce qu'est la <b>visualisation</b> :

<p style="text-align: center">
  <i>"The use of computer-supported, interactive, visual representations of data to amplify cognition." </i>[^2]
</p>

À titre d'exemple d'amplification de compréhension d'un phénomène nous choisissons de citer la carte de Joseph Minard ci-dessous. Elle a été réalisée en 1869, représentant l'évolution de l'effectif des troupes napoléoniennes au cours de la campagne de Russie de 1812.

<div>
<img src="{{site.baseurl}}/assets/img/minard_napoleon.png" style="display: block; margin-left: auto; margin-right: auto; width:100%">
<h5 style="text-align:center">Figure 2 : Évolution de l'effectif la Grande Armée lors de la campagne de Russie par Minard</h5>
</div>

La force de cette visualisation réside dans l'encodage visuel d'une donnée (un effectif) au fil du temps et dans l'espace.

# Algorithme

Nous utiliserons beaucoup le terme algorithme dans cette étude. Nous choisissons d'utiliser une définition simple qui montre la différence entre algorithme et programme informatique.

<p style="text-align: center">
<i>"Ensemble de règles opératoires dont l'application permet de résoudre un problème énoncé au moyen d'un nombre fini d'opérations. Un algorithme peut être traduit, grâce à un langage de programmation, en un programme exécutable par un ordinateur." </i>[^3]
</p>

Un algorithme est donc en premier lieu une somme d'opérations logiques interprétables par l'humain, comme une recette de cuisine. Ainsi, c'est bien une traduction qu'un programmeur doit opérer afin de rendre un algorithme interprétable sous la forme d'un programme. Le programme découle de l'algorithme et pas l'inverse.

# Machine Learning

L'apprentissage automatique décrit une catégorie de programmes informatiques qui améliorent leur performance à une tâche donnée par l'expérience. De manière formelle :

<p style="text-align: center">
<i>"A computer program is said to learn from experience E with respect to some class of tasks T and performance measure P, if its performance at tasks in T, as measured by P, improves with experience E." </i>[^4]
</p>

En pratique, l'apprentissage automatique revient à chercher de manière automatisée une fonction. Cette fonction est produite par un modèle à partir de données d'entrainement. Le modèle évalue la qualité d'une fonction à partir d'une mesure de performance donnée au préalable.

# Cadre d'étude

L'apprentissage automatique est un domaine immense. De plus, les effets sociétaux liés à ses applications sont encore mal connus. Nous nous devons donc donner un cadre à cette étude afin de ne pas nous éparpiller ou risquer de rester à la surface des choses. Nous voulons donc être clair sur ce qui sera traité et ce qui ne le sera pas.

<h4>Sera traité</h4>

 * Les raisons expliquant le besoin de visualiser les algorithmes d'apprentissage automatique
 * Les difficultés
 * z

<h4>Ne le sera pas</h4>

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec placerat odio eu lacus molestie, a interdum nisi lacinia. Etiam faucibus ac sem et congue. Vestibulum et imperdiet odio. Nunc lacus risus, finibus quis elementum sit amet, posuere non justo. Donec faucibus turpis eget magna aliquam pellentesque. Fusce ac rutrum nisi. Maecenas feugiat euismod elit, eu egestas felis dignissim sed. Integer felis leo, blandit at augue in, porta blandit urna.

<a href="{{site.baseurl}}/{% post_url 2019-02-03-visualiser-un-algorithme %}">Partie 1 : Peut-on visualiser un algoithme ?</a>

## Références

[^1]: Donald Norman Artefacts cognitifs Norman
[^2]: <https://books.google.fr/books?id=wdh2gqWfQmgC&printsec=frontcover&hl=fr#v=onepage&q&f=false]>
[^3]: <https://www.larousse.fr/dictionnaires/francais/algorithme/2238]>
[^4]: <http://www.cs.ubbcluj.ro/~gabis/ml/ml-books/McGrawHill%20-%20Machine%20Learning%20-Tom%20Mitchell.pdf]>
