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
(polyfit_variance)=
# Polyfit avec la propagation des variances
Il n'est pas nécessaire de réaliser un calcul supplémentaire pour estimer l'incertitude-type de la pente et de l'ordonnée à l'origine car la fonction offre la possibilité de le faire.

On utilise la signature :

```ipython
pars, V = np.polyfit(X, Y, 1, cov=True)
```

`V` est alors une matrice numpy. L'intertitude-type sur la pente s'obtient alors par $u(Y) \times \sqrt{V[0][0]}$ et l'intertitude-type sur l'ordonnée à l'origine s'obtient alors par $u(Y) \times \sqrt{V[1][1]}$.

````{attention}
Cette méthode a l'air simple MAIS :
* elle n'est pas au programme, celle que vous devez connaître est la méthode de Monte-Carlo. On l'utilise ici simplement pour montrer comment on ferait avec la propagation des variances
* elle est imprécise car elle suppose que $u(Y)$ est le même pour chaque mesure (il faudra prendre une moyenne) et ne tient pas compte des incertitudes sur les abscisses. La multiplication par $u(Y)$ est n'est d'ailleurs pas forcémentr valable suivant les cas.

Il est donc important de maitriser la méthode de Monte-Carlo pour obtenir l'incertitude après régression linéaire.
````