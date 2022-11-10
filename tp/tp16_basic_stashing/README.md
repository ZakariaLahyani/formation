# Git Kata: stockage de base

## Installer:

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous travaillez sur votre projet. Vous avez mis en scène du travail et avez également du travail non mis en scène.
Soudain, vous êtes informé qu'un bogue est arrivé en production. Vous allez ranger votre travail, corriger le bogue et revenir à votre travail d'origine.

1. Explorer le dépôt
   1. Quel travail avez-vous dans le répertoire de travail?
   2. Quelle œuvre avez-vous mis en scène ?
   3. A quoi ressemble le journal des commits ?
   >* Notez que file.txt comporte des modifications par étapes (c'est-à-dire des modifications dans l'index) et des modifications non par étapes (changements dans le répertoire de travail)*
2. Utilisez `git stash` pour stocker votre travail actuel.
   1. Maintenant, quel travail avez-vous dans le répertoire de travail?
   2. Quelle œuvre avez-vous mis en scène ?
   3. A quoi ressemble le journal des commits ?
   4. A quoi ressemble la liste de cachette ?
3. Corrigez les fautes de frappe dans bug.txt sur master et validez vos modifications.
4. Maintenant, pour revenir à votre travail, appliquez le stash au master.
   1. Quel travail avez-vous dans le répertoire de travail?
   2. Quelle œuvre avez-vous mis en scène ?
   >*Oups. Toutes nos modifications ne sont plus mises en scène maintenant. Cela peut être indésirable et inattendu*
5. Annulez nos modifications avec `git reset --hard HEAD`. Il s'agit d'une commande non sécurisée car elle supprimera définitivement les fichiers de votre index et de votre répertoire de travail, mais nos modifications sont stockées en toute sécurité, donc tout va bien. Consultez le kata [reset](reset/README.md) si vous n'êtes pas sûr de ce qui se passe ici.
6. Appliquez le stash au master avec l'option `--index`.
   1. Quel travail avez-vous dans le répertoire de travail?
   2. Quelle œuvre avez-vous mis en scène ?
   >*Ok, retour là où nous étions!*
7. Nous n'aurons plus besoin de la réserve. Laisse tomber.
   1. A quoi ressemble la liste de cachette ?
   2. A quoi ressemble le journal des commits ?

## Useful commands

- `git status`
- `git status -s`
- `git diff`
- `git diff master`
- `git stash`
- `git stash list`
- `git stash apply`
- `git stash apply --index`
- `git stash drop`
- `git log --oneline --all --graph`
- `git commit`
- `git add`
