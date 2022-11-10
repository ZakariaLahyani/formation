# Git Kata: Branchement de base

## Installer

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous vivez à nouveau dans votre propre branche, cette fois nous allons jongler un peu avec les branches, pour montrer à quel point les branches sont légères dans git.
Astuce : `git switch` vous fera passer d'une branche à l'autre.

1. Utilisez `git branch` pour voir les deux branches pertinentes pour cet exercice
2. Dans quelle branche êtes-vous ?
3. Utilisez `git branch mybranch` pour créer une nouvelle branche appelée _mybranch_
4. Utilisez à nouveau `git branch` pour voir la nouvelle branche créée.
5. Utilisez `git switch mybranch` pour passer à votre nouvelle branche.
6. Comment la sortie de `git status` change-t-elle lorsque vous basculez entre le _master_ et la nouvelle branche que vous avez créée?
7. Comment l'espace de travail change-t-il lorsque vous passez d'une branche à l'autre?
8. Assurez-vous d'être sur votre branche _mybranch_ avant de continuer.
9. Créez un fichier appelé `file1.txt` avec votre nom.
10. "Ajouter" le fichier et "valider" avec cette modification.
11. Utilisez `git log --oneline --graph` pour voir votre branche pointant vers le nouveau commit.
12. Revenez à la branche appelée _master_.
13. Utilisez `git log --oneline --graph` et remarquez comment le commit que vous avez fait sur la branche _mybranch_ est manquant sur la branche _master_.
14. Créez un nouveau fichier appelé `file2.txt` et validez ce fichier.
15. Utilisez `git log --oneline --graph --all` pour voir votre branche pointant vers le nouveau commit, et que les deux branches ont maintenant des commits différents.
16. Basculez vers votre agence _mybranch_.
17. Qu'est-il arrivé à votre répertoire de travail ? Pouvez-vous voir votre `file2.txt`?
18. Utilisez `git diff mybranch master` pour voir la différence entre les deux branches.

## Useful commands

- `git switch`
- `git switch -c`
- `git log --oneline --graph`
- `git branch`
- `git diff`
