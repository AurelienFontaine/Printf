# Printf

Ce projet est une ré-implémentation de la fonction `printf` en C, réalisée dans le cadre de mon apprentissage de la programmation bas niveau. Il s'agit d'un exercice classique permettant de comprendre la gestion de la mémoire, la manipulation des chaînes de caractères, la gestion des arguments variadiques et l'affichage formaté.

## Objectif

Reproduire le comportement de la fonction standard `printf` en C, en prenant en charge plusieurs types de conversions :
- Caractères (`%c`)
- Chaînes de caractères (`%s`)
- Entiers signés (`%d`, `%i`)
- Entiers non signés (`%u`)
- Hexadécimal minuscule et majuscule (`%x`, `%X`)
- Pointeurs (`%p`)
- Le caractère `%` lui-même

## Fichiers principaux

- `ft_printf.c` : Fonction principale et gestion du parsing du format.
- `ft_printf.h` : Fichier d'en-tête avec les prototypes et définitions.
- `ft_print_char_str_nbr.c` : Fonctions d'affichage pour les caractères, chaînes et nombres.
- `ft_printHexa.c` : Gestion de l'affichage en hexadécimal.
- `ft_printptr.c` : Affichage des pointeurs.
- `ft_printunsigned.c` : Affichage des entiers non signés.
- `ft_itoa.c` : Conversion d'entiers en chaînes de caractères.
- `Makefile` : Compilation du projet.

## Compilation

Pour compiler le projet, utilisez la commande suivante :

```bash
make
```

Cela génèrera une librairie statique `libftprintf.a` (ou un exécutable selon la configuration du Makefile).

## Utilisation

Incluez le fichier d'en-tête dans votre projet :

```c
#include "ft_printf.h"
```

Utilisez ensuite `ft_printf` comme la fonction standard :

```c
ft_printf("Hello %s!\n", "world");
```

## Pourquoi ce projet ?

Ce projet m'a permis de :
- Approfondir ma compréhension du C et de la gestion mémoire
- Manipuler les arguments variadiques (`va_list`)
- Gérer différents types de données et conversions
- Améliorer la robustesse et la lisibilité de mon code

## Auteur

Aurelien Fontaine

N'hésitez pas à me contacter pour toute question ou suggestion !