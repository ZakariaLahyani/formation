# Git Kata: retour de base
## Installer:

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Dans cette tâche, quelques changements se sont glissés, que nous aimerions sortir. Notre histoire est publique, nous ne pouvons donc pas simplement la changer. Nous devons plutôt utiliser revert pour supprimer les modifications indésirables de manière sûre.

1. Utilisez `git log --oneline` pour consulter l'historique
2. Utilisez `cat` pour afficher le contenu de `greeting.txt`
3. Utilisez `git revert` sur le dernier commit, pour supprimer les modifications ajoutées par le dernier commit
4. Utilisez `git log --oneline` pour afficher l'historique
5. La commande revert a-t-elle ajouté ou supprimé un commit?
6. Utilisez `cat` pour afficher le contenu de `greeting.txt`
7. Utilisez `ls` pour voir le contenu de l'espace de travail
8. Utilisez `git log --oneline` pour trouver le sha du commit en ajoutant les informations d'identification au référentiel
9. Utilisez `git revert` pour annuler le commit qui a ajouté les informations d'identification
10. Utilisez `git log --oneline` pour afficher l'historique
11. Utilisez `ls` pour voir le contenu de l'espace de travail
12. Combien de commits ont été ajoutés ou modifiés par le dernier retour?
13. Utilisez `git show` avec le sha du commit que vous avez annulé pour voir que le fichier d'informations d'identification est toujours dans l'historique
14. Comme vous avez maintenant restauré le fichier d'informations d'identification, il est donc supprimé de votre répertoire de travail, est-il également supprimé de git?

## Useful commands
- `git revert <ref>`
- `git log --oneline`
- `git show <ref>`
