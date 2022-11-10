# Git Kata : fusion à 3 voies

## Installer

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous vivez à nouveau dans votre propre branche, cette fois nous allons jongler un peu avec les branches, pour montrer à quel point les branches sont légères dans git.

1. Créez une branche appelée salutation et basculez vers celle-ci
2. Modifiez le fichier greeting.txt pour qu'il contienne votre message d'accueil préféré
3. Ajoutez les fichiers greeting.txt à la zone de préparation
4. Engagez-vous
5. Revenez à la branche master
6. Créez un fichier README.md avec des informations sur ce référentiel
7. Ajoutez le fichier README.md à la zone de préparation et effectuez la validation
8. Quelle est la sortie de `git log --oneline --graph --all`?
9. Différer les branches
10. Fusionner la branche de salutation dans le maître
11. Quelle est la sortie de `git log --oneline --graph --all` maintenant? Observez le commit de fusion supplémentaire créé avec le message "Merge branch 'greeting'".

## Useful commands

- `git branch`
- `git branch <branch-name>`
- `git branch -d <branch-name>`
- `git switch <branch-name>`
- `git switch -c <branch-name>`
- `git branch -v`
- `git add`
- `git commit`
- `git commit -m`
- `git merge <branchA> <branchB>`
- `git diff <branchA> <branchB>`
- `git log --oneline --graph --all`
