### Ce qu’il faut savoir

- la représentation en machine des nombres réels (on parle souvent en informatique
de nombres flottants) diffère de la représentation en machine des entiers

- la norme IEEE 754 est la norme la plus employée pour la représentation des
nombres à virgule flottante dans le domaine informatique.

- il existe 2 formats associés à la norme IEEE 754 : le format simple précision (le
nombre est représenté sur 32 bits) et le format double précision (le nombre est
représenté sur 64 bits)

- que cela soit en simple précision ou en double précision, la norme IEEE754 utilise :

	- 1 bit de signe (1 si le nombre est négatif et 0 si le nombre est positif)
	
	- des bits consacrés à l'exposant (8 bits pour la simple précision et 11 bits pour la double précision)
	
	- des bits consacrés à la mantisse (23 bits pour la simple précision et 52 bits pour la double précision)
	
- à cause de la limitation de la taille de mantisse on peut dans certains cas avoir des erreurs d’arrondies, par exemple 0.1 + 0.2 n’est pas égal à 0.3. On évitera de tester l’égalité entre 2 flottants (par exemple 0.1 + 0.2 == 0.3 retourne Faux !)

### Ce qu’il faut savoir faire

- vous devez être capable de trouver la représentation en binaire d’un réel (par exemple 0.1, 0.25 ou encore 1/3)

- vous n’avez pas à savoir écrire un nombre flottant en utilisant la norme IEEE754, vous devez juste connaitre les grands principes de cette norme (bit de signe,
mantisse, exposant)