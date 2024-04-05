<div align="center">

**[Index](/README.md) | [Git](/git/git.md) | [GitFlow](/git/gitflow.md) | [GitHub CLI](/git/github-cli.md) | [LazyGit](/git/lazygit.md) | [Node.js](/node-js/node-js.md) | [Raccourcis Système](/shortcut-sys/shortcut.md) | [Raccourcis Terminal](/terminal/terminal.md) | [Markdown](/markdown/markdown.md)**

</div>

<br>

![banner](/git/git-pics/git-conventions-readme.png)

<br>

`feat :` Ajout d’une nouvelle fonctionnalité.

  `fix :` Correction d’un bug.

  `chore :` Tâches de maintenance, mises à jour, etc.

  `docs :` Modifications de la documentation.

  `style :` Changements de style (indentation, espaces, etc.).

  `refactor :` Modifications sans ajout de fonctionnalité ni amélioration des performances.

  `perf :` Améliorations des performances.

  `test :` Ajout ou modification de tests.

  `build :` Changements affectant le système de build ou les dépendances externes.

  `ci :` Modifications concernant les scripts d’intégration ou de configuration.

  `revert:` Annulation d’un commit précédent.

**Portée (scope)** (facultatif) :

- Indique la partie du projet affectée par le commit (par exemple, api, lang, etc.).

**Sujet :**

- Brève description du changement effectué.

**Corps (body)** (facultatif) :

- Explication plus détaillée du changement (si nécessaire).

**Pied de page (footer)** (facultatif) :

- Utilisé pour indiquer les changements de rupture (BREAKING CHANGE) ou d’autres informations pertinentes.

**Voici quelques exemples de messages de commit conformes à cette convention :**

- Ajout d’une nouvelle fonctionnalité :

  `feat(api):` Ajout de l'authentification par token

- Correction d’un bug :

  `fix(lang):` Correction de la traduction du bouton

- Modification de la documentation :

  `docs:` Mise à jour du guide d'utilisation

- Amélioration des performances :

  `perf(api):` Optimisation de la requête de recherche

N’hésitez pas à adopter cette convention pour rendre vos messages de commit plus clairs et cohérents ! 😊

**Quelques ressources complémentaires :**

- https://conventionalcommits.org
- https://buzut.net/cours/versioning-avec-git/bien-nommer-ses-commits
- https://les-enovateurs.com/conventional-commits-details-exemples-pratiques

<a href="/git/conventional-commits.md"><img src="/git/git-pics/index.png" alt="Markdown" style="width: 100px; height: auto; margin-right: 10px;"></a><a href="/README.md"><img src="/readme-pics/back-readme.png" alt="Markdown" style="width: 100px; height: auto; margin-right: 10px;"></a>