---
layout: post_site
title: "3 - Expliquer l'apprentissage automatique"
date: 2019-02-01 12:04:32 +0100
---

Nous nous plaçons donc dans le cadre d'algorithmes dont l'opacité est uniquement liée à sa manière d'opérer. Plusieurs questions vont donc se poser. En effet, expliquer le fonctionnement de l'algorithme va dépendre du public de destination et de la visée. Nous allons donc explorer les objets, modes et moment de visualisation d'un algorithme d'apprentissage automatique. Nous choisissons de focaliser l'étude sur les réseaux de neurones convolutionnels.


<div>
<img src="{{site.baseurl}}/assets/img/cnn.png" style="display: block; margin-left: auto; margin-right: auto; width:80%">
<h5 style="text-align:center">Figure 1 : Schéma d'un réseau de neurones convolutionnels</h5>
</div>

## Que représenter ?

Nous pouvons distinguer quatre grands aspects visualisable d'un réseau de neurones :

* <b>Architecture du modèle</b> : L'architecture du modèle peut tout d'abord être représentée. Celle-ci permet de représenter comment les données se propagent dans le modèle. Cette représentation peut inclure la représentation des liens au matériel ainsi qu'aux sauvegardes et logs effectuées.

* <b>Paramètres appris</b> : Les paramètres appris lors de l'entrainement peuvent être représentés. Les poids des neurones peuvent être comparés de même que l'évolution des filtres de convolution.
Poids et filtres de convolution

* <b>Étapes du processus</b> : Au cours des passes avant et retour d'un réseau de neurones, certains évènements peuvent être visualisés. La valeur d'activation de chaque noeud du réseau peut permettre d'évaluer le "niveau d'utilisation" d'un neurone. Le processus de rétro-propagation peut être visualisé à chaque couche du réseau pour montrer comment l'erreur est distribuée sur les paramètres du réseau.

* <b>Les données aggrégées</b> : Enfin, des données aggrégées peuvent être obtenues, particulièrement lors de l'entrainement, comme les valeurs de perte ou la précision de prédiction des classes au fil des epochs. Ces données sont généralement représentées en fonction du temps afin d'évaluer l'avancement de l'entraînement. Ces données sont particulièrement intéressantes car elles permettent de comparer des modèles très différents.

## Quand ?

Dans le cadre d'un algorithme d'apprentissage automatique, se pose la question du moment de la représentation, pendant ou après l'entrainement. Ainsi, dans le cas d'un réseau de neurones :

* <b>Pendant l'entraînement</b> : Visualiser un modèle pendant l'entrainement permet d'observer l'évolution de sa performance et potentiellement détecter des problèmes comme l'overfitting. Ces visualisations peuvent ainsi permettre de gagner du temps en arrêtant des entrainements qui ne mèneraient à rien.

* <b>Après l'entraînement</b> : Visualiser les sorties du système, les features apprises ou l'état final des poids. Cela permet en particulier de comparer différents modèles sur lesquels les hyperparamètres ont varié.

## Comment ?

# Node-link diagrams

Une première idée de représentation des réseaux de neurones est la visualisation par noeuds et liens. Cela permet de montrer comment sont reliés les neurones et la manière dont ils s'influence. Les visualisations les plus simples sont statiques et utilisent la couleur et l'épaisseur des liens pour encoder des valeur d'activation et l'influence de certains neurones.

Dans la représentation ci-dessous, un réseau de neurones simple, avec une couche cachée est visualisée. Il est destiné à repérer l'appartenance d'un pixel au cerveau sur une IRM.

<div>
<img src="{{site.baseurl}}/assets/img/nn_irm.png" style="display: block; margin-left: auto; margin-right: auto; width:70%">
<h5 style="text-align:center">Figure 2 : Visualisation des valeurs des neurones d'entrée et de sortie pour une classification du cerveau sur une IRM. p correspond aux position (x,y,z), n à des informations sur les pixels environnants, g et s sont des paramètres d'IRM. [^2]</h5>
</div>

Il est remarquable que les entrées n'aient pas la même influence sur le résultat final en fonction de la position du pixel analysé. En effet, le système n'utilise que les informations de position pour prédire le résultat d'un pixel situé au niveau de la machoire. Au contraire, un pixel dans le cerveau utilisera presque toutes les informations disponibles pour valider le résultat.

<b>Cependant, la visualisation, par sa staticité, devient difficile à exploiter pour un réseau de neurones plus complexe.</b> D'autres visualisation s'intéressent au contraire à rendre explorable le réseau afin de laisser l'utilisateur adapter la densité visuelle d'information présentée.

L'outil <b>TensorBoard</b>, permet de représenter un réseau implémenter en TensorFlow. La représentation est toujours faite de noeuds et de liens, mais elle permet d'explorer le réseau et d'agrandir le niveau de détails sur certains noeuds.

<div>
<img src="{{site.baseurl}}/assets/img/tensorboard.gif" style="display: block; margin-left: auto; margin-right: auto; width:90%">
<h5 style="text-align:center">Figure 3 : Démonstration des possibilités d'exploration au sein d'un node-link diagram sur l'outil TensorBoard. [^3]</h5>
</div>

# Scatter plots

# Line charts

# Feature visualization

Saliency maps

# Représentations intéractives mixtes

ConvNetJS https://cs.stanford.edu/people/karpathy/convnetjs/

http://scs.ryerson.ca/~aharley/vis/conv/

http://experiments.mostafa.io/public/ffbpann/




ShapeShop https://github.com/fredhohman/shapeshop

<a href="{{site.baseurl}}/{% post_url 2019-01-30-limites-de-la-demarche %}">Partie 4 : Limites de la démarche</a>

## Références

[^1]: Fred Hohman & al, <https://arxiv.org/pdf/1801.06889.pdf>
[^2]: www.idav.ucdavis.edu/func/return_pdf?pub_id=869
[^3]: https://www.youtube.com/watch?v=eBbEDRsCmv4
