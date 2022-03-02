### Ce qu’il faut savoir

#### Notion de variable

- on associe une valeur présente en mémoire à un nom. C’est cette association “valeur - nom” que l’on appelle variable.

- Plusieurs types de valeurs peuvent être associé à un nom : les entiers (int), les
nombres à virgule (float), les chaînes de caractères (string), les booléens (bool)...

#### Opérations arithmétiques

Il est possible d’effectuer des opérations arithmétiques : + addition ; - soustraction ; *
multiplication ; % modulo (reste de la division euclidienne)... Ces opérations peuvent être
directement effectuées sur des valeurs (int ou float) ou sur des variables.

#### Concaténation des chaînes de caractères

Le signe + est aussi utilisé pour effectuer une concaténation (mettre bout à bout au moins
deux chaînes de caractères)

#### Les fonctions

Les fonctions permettent de décomposer un programme complexe en une série de
sous-programmes plus simples. Les fonctions sont réutilisables et évitent de se “répéter” dans un programme

#### Les conditions

```
if expression :
	suite_instruction1
else :
	suite_instruction2
```

Si "expression" est True alors "suite_instruction1" est exécuté et"suite_instruction2" est
ignoré. Sinon (sous-entendu que "expression" est False) "suite_instruction2" est exécuté et
"suite_instruction1" est ignoré.

#### La boucle while

Une boucle permet d'exécuter plusieurs fois des instructions qui ne sont présentes qu'une
seule fois dans le code.

La structure de la boucle while est la suivante :

```
while expression:
	instruction1
	instruction2
suite programme
```

Tant que l'expression s'évalue à "True", les instructions à l'intérieur du bloc (partie indentée) seront exécutées.

### Ce qu’il faut savoir faire

- savoir créer et utiliser des variables

- savoir effectuer des opérations arithmétiques

- savoir effectuer une concaténation

- savoir écrire et utiliser des fonctions avec et sans paramètre ; avec et sans valeur de
retour (mot clé “return”)

- savoir écrire et lire une condition (if / else)

- savoir écrire et lire une boucle while