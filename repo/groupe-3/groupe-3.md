# Groupe 3

Voici les commandes à utiliser pour ce groupe :
Commandes du groupe 0, 1 et 2, +
`awk`, `tr`, `column`, `>`, `>>`, `<`, `2>`, `2>&1`, et bien sûr les pipes (`|`).

Un fichier de travail `data.txt` est fourni. Il ne devra pas être ajouté au repo.


## Job 00

Commandes attendues :
- une commande qui écrit uniquement dans `stdout` le texte "Hello stdout"
- une commande qui écrit uniquement dans `stderr` le texte "Hello stderr"
- une commande qui redirige `stdout` dans un fichier `stdout.txt`
- une commande qui redirige `stderr` dans un fichier `stderr.txt`
- une commande qui redirige `stdout` et `stderr` dans le même fichier `both.txt`

Notes :
- les fichiers `.txt` ne doivent pas être commit.


## Job 01

Commandes attendues (tout concerne le fichier `data.txt`) :
- une commande qui affiche le nombre de lignes contenant INFO
- une commande qui affiche toutes les lignes contenant WARN, triées alphabétiquement
- une commande qui affiche les lignes uniques contenant DEBUG, sans doublon
- une commande qui affiche uniquement la 3e colonne, séparée par des espaces, des lignes contenant POST
- une commande qui transforme toutes les lettres minuscules en MAJUSCULES

## Job 02

Commandes attendues :
- une commande qui trouve tous les fichiers dont le nom contient ".md"
- une commande qui trouve tous les fichiers de `/app` modifiés il y a moins de 2h
- une commande qui trouve tous les fichiers `.txt` puis affiche leur taille triée par ordre croissant
- une commande qui supprime tous les fichiers trouvés dans le dossier `tmp/` dont le nom contient "old", en demandant une confirmation à chaque fois

Notes :
- Pour cette dernière commande, utilisez `find ... -exec ... \;` plutôt qu'un pipe


## Job 03

Commandes attendues :
- une commande qui remplace dans `data.txt` toutes les occurrences du mot "WARN" par "ATTENTION_ÇA_PIQUE!"
- une commande qui affiche la première et quatrième colonnes du fichier
- une commande qui affiche les données du fichier avec un séparateur ";" au lieu des espaces
- une commande qui supprime toutes les lignes vides
- une commande qui détecte la mauvaise date du fichier
