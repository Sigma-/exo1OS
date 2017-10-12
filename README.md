# Travail pratique OS (1)
## Exercice 3
1. On se place tout d'abord dans le répertoire de connexion grâce à la commande "cd". Puis, pour créer le répertoire "exo", nous utiliserons la commande : "mkdir exo". 
* "pwd" affiche le chemin absolu du répertoire "exo" : /home/users/100/twautele/exo
2. La commande "touch es1" permet de créer un fichier vide. Pour créer le répertoire : "essai2", il suffit d'utiliser la commande "mkdir essai2" tout en étant placer dans le répertoire "exo".
3. Nous utiliserons la commande "cp es1 essai2" pour copier "es1" dans "essai2". Ensuite, nous nous placerons dans le dossier "essai2" grâce à la commande : "cd essai2". Pour finir, la commande : "mv es1 es1-copie" permettra de renommer "es1" en "es1-copie".
* Nous pouvons réduire cela à une seule et unique commande qui est la suivante : "cp es1 essai2/es1-copie".
4. La commande "ls \*" dans le répertoire de connexion affiche les répertoires, fichiers, sous-répertoires et sous-fichiers mais pas plus loin.
* "ls|grep "^es" permet d'afficher les fichiers commençant par "es"
5. Pour supprimer un fichier avec une demande de confirmation, nous utiliserons la commande: "rm -i nom_du_fichier".
* Pour supprimer un répertoire et ses sous-répertoires : "rm -dr nom_du_repertoire"
6. Pour lire la 51e ligne d'un fichier texte de 100 lignes, il faut exécuter la commande suivante : "head -n 51 nom_du_fichier | tail -n 1 nom_du_fichier"
* On peut également utiliser une autre commande : 'sed -n "51 p" ~/fichier.txt'
7. Lorsqu'on utilise "grep passwd /etc/\*", on se rend compte que de nombreuses erreurs s'affichent sur le terminal : "permission denied" pour de nombreux fichiers/répertoires.
* Pour résoudre cette erreur, nous utiliserons la commande : "sudo chmod 777 /etc/". "sudo" sera utilisé pour exécuter la commande en tant qu'administrateur.
8. Pour trouver tous les fichiers commençant par "A" ou "a", on peut utiliser la commande : 'find -name "A\*" ! -name "a\*"'.
9. Pour trouver les fichiers plus récemment modifié qu'un autre fichier spécifié, on utilise la commande : "find -anewer nom_du_fichier_specifique".
10. Pour trouver un fichier finissant par l'extension ".o" et le supprimer, il faut utiliser la commande : "find -name "\*.c" -exec rm -f {} \;"

Bonne journée
