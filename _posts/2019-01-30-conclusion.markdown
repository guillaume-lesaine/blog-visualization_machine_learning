---
layout: post_site
title: "Conclusion"
date: 2019-01-29 12:04:32 +0100
permalink: "conclusion"
---

Pour terminer cet exposé, nous souhaitons nous arrêter sur quelques limites et perspectives associées à la visualisation des algorithmes d'apprentissage automatique. Nous avons vu précédemment que la visualisation peut permettre de représenter des algorithmes au sens large. Nous avons par ailleurs montré que les algorithmes d'apprentissage automatique posaient de nombreuses questions sociétales et techniques, les plaçant au coeur de l'attention du public et des politique. Nous avons enfin abordé le cas d'un algorithme d'apprentissage automatique, les réseaux de neurones convolutionnels, et exposés quelques visualisations possibles pour les rendre plus compréhensibles.

# Limites de la démarche

La première conclusion qu'on pourrait tirer est que les algorithmes d'apprentissage automatique peuvent être mieux compris grâce à la visualisation de données. Cela est vrai, l'acquisition de donnés d'entrainement et fonctionnement ainsi que leur représentation permettent de réprésenter les mécanismes internes des modèles et comment ils agissent sur les données. Cependant de nombreuses limites existent.

* <b>Un problème de visualisation</b> - Nous savons extraire des données de l'entrainement et du fonctionnement des modèles. Ces données sont très variables dans le sens qu'on y associe, leur dimension et leur corrélation. Par ailleurs les publics potentiels de ces visualisations varient grandement dans leur connaissance technique. Ainsi un compromis est à trouver entre le choix des données représentées ou la densité de visualisation et, le caractère explicatif et universel de la représentation.
* <b>Un besoin de traitement au cas par cas</b> - De très nombreux modèles d'apprentissage automatique existent. Par ailleurs, ces modèles ne peuvent être dissocié des données d'entrainement et de test utilisés. Ainsi, une réponse générale à la représentation d'un modèle, indépendante des données semble difficile. Par ailleurs, comme évoqué précédemment, le besoin de satisfaire une variété de publics nécessite en définitive un traitement adapté et unique pour un couple (modèle,données).
* <b>Des compétences rares et couteuses</b> - La représentation de l'apprentissage automatique requiert des compétences techniques relativement rares comme une large connaissance des modèles et de leur fonctionnement, ainsi que des compétences en visualisation. Aucune de ces expertises n'est simple à acquérir. Il semblerait tout de même, qu'il soit plus simple pour un expert en apprentissage automatique de se tourner vers la visualisation que la situation inverse. Néanmoins, les compétences techniques précédentes ne suffisent sans doute pas. En effet, des experts métiers, sociaux et légaux pourraient être utilent dans le processus de conception et utilisation d'une visualisation de modèle. La nécessité de combiner des équipes pluridisciplinaires d'expert s'accompagnera de coups considérables.

# Perspectives

Bien que la représentation des algorithmes d'apprentissage automatique connaisse de nombreuses limites, le développement constant des algorithmes ne nous laisse pas le choix. Nous avons besoin de mieux comprendre et encadrer le fonctionnement des algorithmes. Des initiatives existent comme aux États-Unis où la <b>DARPA</b> (Defense Advanced Research Projects Agency) a récemment lancé un programme d'ampleur pour rendre l'apprentissage automatique plus explicables grâce à une meilleur compréhension des modèle et un développement des moyens pour les représenter.[^1]

En France, le rapport rédigé par <b>la commission dont Cédric Villani était à la tête</b> (2018), lance de nombreuses pistes de réflexion sur l'éthique de l'intelligence artificielle. Cinq principes sont évoqués comme les piliers de la réflexion[^2].

* Développer les capacités nécessaires pour comprendre et auditer le fonctionnement des modèles et investir dans la recherche sur l'explicabilité.
* Adapter la loi pour d'une part, mieux protéger les citoyens des abus potentiels liés à l'utilisation de l'apprentissage automatique, d'autre part assurer que les organisations déployant les modèles soient tenues responsables.
* Adapter la formation des architectes de modèles afin de les rendre conscients des effets négatifs des technologies qu'ils développent.
* Constituer une instance de débat permettant à la population de statuer régulièrement sur l'apprentissage automatique que nous souhaitons, ainsi que sa dose d'application.
* Faire une place à l'intelligence artificiel dans le débat et la vie politique au travers d'une chambre destinée à réfléchir sur les impacts sociétaux des technologies associées.

Bien qu'assez généraux, ces principes pourraient trouver des concrétisations à moyen terme. À titre d'exemple, nous pouvons ici citer la proposition de création d'un "corps d'experts dotés des compétences requises [...] pour procéder à des audits d'algorithmes et de bases de données sur pièce, et procéder à des test par tout moyen requis"[^2]. Cette proposition permettrait par exemple d'offrir des audits forts dans le cas de contentieux.

## Références

[^1]: DARPA, [Explainable AI](https://www.darpa.mil/program/explainable-artificial-intelligence)
[^2]: Cédric Villani, Donner un sens à l'intelligence artificielle, [rapport](https://www.aiforhumanity.fr/pdfs/9782111457089_Rapport_Villani_accessible.pdf), 2018
