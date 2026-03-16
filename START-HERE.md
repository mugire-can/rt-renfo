# START HERE

## Votre setup de git && GitHub

### 1. install

Au commencement, il y avait git. Commencez donc par installer git avec le package manager d'Alpine Linux, `apk`:

`apk add git openssh-client`


### 2. init

Une fois git installé, vous pouvez instancier un repo à la racine de votre projet, `/app/repo`. Si vous ne savez pas où vous êtes, la commande `pwd` pourrait vous aider...

Une fois dans le bon répertoire, initialisez le repo :
`git init -b main`


### 3. who are you?

Déclarez ensuite votre identité locale git avec les commandes suivantes :
`git config --global user.email "your@email.com"`
`git config --global user.name "Your Name"`

Ces changements seront enregistrés automatiquement dans `/root/.gitconfig`.


### 4. synchro GitHub

Créez ensuite un repo sur GitHub avec le nom "btp-cardio". Une fois ce repo créé, faites dans votre repo local :
`git remote set-url origin https://github.com/fdeage/btp-cardio.git`

Si vous faites `cat .git/config` à la racine de votre projet, vous verrez votre remote GitHub apparaître. Il s'appelle `origin`.

Allez ensuite créer un token de connexion depuis https://github.com/settings/tokens : "Générer un nouveau token (classique)". Vous obtiendrez une chaîne de type `ghp_jXS3t...`. Conservez ce token généré, il vous servira de mot de passe pour chaque `git push` !


### 5. Don't ignore `.gitignore`

Une fois votre repo instancié et synchronisé avec GitHub, créez un fichier `.gitignore` pour éviter de commit les fichiers Markdown (fichiers `... .md`). Ce `.gitignore` doit figurer dans votre premier commit. Ce commit doit s'appeler "Add .gitignore".

Vérifiez enfin avec `tig` que c'est bien le cas (`tig` n'est pas installé, vous devrez l'installer avec `apk ...`).


### 6. "Push me, and then just touch me..."

Et maintenant un petit push pour tester tout ça !
- si c'est votre premier push depuis la branche : `git push -u origin groupe-0`
- sinon `git push` suffit.

GitHub devrait vous demander :
```
Username for 'https://github.com': <votrelogin>
Password for 'https://<votrelogin>@github.com':
```
Saisissez le PAT (`ghp...`) obtenu plus haut.
Vous devriez voir un truc du genre :
```
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 569 bytes | 284.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
```
Ça veut dire que tout roule : vous avez bien push sur votre repo GitHub. Allez-y depuis un navigateur Web pour confirmer.


## On code !

Vous pouvez maintenant commencer à coder.
Pour l'édition de texte en ligne de commandes, nous recommandons l'éditeur `helix` (que vous pouvez aussi installer via `apk`). Mais n'importe quel éditeur fera l'affaire (`nano`, `vim`, `emacs`, `ed`...)

Pour accéder au man, commencez par installer aussi les packages suivant avec `apk` : `man-db` et `coreutils-doc`

Vous pouvez prendre les groupes d'exercice dans l'ordre que vous voulez. Cependant, comme ils sont de difficulté croissante, nous recommandons de les traiter dans l'ordre.

Rappelez-vous que vous ne devez commit que sur une branche liée au groupe. Et vous ne devez jamais commit sur la branche `main` ! Commencez donc par créer une branche (on rappelle que la branche doit porter le nom du dossier dans lequel vous allez coder).

Une fois ceci fait, chaque dossier `groupe-n` contient un fichier avec les instructions. Il vous donnera précisément les fichiers à commit dans chaque groupe.


_Happy Hacking!_
