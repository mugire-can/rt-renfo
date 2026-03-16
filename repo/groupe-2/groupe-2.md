# Groupe 2

Voici les commandes à utiliser pour ce groupe :
Commandes du groupe 0 et 1, + `whoami`, `ps`, `wc`, `grep`, `tar`, `cut`, `sort`, `uniq`, `rev`, `sed`

Ce groupe utilise aussi un fichier de logs fictif appelé `logs.txt`. Ce fichier ne devra pas être ajouté à votre repo.


## Job 01

Commandes attendues :
- une commande qui crée un fichier `whoami.txt` contenant le résultat de la commande `whoami`
- une commande qui crée un fichier `ps.txt` contenant le résultat de la commande `ps`, sans la première ligne
- une commande qui affiche le nombre d'*octets* dans le fichier `ps.txt`

Les fichiers `.txt` ne devront pas être ajoutés à votre repo.


## Job 02

Commandes attendues :
- une commande qui affiche la ligne contenant "tail -f /dev/null" du fichier `ps.txt`
- une commande qui n'affiche que la ligne ne contenant pas "root" du fichier
- une commande qui n'affiche que la première colonne du fichier


## Job 03

Commandes attendues :
- une commande qui crée une archive `job03.tar` contenant les fichiers `logs.txt`, `whoami.txt` et `ps.txt`
- une commande qui crée une archive `job03-inception.tar` contenant l'archive précédente ET le fichier `who.txt`
- une commande qui extraie l'archive `job03-inception.tar` dans le répertoire courant


## Job 04

Commandes attendues :
- une commande qui trouve toutes les lignes contenant "POST" et "192.168.0.2"
- une commande qui n'affiche que les lignes sans code d'erreur ou de redirection
- une commande qui n'affiche que le code HTTP du logs
- une commande qui trie les logs par adresse IP
- une commande qui n'affiche que les adresses IP, sans doublons
- une commande qui remplace tous les codes 200 par "OK_YOLO"
- une commande qui compte combien de fois chaque IP a accédé au serveur
