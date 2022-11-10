# Git Kata: rebaser la branche

## Installer

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous vivez à nouveau dans votre propre branche, cette fois nous allons jongler un peu avec les branches, pour montrer à quel point les branches sont légères dans git.

1. Quelles branches existent ?
2. Regardez le journal de la branche master
3. Passez à la branche majuscule
4. Comment le journal se compare-t-il au journal sur la branche master ?
5. Rebasez votre branche majuscule avec le maître (`git rebase master`)
6. Que vient-il de se passer ? Dessine le!
7. Passez maintenant à la branche master
8. Fusionner les majuscules dans le maître
9. À quoi ressemble le journal maintenant?

## Useful commands

- `git switch <branch-name>`
- `git rebase <branch-name>`
- `git log --oneline --graph --all`
- `git merge <branch-name>`
