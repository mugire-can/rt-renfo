# Groupe 1

## Commandes du groupe 1

Voici les commandes à utiliser pour ce groupe :
Commandes du groupe 0, + `chmod`, `chown`, `head`, `tail`, `ln`, `which`

## Job 00

Commandes attendues :
- une commande pour créer un nouveau fichier `yolo.md` avec le contenu "Hello, World", avec retour à la ligne final
- une commande pour ajouter à ce fichier la ligne "Hello, la Plateforme", sans retour à la ligne
- une commande qui copie ce fichier en `yolo2.md`
- une commande qui affiche le contenu de ces deux fichiers, en commençant par le deuxième


## Job 01

Commandes attendues :
- une commande pour afficher les deux premières lignes de `groupe-1.md`
- une commande pour afficher les dix dernières lignes de `groupe-1.md`
- une commande pour afficher l'emplacement de la commande `ls` sur votre système


## Job 02

Saisissez (dans l'ordre que vous voulez) toutes les commandes pour obtenir précisément les lignes suivantes :

```
$> ls -l
total YYY
-rw-r--r--    1 root  root     YYYY YYY   Y YY:YY groupe-1.md
--w-r-xrw-    1 root  root       14 Fev   3 05:28 yolo3.md
```

Remarques :
- Les caractères "YY" n'ont pas d'importance
- La taille, la date et l'heure sont à reproduire précisément .
- Où est la taille du contenu du fichier ? Pourquoi semble-t-elle "dépasser de 1" son contenu ?
- Que sont `root` et `root` ?


## Job 03

Saisissez toutes les commandes pour obtenir précisément l'affichage suivant :

```
$> ls -l
total YYY
-rw-r--r--    1 root     root YYYY YYY  Y YY:YY groupe-1.md
dr-x------    2 root     root   YY Jan  1 20:47 test0
-rwx--xr--    1 root     root    4 Jan  1 21:46 test1
lrwxrwxrwx    1 root     root    5 Jan  1 22:20 test2 -> test0
```

Remarques :
- Les caractères "YY" n'ont pas d'importance
