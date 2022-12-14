# Programmation

La programmation (ou codage) consiste à écrire des programmes informatiques.

Ecrire un programme, c'est donner des instructions à un ordinateur pour qu'il l'exécute à notre place.

## Langage de programmation

La langue utilisée pour écrire le programme est appelé un langage de programmation.

Pour qu'il soit compris par l'ordinateur, le programme doit suivre les règles de syntaxes et d'orthographes défini par le langage.

## Exécution d'un programme

L'ordinateur va lire ligne par ligne le programme donné et dans chaque ligne, lire tous les caractères qui la compose.

Il vérifie tout d'abord si le programme suit bel et bien les règles définies par le langage, puis exécute le programme ligne par ligne.

> Vous pouvez exécuter votre code sur [l'éditeur Gymnacode](https://gymnacode.blueur.com/editor). 

## Calcul & Expression

Une des fonctionnalités primaires du programme est de pouvoir faire des calculs. La syntaxe est la suivante : `expr op expr`

- `expr` est une **expression** qui peut être une valeur (p. ex. `42`, `3.14`, `"bleu"`, ...) ou un calcul (p. ex. `3 + 4`)
- `op` est une **opération** qui sera représenté par un ou plusieurs caractère (p. ex. `+`, `-`, `**`, ...)

### Evaluation

L'expression `3 + 4 - 2` sera évalué en deux étapes car elle est composée de deux calculs :

$$ \underbrace{\underbrace{3\ +\ 4}_{=7}\ -\ 2}_{=5} $$

## Variable

Une variable permet de stocker une valeur pour pouvoir la récupérer plus tard. La syntaxe est la suivante : `var = expr`

- `var` étant le nom (identifiant) de la variable

Une expression peut aussi être une variable : la valeur courante de la variable sera donc utilisée pour l'évaluation. 

```python
a = 3 # crée la variable 'a' qui contient la valeur 3

4 + a # sera évalué à 7

a + a # sera évalué à 6

a = 13 + a # remplace la valeur de la variable 'a' par la valeur 16

a / 2 # sera évalué à 8
```

## Print

La fonction `print` permet d'afficher quelque chose dans la console pour l'utilisateur. La syntaxe est la suivante : `print(expr)` ou `print(expr, expr, expr, ...)`

L'appel d'une fonction se fait à travers son identifiant (ici `print`) suivi de `()` avec zéro, une ou plusieurs arguments séparés par des virgules à l'intérieur des parenthèses. Chaque argument est une expression. 

```python
print() # Imprime une ligne vide

print(3) # Imprime '3' puis un retour à la ligne

print(6, 12) # Imprime '6 12' puis un retour à la ligne

a = 32
print(a, 4 - 2) # Imprime '32 2' puis un retour à la ligne
```

## Type

Chaque expression a un type. Le type défini la nature des valeurs possibles et par extension les opérations qui peuvent être appliquées à l'expression. 

```python
entier = 42 # a un type 'int'

decimal = 3.14 # a un type 'float'

texte = "Bonjour !" # a un type 'str'

booleen = True # a un type 'bool'
```

Les opérateurs peuvent avoir des significations différentes suivant le type des expressions des opérandes :

- `int + int` sera un `int` (opération arithmétique)
- `int - float` sera un `float` (opération arithmétique entre un `int` et un `float` va donner un `float`)
- `int / int` sera un `float` (une division donne un `float`)
- `str + str` sera un `str` (concatenation entre deux chaines de caractères)
- `str + int` erreur !

## Saisie

Pour demander des informations à l'utilisateur, on utilise la fonction `input` qui peut prendre 0 ou 1 argument. 

Cette fonction va faire attendre le programme jusqu'à ce que l'utilisateur entre une chaine de caractère et appuie sur ENTER. 

L'argument, s'il y a, doit être de type `str` et détermine qui sera affiché à l'utilisateur ce qu'on attend de lui. 

La valeur retournée par `input` sera toujours de type `str`. 

```python
input() # attend un texte de l'utilisateur

input("Quel est votre nom ?") # affiche 'Quel est votre nom', puis attend un texte de l'utilisateur

nom = input("Quel est votre nom ?") # met la valeur entrée par l'utilisateur dans la variable 'nom'

texte = input("Quel âge avez-vous ?") # Peu importe la question, le type de la variable sera toujours une 'str'
```

---

[Retour à l'accueil](../README.md)
