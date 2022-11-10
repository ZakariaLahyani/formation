# Git kata: modification des commits
Lorsque nous travaillons, nous faisons beaucoup de commits.
Parfois, nous oublions simplement quelque chose d'évident que nous voulons corriger rapidement.

`git commit --amend` nous permet de faire cela - bricoler avec le dernier commit que nous avons fait.

Vous pouvez utiliser `git log -p` ou `git show` pour inspecter le contenu des commits et les modifications de fichiers qui ont été ajoutées aux commits.

## Installer:

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Que nous dit `git status`?
2. Que nous dit `git log -p`?
3. Étape l'ajout de bar.txt
4. Exécutez `git commit --amend`
5. Que s'est-il passé ? Que nous dit `git log -p`?
6. Que se passe-t-il si vous relancez `git commit --amend`?

## Useful commands

- `git add`
- `git log --oneline --graph`
- `git log -p`
- `git show`
- `git commit --amend`
