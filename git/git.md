<div align="center">

**[Index](/README.md) | [GitFlow](/git/gitflow.md) | [GitHub CLI](/git/github-cli.md) | [LazyGit](/git/lazygit.md) | [Raccourcis Système](/shortcut-sys/shortcut.md) | [Raccourcis Terminal](/terminal/terminal.md) | [Markdown](/markdown/markdown.md)**

</div>

<br>

![banner](/git/git-pics/git.png)

<br>

# Configuration

**Vérifier la configuration Git :**

Renvoie une liste d'informations sur sa configuration Git, y compris le nom d'utilisateur et l'e-mail.


<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git config -l</code></pre>

**Configurer le nom d'utilisateur Git :**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git config --global user.name "Fabio"</code></pre>

**Configurer l'e-mail utilisateur Git :**

Permet de configurer l'adresse e-mail de l'utilisateur qui sera utilisée dans les commits.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git config --global user.email "signups@fabiopacifici.com"</code></pre>

**Mettre en cache ses identifiants de connexion dans Git :**

Stocke les identifiants de connexion dans le cache afin de ne pas avoir à les taper à chaque fois.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git config --global credential.helper cache</code></pre>

# Dépôt (repo)

**Initialiser un dépôt Git :**

Initialise un nouveau dépôt Git localement dans la racine de son projet.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git init</code></pre>

**Vérifier l'état d'un dépôt dans Git :**

Afiche l'état du dépôt actuel, y compris les fichiers en staged, unstaged et untracked.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git status</code></pre>

**Ajouter un dépôt distant dans Git :**

Ajoute un dépôt distant au dépôt local (remplacer simplement https://repo_ici par l'URL du dépôt distant).

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git add remote https://repo_ici</code></pre>

**Voir les URL distantes dans Git :**

Montre tous les dépôts distants de son dépôt local.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git remote -v</code></pre>

**Obtenir plus d'informations sur un dépôt distant dans Git :**

Remplacer simplement origin par le nom du dépôt distant obtenu en exécutant la commande git remote -v.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git remote show origin</code></pre>

**Pousser des changements vers un dépôt distant dans Git :**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git push</code></pre>

**Tirer des changements d'un dépôt distant dans Git :**

Récupére les derniers changements effectués sur le dépôt distant.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git pull</code></pre>

**Récupérer les changements du dépôt distant dans Git :**

Télécharge les changements d'un dépôt distant mais ne fusionnera pas la branche locale (car git pull le fait à la place).

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git fetch</code></pre>

**Récupére les dernières modifications depuis un dépôt distant dans votre dépôt local :**

L'option "--prune" est utilisée pour supprimer les références locales qui n'existent plus sur le dépôt distant.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git fetch --prune</code></pre>

**Fusionner un dépôt distant avec le dépôt local dans Git :**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git merge origin/main</code></pre>

# Zone de staging

**Ajouter un fichier à la zone de staging dans Git :**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git add filename_here</code></pre>

**Ajouter tous les fichiers dans la zone de staging dans Git :**

Ajoute tous les fichiers du projet à la zone de staging, en utilisant un joker . et tous les fichiers seront ajoutés.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git add .</code></pre>

**Ajouter uniquement certains fichiers à la zone de staging dans Git :**

Avec l'astérisque, ajoute tous les fichiers commençant par 'fil' dans la zone de staging.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git add fil*</code></pre>

# Modifications et messages (commit)

**Valider les modifications (commit) dans l'éditeur dans Git :**

Ouvre un éditeur de texte dans le terminal pour écrire un message de validation complet.
Un message de validation se compose d'un bref résumé des modifications, d'une ligne vide, et d'une description complète des modifications qui suivent.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git commit</code></pre>

**Valider les modifications avec un message dans Git :**

Ajoute un message de validation sans ouvrir l'éditeur. Permet de spécifier uniquement un bref résumé de son message.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git commit -m "message"</code></pre>

**Valider les modifications (et passer la zone de staging) dans Git :**

Ajoute et valide les fichiers suivis avec une seule commande en utilisant les options -a et -m.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git commit -a -m "message"</code></pre>

**Fusionner les changements de deux branches différentes tout en conservant une trace de l'historique des modifications**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">merge commit</code></pre>

**Voir l'historique des commits dans Git :**

Affiche l'historique des commits du dépôt actuel. Du plus récent au plus ancien.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git log</code></pre>

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git log -p</code></pre>

Affiche l'historique des commits, mais aussi les différences (diff) introduites par chaque commit. 

**Voir un commit spécifique dans Git :**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git show commit-id</code></pre>

**Voir les statistiques du journal dans Git :**

Fait en sorte que le journal Git affiche quelques statistiques sur les modifications apportées à chaque commit, y compris la/les ligne(s) modifiée(s) et les noms des fichiers.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git log --stat</code></pre>

**Voir les modifications apportées avant de les valider en utilisant "diff" dans Git :**

Passe un fichier en paramètre pour ne voir que les modifications sur un fichier spécifique.
git diff montre uniquement les modifications non indexées par défaut.
Appeler diff avec le drapeau --staged pour voir les modifications indexées.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git diff</code></pre>

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git diff all_checks.py</code></pre>

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git diff --staged</code></pre>

**Voir les modifications en utilisant "git add -p" :**

Ouvre une invite et demande si l'on veut mettre en stage les modifications ou non, et inclut d'autres options.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git add -p</code></pre>

**Supprimer les fichiers suivis de l'arborescence de travail actuelle dans Git :**

Attend un message de validation pour expliquer pourquoi le fichier a été supprimé.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git rm nom_du_fichier</code></pre>

**Renommer des fichiers dans Git :**

Met en stage les modifications, puis attend un commit.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git mv ancien_fichier nouveau_fichier</code></pre>

**Annuler les modifications non indexées dans Git :**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git checkout nom_du_fichier</code></pre>

**Annuler les modifications indexées dans Git :**

Utiliser le drapeau d'option -p pour spécifier les modifications à réinitialiser.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git reset HEAD nom_du_fichier</code></pre>

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git reset HEAD -p</code></pre>

**Modifier la validation la plus récente dans Git :**

Permet de modifier et d'ajouter des modifications à la validation la plus récente.
!!Note!!: corriger une validation locale avec amend est une excellente idée et vous pouvez la pousser vers un dépôt partagé après l'avoir corrigée. Mais vous devriez éviter de modifier les validations qui ont déjà été rendues publiques.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git commit --amend</code></pre>

**Annuler le dernier commit dans Git :**

git revert va créer un nouveau commit qui est l'opposé de tout ce qui se trouve dans le commit donné. Annuler le dernier commit en utilisant l'alias head comme ceci.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git revert HEAD</code></pre>

**Annuler un ancien commit dans Git :**

Annule un ancien commit en utilisant son identifiant de commit. Cela ouvre l'éditeur pour y ajouter un message de commit.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git revert identifiant_commit_ici</code></pre>

**Afficher le journal des commits sous forme de graphique dans Git :**

Utiliser --graph pour obtenir le journal des commits sous forme de graphique. De plus, --oneline limitera les messages de commit à une seule ligne.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git log --graph --oneline</code></pre>

**Afficher le journal des commits sous forme de graphique de toutes les branches dans Git :**

Fait la même chose que la commande ci-dessus, mais pour toutes les branches.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git log --graph --oneline --all</code></pre>

**Vérifier le journal des commits actuels d'un dépôt distant dans Git :**

Commit après commit, Git construit un journal. Trouve le journal du dépôt distant.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git log origin/main</code></pre>

# Branches (branch)

**Créer une nouvelle branche dans Git :**

Git ne basculera pas automatiquement dessus.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git branch nom_de_la_branche</code></pre>

**Basculer vers une nouvelle branche nouvellement créée dans Git :**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git checkout nom_de_la_branche</code></pre>

**Lister les branches dans Git :**

Montre toutes les branches créées. Liste de toutes les branches et marquera la branche actuelle avec un astérisque et la mettra en surbrillance en vert.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git branch</code></pre>

**Créer une branche dans Git et basculer immédiatement dessus :**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git checkout -b nom_de_la_branche</code></pre>

**Supprimer une branche dans Git :**

Après voir fini de travailler avec une branche et l'avoir fusionnée, supprime la branche.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git branch -d nom_de_la_branche</code></pre>

**Fusionner deux branches dans Git :**

Fusionne l'historique de la branche courante avec la branche souhaitée.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git merge nom_de_la_branche</code></pre>

**Annuler une fusion en conflit dans Git :**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git merge --abort</code></pre>

**Vérifier les branches distantes que Git suit :**

Montre le nom de toutes les branches distantes que Git suit pour le dépôt actuel.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git branch -r</code></pre>

**Obtenir le contenu des branches distantes dans Git sans fusion automatique :**

Permet de mettre à jour le dépôt distant sans fusionner aucun contenu dans les branches locales. Utiliser git merge ou git checkout pour effectuer la fusion.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git remote update</code></pre>

**Pousser une nouvelle branche vers un dépôt distant dans Git :**

Ne pas oublier d'ajouter -u pour créer la branche en amont.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git push -u origin nom_de_la_branche</code></pre>

**Supprimer une branche distante dans Git :**

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git push --delete origin nom_de_la_branche_ici</code></pre>

# Autres commandes

**Forcer une push request dans Git :**

C'est généralement acceptable pour les pull request de branches car personne d'autre ne devrait les avoir clonées. Mais ce n'est pas quelque chose à faire avec des dépôts publics.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git push -f</code></pre>

**Utiliser Git rebase :**

Transfére un travail terminé d'une branche à une autre.
Git Rebase peut devenir vraiment désordonné s'il n'est pas fait correctement. Avant d'utiliser, il est suggeré de relire la documentation officielle.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git rebase nom_de_la_branche_ici</code></pre>

**Exécuter un rebase de manière interactive dans Git :**

Exécute git rebase de manière interactive en utilisant le drapeau -i. Ouvre l'éditeur et présente un ensemble de commandes utilisables.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git rebase -i master</code></pre>

- `p, pick = utiliser le commit
- r, reword = utiliser le commit, mais modifier le message du commit
- e, edit = utiliser le commit, mais s'arrêter pour modifier
- s, squash = utiliser le commit, mais fusionner avec le commit précédent
- f, fixup = comme "squash", mais supprimer le message de journal de ce commit
- x, exec = exécuter une commande (le reste de la ligne) en utilisant le shell
- d, drop = supprimer le commit`

**Enregistrer temporairement les modifications non validées dans un répertoire de travail :**

Les modifications enregistrées sont placées dans une pile de stash.

<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git stash</code></pre>

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