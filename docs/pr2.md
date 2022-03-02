Le deuxième projet va vous permettre de mettre au point un générateur de questions à choix multiples.

Voici une vidéo qui va vous permettre de comprendre ce qui est attendu :

[https://www.youtube.com/watch?v=_-2nQRZGa-c](https://www.youtube.com/watch?v=_-2nQRZGa-c)

Vous avez à votre disposition un fichier texte qcm.txt qu'il est possible de télécharger [ici](asset/qcm.txt). Ce fichier contient 30 questions et réponses, voici un exemple de question (et de la réponse qui va avec) :

```
Un octet correspond à A-1bit B-4 bits C-8 bits D-32 bits;;C
```

Comme vous pouvez le constater, la question et la réponse correcte sont séparées par 2 points-virgules.

N.B. : il est tout à fait possible de rédiger vos propres questions et de les placer dans un fichier au format texte.

Votre programme devra "piocher" au hasard 10 questions parmi les 30 questions présentes dans le fichier qcm.txt (à chaque exécution de votre programme, les 10 questions ne seront pas identiques)

On ne pourra pas avoir 2 fois la même question au cours d'une même session.

À la fin des 10 questions, le score devra être affiché

Au cours de ce projet, il vous sera sans doute nécessaire d'étudier les 2 points suivants :

- le module random qui permet de gérer le "hasard" en Python (pour en savoir plus, voir [ici](https://www.w3schools.com/python/module_random.asp)

- la méthode split qui permet de séparer en plusieurs morceaux une chaîne de caractères (pour en savoir plus, voir [ici](https://www.w3schools.com/python/ref_string_split.asp))

N'oubliez pas d'utiliser le plus possible les fonctions.