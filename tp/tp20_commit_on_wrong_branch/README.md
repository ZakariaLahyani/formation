# gitkatas

## Setup

1. Run `source setup.sh` (or `.\setup.ps1` in PowerShell)

## Kata 5: Commit on wrong branch

Vous travaillez très dur sur la branche master.
Une partie de votre travail est déjà engagée. C'est à ce moment que votre patron arrive avec une demande urgente.

Étant donné que votre HEAD actuel n'est pas prêt pour le prime time, vous sauvegardez un commit et démarrez une nouvelle branche nommée 'quickfix'. Vous faites ce que votre patron veut et validez les modifications apportées à cette nouvelle branche.

C'est alors que vous vous rendez compte que vous avez créé un désordre mineur avec vos branches.

Actuellement, vos commits ressemblent à ceci

```text
         master
           |
           v
   A <---- B
   ^ \
   |  \--- C
remote     ^
           |
        quickfix
```

Mais vous voulez qu'il ressemble à ceci:

```text
         remote
           |
           v
   A <---- C <---- B
                   ^
                   |
                  HEAD
```

Git ahead!

Remarque: étant donné que le `B` dans la structure actuelle et dans la structure cible n'a pas le même parent, il ne peut pas s'agir littéralement du même commit.
## The task

1. Utilisez `git log --oneline --graph --all` pour afficher toutes les branches et leurs commits.
2. Copiez `C` sur `master` avant `B` en rebasant `quickfix` sur `master`.
3. Créez une nouvelle branche (`changes-incluant-B`) à partir de notre `master` afin que nous puissions continuer à travailler sur `B`.
4. Réinitialisez 'maître' à 'C'.
5. Supprimez la branche `quickfix`.
6. Appuyez sur "maître". Vous ne pouvez pas faire cela dans l'exercice d'entraînement.
7. Vous pouvez fusionner la branche `changes-incluant-B` avec `master` et supprimer `changes-incluant-B` ou simplement passer à `changes-incluant-B` et y travailler.

## Useful commands

- `git log --oneline --graph --all`
- `git switch <branch-name>`
- `git rebase <branch-name>`
- `git branch <branch-name>`
- `git reset --soft HEAD~`
- `git branch -d <branch-name>`
- `git merge <branch-name>`
