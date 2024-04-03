<div align="center">

**[Index](/README.md) | [Git](/git/git.md) | [GitFlow](/git/gitflow.md) | [LazyGit](/git/lazygit.md) | [Raccourcis Système](/shortcut-sys/shortcut.md) | [Raccourcis Terminal](/terminal/terminal.md) | [Markdown](/markdown/markdown.md)**

# GitHub CLI

</div>

**Authentification et configuration :**

`gh auth login` : Authentifiez-vous sur GitHub.
`gh auth logout` : Déconnectez-vous de GitHub.
`gh config set` : Configurez des options pour gh, comme l'éditeur par défaut.

**Travail avec des référentiels (repositories) :**

`gh repo create` : Créez un nouveau référentiel à distance.
`gh repo clone` : Clonez un référentiel à partir de GitHub.
`gh repo view` : Affichez les détails d'un référentiel.

**Travail avec des pull requests (demandes de tirage) :**

`gh pr list` : Liste toutes les demandes de tirage.
`gh pr create` : Créez une nouvelle demande de tirage.
`gh pr checkout` : Vérifiez une demande de tirage localement.

**Travail avec des problèmes (issues) :**

`gh issue list` : Liste toutes les issues dans un référentiel.
`gh issue create` : Créez un nouveau problème.
`gh issue view` : Affichez les détails d'un problème.

**Autres commandes utiles :**

`gh gist create` : Créez un nouveau Gist.
`gh workflow list` : Liste les workflows d'un référentiel.
`gh release create` : Créez une nouvelle version d'un référentiel.

Vous pouvez obtenir plus d'informations sur chaque commande en utilisant gh help [commande]. Par exemple, gh help pr list vous donnera des informations sur la commande gh pr list.