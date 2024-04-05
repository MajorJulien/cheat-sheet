<div align="center">

**[Index](/README.md) | [Git](/git/git.md) | [GitHub CLI](/git/github-cli.md) | [LazyGit](/git/lazygit.md) | [Conventions](/git/conventional-commits.md) | [Node.js](/node-js/node-js.md) | [Raccourcis Système](/shortcut-sys/shortcut.md) | [Raccourcis Terminal](/terminal/terminal.md) | [Markdown](/markdown/markdown.md)**

![banner](/git/git-pics/gitflow.png)

</div>

**Configuration et Initialisation**

Initialise un dossier .git vide, dans le dépôt courant et déplace l'utilisateur sur la branche develop :
<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git flow init</code></pre>

**Branches**

Crée une branche de feature et en fait la branche courante :
<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git flow feature start [branche]</code></pre>

Fusionne la branche de feature sur la branche develop, et supprime la branche feature :
<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git flow feature finish [branche]</code></pre>

Crée une branche de déboggage et en fait la branche courante :
<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git flow hotfgit flow hotfix start [branche]</code></pre>

Fusionne la branche hotfix à la branche main et develop, et supprime la branche hotfix :
<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git flow hotfix finish [branche]</code></pre>

Crée une nouvelle branche de release à partir de la branche develop :
<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git flow release start [numero de version]</code></pre>

Fusionne la branche release sur la branche main et supprime la branche release :
<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git flow release finish [numero de version]</code></pre>

**Partage de branches**

Pousse la branche feature sur le dépôt distant :
<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git flow feature publish [branche]</code></pre>

Récupère une branche d'un dépôt distant :
<button class="btn" data-clipboard-target="#git-command"></button>
<pre><code id="git-command">git flow feature pull [remote] [branche]</code></pre>
</div>

[![Retour en haut de page](/git/git-pics/back-top.png)](#) <a href="/README.md"><img src="/git/git-pics/back-readme.png" alt="Markdown" style="width: 100px; height: auto; margin-right: 10px;"></a>