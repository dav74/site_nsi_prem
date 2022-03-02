### Ce qu’il faut savoir

#### Norme ASCII

La norme ASCII (American Standard Code for Information Interchange) permet de représenter les caractères. Chaque caractère est associé à un nombre codé sur 8 bits (7 bits pour coder le caractère + 1 bit dit de parité). Avec 7 bits il est donc possible de coder
128 caractères.

#### Norme ISO-8859-1

La norme ASCII convient bien à la langue anglaise, mais pose des problèmes dans d'autres langues, par exemple le français. En effet l'ASCII ne prévoit pas d'encoder les lettres accentuées. C'est pour répondre à ce problème qu'est née la norme ISO-8859-1. Cette
norme reprend les mêmes principes que l'ASCII, mais les nombres binaires associés à chaque caractère sont codés sur 8 bits, ce qui permet d'encoder jusqu'à 256 caractères Cette norme va être principalement utilisée dans les pays européens puisqu'elle permet
d'encoder les caractères utilisés dans les principales langues européennes.

#### Unicode

Le but de la norme Unicode est de pouvoir encoder tous les caractères que l’on peut rencontrer dans le monde. Unicode est uniquement une table qui regroupe tous les
caractères existant au monde, il ne s'occupe pas de la façon dont les caractères sont codés dans la machine. Unicode accepte plusieurs systèmes de codage : UTF-8, UTF-16, UTF-32. Le plus utilisé, notamment sur le Web, est UTF-8. Pour encoder les caractères Unicode,
UTF-8 utilise un nombre variable d'octets : les caractères "classiques" (les plus couramment
utilisés) sont codés sur un octet, alors que des caractères "moins classiques" sont codés sur
un nombre d'octets plus important (jusqu'à 4 octets). Il y a compatibilité entre ASCII et UTF-8 puisque les caractères Unicode codés avec UTF-8 ont exactement le même code que les mêmes caractères en ASCII.

### Ce qu’il faut savoir faire

Convertir un fichier texte dans différents formats d’encodage.