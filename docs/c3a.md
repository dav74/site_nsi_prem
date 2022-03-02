### activité 3.1

Il est possible d'afficher le contenu d'un dictionnaire dans la console.

Tapez la ligne suivante dans la partie éditeur de Spyder ou de basthon :

```
mes_fruits = {"poire": 3, "pomme": 4, "orange": 2}
```
après avoir exécuté le "programme" ci-dessus, tapez  *mes_fruits* dans la partie console. Vous devriez alors voir s'afficher le contenu (clés et valeurs) du dictionnaire.

### activité 3.2

```
d = {"voiture": 25, "vélo": 55, "train": 20}
tr = d['vélo']
```
Quelle  est la valeur de la variable *tr* après l'exécution du programme ci-dessus. Vérifiez votre réponse à l'aide de la console.

### activité 3.3

```
tab = []
d = {"voiture": 25, "vélo": 55, "train": 20}
for t in d.values():
	if t < 40 :
		tab.append(t)
```
Quelle est la valeur de la variable *tab* après l'exécution de  ce programme. Vérifiez votre réponse à l'aide de la console.

### activité 3.4

```
tab = []
d = {"voiture": 25, "vélo": 55, "train": 20}
for v,t in d.items():
	if t < 40 :
		tab.append(v)
```
Quelle est la valeur de la variable *tab* après l'exécution de  ce programme. Vérifiez votre réponse à l'aide de la console.


### activité 3.5

```
tab = [{'nom': 'toto', 'num': 2}, {'nom': 'titi', 'num': 5},  {'nom': 'tata', 'num': 4}]
tab_nom =  []

for t in tab :
	if t['num'] > 3:
		tab_nom.append(t['nom'])
```
Quelle est la valeur de la variable *tab_nom* après l'exécution de  ce programme. Vérifiez votre réponse à l'aide de la console.

### activité 3.6

On utilise un tableau contenant des dictionnaires afin de stocker les  notes des élèves Titi, Toto et Tutu :

```
[{'nom':'Titi', 'note':12}, {'nom':'Tutu', 'note':11}, {'nom':'Toto', 'note':17}]
```

La fonction *plusHaute* prend en paramètre un tableau contenant des dictionnaires (comme celui ci-dessus) et renvoie le nom de l'élève ayant obtenu la meilleure note (on partira du principe que les élèves ont tous des notes différentes).

```
def plusHaute(tab):
	nom = ""
	max_note = ...
	for t in ...:
		if t['note'] > ...:
			max_note = t[...]
			nom = t[...]
	return ...
```
			
Complétez la fonction *plusHaute*

### activité 3.7

On utilise un tableau et des dictionnaires pour stocker des noms et des numéros  de téléphone :

```
[{'nom':'Titi', 'num':987675643}, {'nom':'Tutu', 'num':424224}, {'nom':'Toto', 'num':343235365}]
```

La fonction *numTel* prend 2 paramètres :

- un tableau de dictionnaires *tab_tel* contenant les noms  et les numéros de téléphone (comme celui ci-dessus)
- un nom *n*

La fonction *numTel* doit renvoyer le numéro de téléphone de *n* si ce dernier existe. Dans le cas où *n* n'existe pas, la  fonction *numTel* doit renvoyer -1

```
def numTel(n, ...):
	for ... in tab_tel:
		if ...  == t['nom']:
			return ...
	return ...
```

### activité 3.8

On utilise un tableau contenant des dictionnaires afin de stocker les  notes des élèves Titi, Toto et Tutu :

```
[{'nom':'Titi', 'note':12}, {'nom':'Tutu', 'note':11}, {'nom':'Toto', 'note':17}]
```
La fonction *moyenne* prend en paramètre un tableau contenant des dictionnaires (comme celui ci-dessus) et renvoie la moyenne des notes.

Écrivez la fonction *moyenne*
 