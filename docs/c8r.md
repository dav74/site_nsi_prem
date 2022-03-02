### Ce qu’il faut savoir

#### Des transistors aux circuits complexes
- à la base de la plupart des composants d'un ordinateur, on retrouve le transistor.

- dans un ordinateur, les transistors sont regroupés au sein de ce que l'on appelle des circuits intégrés. Dans un circuit intégré, les transistors sont gravés sur des plaques de silicium

- dans un ordinateur les transistors se comportent comme des interrupteurs : soit le transistor laisse passer le courant électrique (interrupteur fermé, état haut), soit il ne le laisse pas passer (interrupteur ouvert, état bas).

- on symbolise souvent l'état "haut" par le chiffre "1" et l'état "bas" par le chiffre "0"

- un ordinateur ne “connait” que 2 états (haut et bas ou 0 et 1), un ordinateur travaille donc en binaire

- Le transistor est l'élément de base des circuits logiques. Un circuit logique permet de réaliser une opération booléenne.

- Il existe deux catégories de circuit logique :

	- les circuits combinatoires (les états en sortie dépendent uniquement des états en entrée)

	- les circuits séquentiels (les états en sortie dépendent des états en entrée ainsi que du temps et des états antérieurs)

- les portes logiques sont des circuits combinatoires. Il existe 4 types de portes logiques : la porte NON, la porte OU, la porte ET et la porte OU EXCLUSIF

- à chaque type de porte logique on associe une table de vérité (vous devez connaître ces tables)

- en combinant les portes logiques, on obtient des circuits plus complexes (exemples : mémoire, additionneur…)

#### Les différents composants d’un ordinateur

- la mémoire vive ou RAM (Random Access Memory) : la mémoire vive permet de stocker des données et des programmes. La mémoire vive est une mémoire volatile :
toutes les données présentes en mémoire sont perdues en cas de coupure de courant. Pour stocker les données plus longtemps on utilisera la mémoire de masse
qui elle, n’est pas volatile (clé USB, disque dur, disque SSD…)

- Le microprocesseur ou CPU (Central Processing Unit) : Le microprocesseur est le "coeur" d'un ordinateur : les instructions sont exécutées au niveau du CPU. Il est
schématiquement constitué de 3 parties :

	- les registres permettent de mémoriser de l'information (donnée ou instruction) au sein même du CPU. Leur nombre et leur taille sont variables en fonction du type de microprocesseur.

	- L'unité arithmétique et logique (UAL ou ALU en anglais) est chargée de l'exécution de tous les calculs que peut réaliser le microprocesseur. Nous allons retrouver dans cette UAL des circuits comme l'additionneur

	- L'unité de commande permet d'exécuter les instructions (les programmes)

- Le bus : les données doivent circuler entre les différentes parties d’un ordinateur, notamment entre la mémoire vive et le CPU. Le système permettant cette circulation est appelé bus. Il existe, sans entrer dans les détails, 3 grands types de bus :

	- Le bus d’adresse permet de faire circuler des adresses (par exemple l’adresse d’une donnée à aller chercher en mémoire)

	- Le bus de données permet de faire circuler des données

	- Le bus de contrôle permet de spécifier le type d’action (exemples : écriture d’une donnée en mémoire, lecture d’une donnée en mémoire).

#### Architecture de von Neumann

John von Neumann (mathématicien et physicien américano-hongrois 1903-1957) a eu l'idée en 1945 d'utiliser une structure de stockage unique pour les données et les instructions , on parle d'architecture de von Neumann. Voici un schéma qui représente ce modèle de von
Neumann :

Sur ce schéma, nous avons :

![](img/c8c_13.gif)

- La mémoire qui correspond à la RAM vue ci-dessus

- L'unité arithmétique et logique qui correspond à l'UAL vu ci-dessus (l'accumulateur est un registre permettant de stocker les résultats intermédiaires lors d'un calcul)

- L'unité de commande qui gère l'exécution des instructions machines. À noter que cette unité de commande est aussi parfois appelée "unité de contrôle"

- Le système "entrée-sortie" qui permet de communiquer avec "le monde extérieur" au système CPU+RAM (clavier, souris, écran, carte graphique, disque dur...)

Les ordinateurs actuels continuent de se baser sur l'architecture de von Neumann. Pendant très longtemps les constructeurs ont cherché à augmenter la fréquence d’horloge des CPU afin d’améliorer les performances, aujourd’hui la tendance est plutôt à l’augmentation du
nombre de coeurs

### Ce qu’il faut savoir faire

Vous devez être capable d’écrire et de lire (et comprendre) des programmes simples en assembleur (en ayant en votre possession l’aide mémoire sur l’assembleur)