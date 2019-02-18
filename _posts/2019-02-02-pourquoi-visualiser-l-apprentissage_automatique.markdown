---
layout: post_site
title: "2 - Pourquoi visualiser l'apprentissage automatique ?"
date: 2019-02-02 12:04:32 +0100
---
Les algorithmes d'apprentissage automatique diffèrent fondamentalement des algorithmes conventionnels. Peter Norvig, directeur de la recherche chez Google[^1], justifie ainsi le besoin de mieux comprendre l'apprentissage automatique.

<p style="text-align: center">
  <i>"On the traditional software model, we have a programmer they create a bunch of rules, they write them down, they try to get all the rules right, it's hard to do right because there's complexity. <b>In machine learning models, it's not a programmer that writes the program, it's a machine that writes the program and how does the machine know to write the program? Trough data.</b> You show it lots of examples, you give it a model that says "this is what I think the world is like" and then you tell the system : "arrange it so that in the future you'll do things similar to the examples you saw in the past. And then, outcomes what's mostly a black box. So you give examples in, what comes out is a program that will do the right thing. You're note quite sure exactly how it works. But it's a black box with a leed that's open because we can peer inside it and one of the big challenges now is, how do you peer inside and how do you understand what's been written by this machine." </i>[^2]
</p>

Par ailleurs, il faut distinguer l'apprentissage et
Ainsi, le développeur d'un algorithme d'apprentissage automatique n'en implémente que partiellement la logique.

Ainsi, quand un ordinateur créé l'algorithme, il devient difficile d'en cartographier la logique. Tout devient beaucoup plus opaque, nous sommes alors incapables d'expliquer comment et pourquoi le programme produit un certain résultat.


## Des enjeux : vitaux et omniprésents

Liste des critères à optimiser : [^3]
* Fairness
* Unbiasedness
* Privacy
* Reliability
* Robustness
* Causality
* Usability
* Trusted

## Un problème : l'opacité de l'apprentissage automatique

Faire un point sur le droit à l'explication existant dans la RGPD.

Jenna Burrell, professeure à Berkeley, s'intéresse à l'interprétabilité des algorithmes d'apprentissage automatique. Elle distingue trois catégories d'opacité associées à ces algorithmes[^3].

* <b>Opacité intentionnelle par discrétion</b> : certains algorithmes d'apprentissage automatique peuvent avoir leur code protégé par leurs propriétaires. Ces derniers peuvent ainsi chercher à conserver un avantage compétitif ou assurer la performance de leur produit (ex : un filtre de spam ne sera pas efficace si les responsables de ces mêmes spams savent exactement comment vous vous en protégez). Ce type d'opacité est volontaire et peut se justifier. Si besoin le régulateur peut demander l'audit ou l'ouverture du code au public.
* <b>Opacité technologique</b> : les algorithmes d'apprentissage automatique sont implémentés dans des languages informatiques. Ces languages ne sont intelligibles que par un fragment de la population ce qui rend les algorithmes inaccessibles pour beaucoup. Par ailleurs, une grande latitude est laissée à tout développeur. Cela signifie qu'un même programme pour la machine pourra être rédigé d'une manière qui facilite ou empêche la lecture. Ce type d'opacité est malheureux mais est indépendante de l'algorithme. L'éducation à la bonne rédaction de code et l'enseignement de sa compréhension sont les seules armes à notre disposition.
* <b>Opacité opérationnelle</b> : les algorithmes d'apprentissage automatique reposent sur une intéraction entre des données et des règles de modélisation. Ce dernier type d'opacité est du à notre incapacité à comprendre la dynamique qui allie les données et les règles dans le processus d'apprentissage. <b>C'est ce type d'opacité que nous nous proposons de traité dans la suite de cette étude.</b>

Exemple de l'organigramme d'une entreprise

Définition de l'interprétabilité :
<p style="text-align: center">
  <i>"Ability to explain or to present in understanding terms to a human."</i>[^3]
</p>

Il est possible que nous n'ayons pas besoin d'expliquer le contenu et fonctionnement d'une boite noire :
* Conséquences faibles : les résultats innacceptables n'entrainent pas de problèmes majeurs.
* La boite noire n'évolue pas et est suffisamment étudiée et testée en cas d'application réel.

## Quatre raisons de visualiser l'apprentissage automatique

Nous pouvons distinguer quatre raisons de visualiser le deep learning :[^4]

1. Interprétabilité :  [critique de sa définition] et volonté d'explication
2. Optimisation : Débuggage et amélioration
3. Comparaison : et sélection de modèles
4. Enseignement : Enseigner le deep learning


<a href="{{site.baseurl}}/{% post_url 2019-02-01-expliquer-l-apprentissage-automatique %}">Partie 3 : Rendre compte du fonctionnement des algorithmes de machine learning</a>

## Références

[^1]: Google Research, <https://ai.google/research/people/author205>
[^2]: Peter Norvig, USI 2015, (3:10 - 4:10) <https://www.youtube.com/watch?v=BJ2QVzGmb2w>
[^3]: Jenna Burrell, <https://journals.sagepub.com/doi/10.1177/2053951715622512>
[^4]: Fred Hohman & al, <https://arxiv.org/pdf/1801.06889.pdf>
