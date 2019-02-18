---
layout: post_site
title: "3 - Expliquer l'apprentissage automatique"
date: 2019-02-01 12:04:32 +0100
---

## À qui expliquer ?

On peut distinguer trois types de destinataires de la visualisation du deep learning

<div>
<img src="{{site.baseurl}}/assets/img/personas.png" style="display: block; margin-left: auto; margin-right: auto; width:100%">
<h5 style="text-align:center">Figure 1 : Les destinataires de la visualisation du deep learning[^1]</h5>
</div>


* Architectes : développeurs de modèles
* Entraineur : utilisateurs de modèles
* Utilisateur final : grand public

## Que représenter ?

# Architecture du modèle

Graph des flux de données (computational graph)

# Paramètres appris

Poids et filtres de convolution

# Parties du processus

L'activation et le fonctionnement de la rétro-propagation permettant, à chaque passe aller d'observer comment est distribuée l'erreur.

# Les données aggrégées

Métriques classiques (ce sont essentiellement des séries temporelles)(souvent utilisées pour controller l'avancement de l'entrainement) : perte, précision

Données particulièrement intéressantes car elles permettent de comparer des modèles.

## Comment ?

## Quand ?

# Pendant l'entraînement

# Après l'entraînement

## Quels outils à notre disposition ?

Certains outils ont déjà permis d'illustrer les parties précédentes. Nous pensons néanmoins que chaque type de destinataire de visualisation de deep learning peut retenir quelques outils :

<a href="{{site.baseurl}}/{% post_url 2019-01-30-limites-de-la-demarche %}">Partie 4 : Rendre compte du fonctionnement des algorithmes de machine learning</a>

## Références

[^1]: Hendrik Strobelt & al,<https://arxiv.org/pdf/1606.07461.pdf>
[^2]: Fred Hohman & al, <https://arxiv.org/pdf/1801.06889.pdf>
[^3]:
[^4]:
