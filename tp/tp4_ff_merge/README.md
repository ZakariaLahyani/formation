# Git Kata: fusion rapide

## Installer

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous vivez à nouveau dans votre propre branche, cette fois nous allons jongler un peu avec les branches, pour montrer à quel point les branches sont légères dans git.

1. Créez une branche (fonctionnalité) appelée `fonctionnalité/majuscules` (oui, `fonctionnalité/majuscules` est un nom de branche parfaitement légal et une convention courante).
2. Basculez vers cette branche
3. Quelle est la sortie de `git status`?
4. Modifiez le fichier greeting.txt pour qu'il contienne un message d'accueil en majuscule
5. Ajoutez les fichiers `greeting.txt` à la zone de staging et validez
6. Quelle est la sortie de `git branch`?
7. Quelle est la sortie de `git log --oneline --graph --all`

   *N'oubliez pas: vous souhaitez mettre à jour la branche principale afin qu'elle contienne également toutes les modifications actuellement apportées à la branche de fonctionnalités. La commande 'git merge [nom de la branche]' prend une branche comme argument à partir de laquelle elle prend les modifications. La branche pointée par HEAD (branche actuellement extraite) est ensuite mise à jour pour inclure également ces modifications.*

8. Basculez vers la branche `master`
9. Utilisez `cat` pour voir le contenu des salutations
10. Différer les branches
11. Fusionner les branches
12. Utilisez `cat` pour voir le contenu des salutations
13. Supprimer la branche majuscule

## Useful commands

- `git branch`
- `git branch <branch-name>`
- `git branch -d <branch-name>`
- `git switch`
- `git branch -v`
- `git add`
- `git commit`
- `git commit -m`
- `git merge <branch>`
- `git diff <branchA> <branchB>`
- `git log --oneline --graph --all`
