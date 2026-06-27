# Simulations et probabilités

## Objectif

Utiliser une simulation pour estimer une probabilité et distinguer fréquence observée
et probabilité théorique.

## Principe

Une simulation reproduit une expérience aléatoire un grand nombre de fois.

La fréquence d’un événement est :

$$
\text{fréquence}=\frac{\text{nombre de réalisations de l’événement}}
{\text{nombre total d’expériences}}.
$$

Quand le nombre d’essais augmente, la fréquence a tendance à se rapprocher de la
probabilité théorique. Elle ne devient pas forcément exactement égale.

## Algorithme type

```text
succès ← 0
répéter 1000 fois
    tirage ← entier aléatoire entre 1 et 6
    si tirage est supérieur à 4 alors
        succès ← succès + 1
afficher succès / 1000
```

La sortie estime la probabilité d’obtenir 5 ou 6 avec un dé, dont la valeur théorique
est $2/6=1/3$.

## Erreurs fréquentes

- croire qu’une simulation prouve exactement une probabilité ;
- oublier de remettre à zéro le compteur ;
- diviser par le nombre de succès au lieu du nombre total d’essais ;
- générer des valeurs qui ne correspondent pas à l’expérience.

