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

# Préliminaires

Parmi les différents types d'ondes qu'on peut étudier en séance de travaux pratiques, les ondes à la surface de l'eau présentent l'avantage de s'observer très facilement. A l'inverse, leur étude théorique est relativement complexe, c'est pourquoi, nous nous tiendrons dans ce TP à une étude descriptive des ondes. Il s'agira d'observer plusieurs phénomènes liés aux ondes:

* leur propagation: de la simple observation à l'obtention de leur vitesse de propagation.
* leur forme: onde plane et onde circulaire.
* les phénomènes d'interférences et de diffraction d'une onde.

Pour étudier de telles ondes, on utilisera un dispositif particulièrement adapté: la cuve à onde.

## Dispositif
On dispose à la surface de l'eau qui remplit la cuve (\cref{fig_cuve_a_ondes}) une pointe ou une tige reliée à un dispositif pneumatique permettant sa vibration et donc la création d'ondes de surfaces. L'excitation peut-être soit unique au moyen d'une g\^achette de contrôle qu'on branche sur l'alimentation, soit périodique (débrancher la g\^achette) en réglant la fréquence d'excitation et l'amplitude sur le bloc alimentation.

```{figure} ./images/Signaux_Cuve_A_Ondes.jpg
:name: cuve_ondes
:align: center
Cuve à ondes
```

Contrairement au schéma proposé, le bloc d'alimentation du vibreur est confondu avec le projecteur stroboscopique. Cela permet notamment de synchroniser la fréquence du stroboscope et du vibreur. Il faut aussi noter que l'excitation périodique n'est activer que si la g\^achette de contrôle est débranchée du bloc.

```{figure} ./images/Signaux_Ombroscopie.jpg
:name: ombroscopie
:align: center
Effet de lentille des vagues
```

Gr\^ace qu dispositif de la cuve à ondes, on réalise une projection par ombre (ombroscopie). Une convexité à la surface de l'eau joue le rôle de lentille convergente (Figure A.2), alors qu'une concavité jouera le rôle d'une lentille divergente. Ainsi, on observe sur le dépoli des zones d'ombre et des zones de lumière suivant que le faisceau lumineux traverse une région concave ou convexe.


