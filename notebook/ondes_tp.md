---
jupytext:
  encoding: '# -*- coding: utf-8 -*-'
  formats: ipynb,md:myst
  split_at_heading: true
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.10.3
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Travaux pratiques
L'émetteur ultrasons a déjà été utilisé dans le premier TP. Se référer à ce TP pour son utilisation.

Les ultrasons sont des ondes sonores dont l'étude présente l'avantage de n'\^etre pas audible par l'oreille humaine (la fatigue auditive est donc moins importante à la fin du TP ou lorsqu'on fait une marche arrière avec un radar de recul!). Elles sont néanmoins des ondes sonores qui peuvent \^etre émises, se propager et \^etre reçues par un récepteur adéquat. On peut donc faire l'étude de la propagation des ondes acoustiques.

## Influence de la fréquence d'échantillonnage

````{admonition} Manipulation
:class: tip
1. Choisir un mode d'émission continu pour l'émetteur. Choisir correctement une durée d'acquisition sachant que la fréquence du signal à observer est autour de 40kHz.
2. Observer le signal excitateur de l'émetteur sur l'Atelier Scientifique en mode d'acquisition unique en imposant une période d'échantillonage de 0,25$mu$s et mesurer la fréquence du signal de deux manières:
    * Par une mesure directe de la période temporelle.
    * En demandant le tracé du spectre du signal (Calculs $\longrightarrow$ Transformée de Fourier).
3. Est-ce un signal sinusoïdal? Répondre en analysant l'évolution temporelle puis le spectre de Fourier. Obtenir les caractéristiques des composantes spectrales gr\^ace à la transformée de Fourier.
4. Procéder aux m\^emes mesures pour des périodes d'échantillonnage: 2,5$mu$s et 25$mu$s. Commenter notamment la fréquence des ultrasons mesurées sur le spectre de Fourier.

````

## Effet de la transduction
````{admonition} Manipulation
:class: tip
Placer un récepteur juste en face de l'émetteur et acquérir les deux signaux émissions et réception en mode d'acquisition continu. L'amplitude du signal reçu dépend-elle de la fréquence de l'émetteur? Si oui, régler la fréquence de manière à observer un maximum d'amplitude pour le récepteur. Comparer de deux manières les deux signaux (préciser les méthodes). Quels sont alors les points communs et les différences? D'où viennent-elles?
````

## Propagation d'un signal ultrasonore dans l'air

Pour les expériences à venir, on se servir intelligemment des deux récepteurs et du rail double. On réfléchira au
mode d'émission (continu ou salve) préférable et on s'entra\^inera à travailler avec le mode d'acquisition continu. 

Le but est de vérifier la relation de dispersion $c = f\lambda$. On allons mesurer les trois grandeurs séparément puis tester le rapport $\frac{c}{\lambda f}$.

````{admonition} Mesure de la longueur d'onde
:class: tip
1. En vous aidant de la définition de la longueur d'onde, proposer un protocole expérimental utilisant les deux récepteurs et permettant de mesurer la longueur d'onde des ultrasons émis.
2. Faire un bilan des sources d'erreurs. Commenter le caractère a priori négligeable/prépondérant des sources. Réfléchir alors à une manière simple de diminuer l'incertitude de mesure.
3. Réaliser l'expérience et mesurer la longueur d'onde du signal avec son incertitude. On précèdera à une propagation des variances.

````

````{admonition} Mesure directe de la célérité des ultrasons
:class: tip
1. Proposer un protocole expérimentale permettant de mesurer directement la célérité de l'onde. Elle devra s'appuyer sur 5 mesures.
2. Réaliser la mesure de la célérité avec son incertitude.
````

````{admonition} Exploitation
:class: tip
Estimer le rapport $\eta = \frac{c}{\lambda f}$ ainsi que son incertitude (par propagation des variances) et vérifier que la relation de dispersion est bien vérifiée.
````