# Git katas: Git reset
Nous pouvons très bien manipuler l'Histoire. Nous ne devrions jamais bricoler avec notre histoire locale. En tant que publication publique, les commits doivent s'attendre à être immuables.

Nous utilisons la réinitialisation pour désactiver le changement, mais nous pouvons également faire beaucoup plus de choses différentes.

## Installer

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## Tâche

1. A quoi ressemble votre répertoire de travail ?
2. À quoi ressemble votre journal? A quoi ressemble votre scène ?
3. Essayez de lancer `git reset --soft HEAD~1`
4. Qu'advient-il de votre répertoire de travail, de votre log et de votre stage ?
5. Lancez `git reset --mixed HEAD~1`
6. Qu'advient-il de votre répertoire de travail, de votre log et de votre stage ?
7. Lancez `git reset --hard HEAD~1`
8. Qu'advient-il de votre répertoire de travail, de votre log et de votre stage ?
9. Essayez maintenant d'utiliser `git revert HEAD~1`
10. Qu'advient-il de votre répertoire de travail, de votre log et de votre stage ?

## Useful commands

- `git log --oneline`
- `git commit --amend`
- `git status`
- `git reset --soft`
- `git reset --mixed`
- `git reset --hard`
- `git revert`

## Further explanation

Ce qui suit est tiré de la section Récapitulatif de [https://git-scm.com/book/en/v2/Git-Tools-Reset-Demystified].
La commande reset écrase ces trois arborescences dans un ordre spécifique, s'arrêtant lorsque vous lui dites de:
1. Déplacez ce vers quoi la branche HEAD pointe (arrêtez-vous ici si --soft)
2. Faites en sorte que la scène ressemble à HEAD (arrêtez-vous ici sauf si --hard)
3. Faites en sorte que le répertoire de travail ressemble à la scène