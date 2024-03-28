# Commandes Git

`git init` : Initialise un nouveau dépôt Git dans un répertoire existant

`git clone` [url] : Clone un dépôt distant dans un nouveau répertoire local.

`git add` [fichier] : Ajoute un fichier à l'index (staging area) pour le suivi.

`git commit -m` "[message]" : Enregistre les modifications de l'index dans l'historique du dépôt, avec un message descriptif.

`git status` : Affiche l'état des fichiers dans le répertoire de travail et de l'index.

`git log` : Affiche l'historique des commits.

`git branch` [nom_de_branche] : Crée une nouvelle branche.

`git checkout` [nom_de_branche] : Permet de basculer entre les branches.

`get switch` [nom_de_branche] : Permet de basculer sur la branche souhaitée

`git merge` [nom_de_branche] : Fusionne une branche spécifiée dans la branche actuelle.

`git push` [remote] [branche] : Envoie les commits locaux vers un dépôt distant.

`git pull` [remote] [branche] : Récupère les commits d'un dépôt distant et les fusionne dans la branche locale.

`git remote add` [remote] [url] : Ajoute un nouveau dépôt distant.

`git remote -v` : Affiche les dépôts distants configurés.

`git diff` : Affiche les différences entre les fichiers dans l'index et la version actuelle.

`git rm` [fichier] : Supprime un fichier du répertoire de travail et de l'index.

`git rf` [répertoire] : Supprime un répertoire de travail et de l'index

`git commit --amend -m` "Nouveau message de commit" : Renomme le dernier commit