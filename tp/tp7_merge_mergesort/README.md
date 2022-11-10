# Git Kata: Fusionner Fusionner
Dans ce kata, vous serez confronté à votre premier conflit de fusion!
Il y aura deux branches différentes :

* Mergesort-Impl
* Maître

La tâche consiste à examiner le conflit de fusion et à le résoudre en modifiant le fichier en conséquence.

## Installer:

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Lancez `git branch` pour voir les deux branches présentes
2. Fusionner `Mergesort-Impl` dans `master`
3. Soit:
    1. Résolvez le conflit de fusion avec votre éditeur préféré et terminez la fusion (`git status` vous dira quoi faire), **ou**
    2. Utilisez `git mergetool --tool=emerge` (pour les fans d'emacs) ou `git mergetool --tool=vimdiff` (pour les fans de vim) et terminez la fusion (`git status` vous dira quoi faire)

## Relevant commands
- `git branch`
- `git merge`
- `git status`
- `git mergetool --tool=emerge`
- `git mergetool --tool=vimdiff`
- `git add`
- `git commit`

