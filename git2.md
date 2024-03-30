<div align="center"><img src="https://image.noelshack.com/fichiers/2024/13/6/1711822520-cheat-sheet-git.png" style="width: 1000px;"/></div>
<br>
<br>

# Configuration

**Vérifier la configuration Git :**

Renvoie une liste d'informations sur sa configuration Git, y compris le nom d'utilisateur et l'e-mail.

<code>git config -l</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Configurer le nom d'utilisateur Git :**

<code>git config --global user.name "Fabio"</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Configurer l'e-mail utilisateur Git :**

Permet de configurer l'adresse e-mail de l'utilisateur qui sera utilisée dans les commits.

<code>git config --global user.email "signups@fabiopacifici.com"</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Mettre en cache ses identifiants de connexion dans Git :**

Stocke les identifiants de connexion dans le cache afin de ne pas avoir à les taper à chaque fois.

<code>git config --global credential.helper cache</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

# Dépôt (repo)

**Initialiser un dépôt Git :**

Initialise un nouveau dépôt Git localement dans la racine de son projet.

<code>git init</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Vérifier l'état d'un dépôt dans Git :**

Afiche l'état du dépôt actuel, y compris les fichiers en staged, unstaged et untracked.

<code>git status</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>
**Ajouter un dépôt distant dans Git :**

Ajoute un dépôt distant au dépôt local (remplacer simplement https://repo_ici par l'URL du dépôt distant).

<code>git add remote https://repo_ici</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Voir les URL distantes dans Git :**

Montre tous les dépôts distants de son dépôt local.

<code>git remote -v</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Obtenir plus d'informations sur un dépôt distant dans Git :**

Remplacer simplement origin par le nom du dépôt distant obtenu en exécutant la commande git remote -v.

<code>git remote show origin</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Pousser des changements vers un dépôt distant dans Git :**

<code>git push</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Tirer des changements d'un dépôt distant dans Git :**

Récupére les derniers changements effectués sur le dépôt distant.

<code>git pull</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Récupérer les changements du dépôt distant dans Git :**

Télécharge les changements d'un dépôt distant mais ne fusionnera pas la branche locale (car git pull le fait à la place).

<code>git fetch</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Fusionner un dépôt distant avec le dépôt local dans Git :**

<code>git merge origin/main</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

# Zone de staging

**Ajouter un fichier à la zone de staging dans Git :**

<code>git add filename_here</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Ajouter tous les fichiers dans la zone de staging dans Git :**

Ajoute tous les fichiers du projet à la zone de staging, en utilisant un joker . et tous les fichiers seront ajoutés.

<code>git add .</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Ajouter uniquement certains fichiers à la zone de staging dans Git :**

Avec l'astérisque, ajoute tous les fichiers commençant par 'fil' dans la zone de staging.

<code>git add fil*</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

# Modifications et messages (commit)

**Valider les modifications (commit) dans l'éditeur dans Git :**

Ouvre un éditeur de texte dans le terminal pour écrire un message de validation complet.
Un message de validation se compose d'un bref résumé des modifications, d'une ligne vide, et d'une description complète des modifications qui suivent.

<code>git commit</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Valider les modifications avec un message dans Git :**

Ajoute un message de validation sans ouvrir l'éditeur. Permet de spécifier uniquement un bref résumé de son message.

<code>git commit -m "message"</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Valider les modifications (et passer la zone de staging) dans Git :**

Ajoute et valide les fichiers suivis avec une seule commande en utilisant les options -a et -m.

<code>git commit -a -m "message"</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Voir l'historique des commits dans Git :**

Affiche l'historique des commits du dépôt actuel. Du plus récent au plus ancien.

<code>git log</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

<code>git log -p</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

Affiche l'historique des commits, mais aussi les différences (diff) introduites par chaque commit. 

**Voir un commit spécifique dans Git :**

<code>git show commit-id</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Voir les statistiques du journal dans Git :**

Fait en sorte que le journal Git affiche quelques statistiques sur les modifications apportées à chaque commit, y compris la/les ligne(s) modifiée(s) et les noms des fichiers.

<code>git log --stat</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Voir les modifications apportées avant de les valider en utilisant "diff" dans Git :**

Passe un fichier en paramètre pour ne voir que les modifications sur un fichier spécifique.
git diff montre uniquement les modifications non indexées par défaut.
Appeler diff avec le drapeau --staged pour voir les modifications indexées.

- <code>git diff</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>
- <code>git diff all_checks.py</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>
- <code>git diff --staged</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Voir les modifications en utilisant "git add -p" :**

Ouvre une invite et demande si l'on veut mettre en stage les modifications ou non, et inclut d'autres options.

<code>git add -p</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Supprimer les fichiers suivis de l'arborescence de travail actuelle dans Git :**

Attend un message de validation pour expliquer pourquoi le fichier a été supprimé.

<code>git rm nom_du_fichier</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Renommer des fichiers dans Git :**

Met en stage les modifications, puis attend un commit.

<code>git mv ancien_fichier nouveau_fichier</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Annuler les modifications non indexées dans Git :**

<code>git checkout nom_du_fichier</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Annuler les modifications indexées dans Git :**

Utiliser le drapeau d'option -p pour spécifier les modifications à réinitialiser.

- <code>git reset HEAD nom_du_fichier</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>
- <code>git reset HEAD -p</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Modifier la validation la plus récente dans Git :**

Permet de modifier et d'ajouter des modifications à la validation la plus récente.
!!Note!!: corriger une validation locale avec amend est une excellente idée et vous pouvez la pousser vers un dépôt partagé après l'avoir corrigée. Mais vous devriez éviter de modifier les validations qui ont déjà été rendues publiques.

<code>git commit --amend</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Annuler le dernier commit dans Git :**

git revert va créer un nouveau commit qui est l'opposé de tout ce qui se trouve dans le commit donné. Annuler le dernier commit en utilisant l'alias head comme ceci.

<code>git revert HEAD</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Annuler un ancien commit dans Git :**

Annule un ancien commit en utilisant son identifiant de commit. Cela ouvre l'éditeur pour y ajouter un message de commit.

<code>git revert identifiant_commit_ici</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Afficher le journal des commits sous forme de graphique dans Git :**

Utiliser --graph pour obtenir le journal des commits sous forme de graphique. De plus, --oneline limitera les messages de commit à une seule ligne.

<code>git log --graph --oneline</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Afficher le journal des commits sous forme de graphique de toutes les branches dans Git :**

Fait la même chose que la commande ci-dessus, mais pour toutes les branches.

<code>git log --graph --oneline --all</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Vérifier le journal des commits actuels d'un dépôt distant dans Git :**

Commit après commit, Git construit un journal. Trouve le journal du dépôt distant.

<code>git log origin/main</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

# Branches (branch)

**Créer une nouvelle branche dans Git :**

Git ne basculera pas automatiquement dessus.

<code>git branch nom_de_la_branche</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Basculer vers une nouvelle branche nouvellement créée dans Git :**

<code>git checkout nom_de_la_branche</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Lister les branches dans Git :**

Montre toutes les branches créées. Liste de toutes les branches et marquera la branche actuelle avec un astérisque et la mettra en surbrillance en vert.

<code>git branch</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Créer une branche dans Git et basculer immédiatement dessus :**

<code>git checkout -b nom_de_la_branche</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Supprimer une branche dans Git :**

Après voir fini de travailler avec une branche et l'avoir fusionnée, supprime la branche.

<code>git branch -d nom_de_la_branche</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Fusionner deux branches dans Git :**

Fusionne l'historique de la branche courante avec la branche souhaitée.

<code>git merge nom_de_la_branche</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Annuler une fusion en conflit dans Git :**

<code>git merge --abort</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Vérifier les branches distantes que Git suit :**

Montre le nom de toutes les branches distantes que Git suit pour le dépôt actuel.

<code>git branch -r</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Obtenir le contenu des branches distantes dans Git sans fusion automatique :**

Permet de mettre à jour le dépôt distant sans fusionner aucun contenu dans les branches locales. Utiliser git merge ou git checkout pour effectuer la fusion.

<code>git remote update</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Pousser une nouvelle branche vers un dépôt distant dans Git :**

Ne pas oublier d'ajouter -u pour créer la branche en amont.

<code>git push -u origin nom_de_la_branche</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Supprimer une branche distante dans Git :**

<code>git push --delete origin nom_de_la_branche_ici</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

# Autres commandes

**Forcer une push request dans Git :**

C'est généralement acceptable pour les pull request de branches car personne d'autre ne devrait les avoir clonées. Mais ce n'est pas quelque chose à faire avec des dépôts publics.

<code>git push -f</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Utiliser Git rebase :**

Transfére un travail terminé d'une branche à une autre.
Git Rebase peut devenir vraiment désordonné s'il n'est pas fait correctement. Avant d'utiliser, il est suggeré de relire la documentation officielle.

<code>git rebase nom_de_la_branche_ici</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>

**Exécuter un rebase de manière interactive dans Git :**

Exécute git rebase de manière interactive en utilisant le drapeau -i. Ouvre l'éditeur et présente un ensemble de commandes utilisables.

<code>git rebase -i master</code> <button onclick="navigator.clipboard.writeText(document.querySelector('code').textContent).then(()=>alert('Copié !')).catch(err=>console.error(err));">Copier</button>
- `p, pick = utiliser le commit
- r, reword = utiliser le commit, mais modifier le message du commit
- e, edit = utiliser le commit, mais s'arrêter pour modifier
- s, squash = utiliser le commit, mais fusionner avec le commit précédent
- f, fixup = comme "squash", mais supprimer le message de journal de ce commit
- x, exec = exécuter une commande (le reste de la ligne) en utilisant le shell
- d, drop = supprimer le commit`