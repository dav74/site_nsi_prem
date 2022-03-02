Vous allez réaliser une version "site web" du projet répertoire téléphonique.

Voici une vidéo qui va vous permettre de comprendre ce qui est attendu :

[https://www.youtube.com/watch?v=xTETvikDMBw](https://www.youtube.com/watch?v=xTETvikDMBw)

Pour réaliser ce projet, vous allez utiliser le framework Python flask. Nous allons commencer par voir 2 choses :

- Comment utiliser une feuille de style css avec flask

- Comment gérer les liens (balise \<a>) avec flask

Pour créer une feuille de style, vous devez commencer par créer un répertoire "static" (au même niveau de l'arborescence que le répertoire "templates") et placer votre fichier "style.css" dans ce répertoire "static"

Pour les liens entre les pages, il faut utiliser les balises <a>, mais l'URL est un peu particulière

Pour illustrer tout cela, voici un exemple très simple qui utilise les liens et une feuille de style :

views.py

```
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def index():
    return render_template("index.html")
@app.route('/autre_page')
def autre_page():
    return render_template("autre_page.html")
app.run(debug=True)
```

index.html (répertoire "templates")

```
<!doctype html>
<html lang="fr">

<head>
    <meta charset="utf-8">
    <title>Ma page</title>
    <link rel="stylesheet" href="{{url_for('static', filename='style.css')}}">
</head>

<body>
    <h1>Mon super site</h1>
    <p>Tout fonctionne parfaitement, voici <a href="{{ url_for('autre_page') }}">un lien</a> vers une autre page</p>
</body>

</html>
```

autre_page.html (répertoire "templates")

```
<!doctype html>
<html lang="fr">

<head>
    <meta charset="utf-8">
    <title>Ma page</title>
    <link rel="stylesheet" href="{{url_for('static', filename='style.css')}}">
</head>

<body>
    <h1>About</h1>
    <p><a href="{{ url_for('index') }}">Retour vers la première page</a></p>
</body>

</html>
```

style.css (répertoire "static")

```
h1{
	text-align: center;
}
```

En étudiant attentivement l'exemple ci-dessus, vous devriez être capable d'utiliser les feuilles de style et les liens.

Le coeur de votre projet devrait pas mal ressembler au projet 1 "répertoire téléphonique", il vous faudra notamment sauvegarder les données dans un fichier texte. À ce propos, nous verrons l'année prochaine un autre système bien plus efficace qu'un simple fichier texte pour sauvegarder des données : les bases de données.