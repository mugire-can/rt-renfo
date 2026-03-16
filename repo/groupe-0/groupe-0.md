# Groupe 0

Ce fichier contient les instructions de rendu pour le premier groupe de commandes, `groupe-0`.

Vous devrez mettre toutes vos commandes dans des fichiers `job00.txt`, `job01.txt`, etc., comme demandé plus bas. Chaque commande sera suivie d'un retour à la ligne. Suivez précisément cette typologie.


## Le fichier `.bashrc`

D'abord, configuer votre shell !

Commencez par améliorer le fichier de configuration de votre shell, `.bashrc`. Il se trouve dans le répertoire `/root`.

Ce fichier contient une commande `alias` et une commande `export`. Malheureusement, les commandes proposées sont bof. Commençons par l'améliorer :

1. D'abord, il vous faut définir un alias pour la commande `ls` qui :
- affiche tous les fichiers présents en format long, et
- affiche tous les fichiers, même cachés
- cet alias devrait n'avoir qu'une seule lettre

Aidez-vous de la commande `man ls` pour trouver cette configuration.

2. Ajoutez ensuite quelques alias de votre choix pour des commandes que vous utilisez souvent.

3. Ajoutez un chemin à votre variable d'environnement `PATH`.

4. Enfin, renseignez-vous sur la variable PS1 et modifiez-la pour configurer votre prompt. Vous devriez avoir au moins un élément en couleur, et afficher le répertoire courant.


À la fin, sourcez ce fichier avec cette commande pour voir les modifications dans votre shell :
`source /root/.bashrc`

Notes :
- Le fichier `.bashrc` est en dehors de votre repo et n'aura pas à être commit.
- Voyez s'il ne serait pas intéressant d'avoir un alias pour sourcer ce fichier...


## Commandes du groupe 0

Voici les commandes à utiliser pour ce groupe :
`pwd`, `echo`, `cd`, `ls`, `cp`, `mv`, `rm`, `mkdir`, `rmdir`, `history`, `cat`, `touch`, `stat`, `man`.

La commande `man xxx` (xxx = le nom de la commande) vous aidera grandement à fouiller dans les options de chacune.


## Job 00

Dans un fichier `job00.txt`, saisissez les commandes suivantes :
- une commande qui affiche le répertoire courant
- une commande qui vous déplace au répertoire parent
- une commande qui revient au répertoire où vous étiez juste avant, sans taper son nom


## Job 01

Une seule commande attendue :
- elle liste les fichiers présents dans le répertoire courant, en format long
- et affiche les fichiers cachés...
- ...mais n'affiche pas `.` ni `..`
- les répertoires devraient être suivis d'un caractère `/`
- affiche les tailles de fichier en format "human-readable", avec des préfixes de taille (kilo, méga...)


## Job 02

- une commande qui copie le fichier `groupe-0.md` en `copy.md`
- une commande qui renomme le fichier `copy.md` en `copy2.md`
- une commande qui affiche le contenu de tous les fichiers Markdown du répertoire


## Job 03

Commandes attendues :
- une commande pour afficher à l'écran le texte "Hello, World!" avec retour à la ligne à la fin
- une commande pour afficher votre historique de commandes shell
- une commande qui crée un nouveau fichier `yolo.md`
- une commande qui affiche les statistiques de ce nouveau fichier
- une commande qui supprime ce fichier


## Job 04

Commandes attendues :
- une commande pour créer un nouveau répertoire `tmp`
- une commande pour renommer ce répertoire en `tmp2`
- une commande pour créer un nouveau répertoire `tmp3` dans `tmp2`
- une commande pour supprimer ce répertoire `tmp3`
