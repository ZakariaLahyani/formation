# Git Kata: mise en scène de base

Ce kata examinera la zone de staging de git.

Dans git, nous travaillons avec trois domaines différents:

* Le répertoire de travail où vous effectuez vos modifications
* La zone de préparation où toutes les modifications que vous avez ajoutées via `git add` resteront
* Le référentiel où chaque commit se termine, créant votre historique. Pour mettre vos modifications par étapes ici, vous émettez la commande `git commit`.

Un fichier peut avoir des modifications à la fois dans le répertoire de travail et dans la zone de staging.
Ces changements ne doivent pas nécessairement être les mêmes.

Nous travaillerons également avec `git restore` pour restaurer les modifications par étapes d'un fichier, et `git checkout` pour ramener un fichier à un état antérieur.

## Installer

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

Vous vivez dans votre propre référentiel. Il existe un fichier appelé `file.txt`.

1. Quel est le contenu de `file.txt`?
2. Écrasez le contenu dans `file.txt`: `echo 2 > file.txt` pour changer l'état de votre fichier dans le répertoire de travail (ou `sc file.txt '2'` dans PowerShell)
3. Que vous dit `git diff`?
4. Que vous dit `git diff --staged`? pourquoi est-ce vide?
5. Exécutez `git add file.txt` pour mettre en scène vos modifications à partir du répertoire de travail.
6. Que vous dit `git diff`?
7. Que vous dit `git diff --staged`?
8. Remplacez le contenu de `file.txt`: `echo 3 > file.txt` pour modifier l'état de votre fichier dans le répertoire de travail (ou `sc file.txt '3'` dans PowerShell).
9. Que vous dit `git diff`?
10. Que vous dit `git diff --staged`?
11. Expliquez ce qui se passe
12. Exécutez `git status` et observez que `file.txt` est présent deux fois dans la sortie.
13. Exécutez `git restore --staged file.txt` pour annuler la modification
14. Qu'est-ce que `git status` vous dit maintenant?
15. Mettez en scène le changement et faites un commit
16. A quoi ressemble le journal ?
17. Remplacez le contenu de `file.txt`: `echo 4 > file.txt` (ou `sc file.txt '4'` dans PowerShell)
18. Quel est le contenu de `file.txt`?
19. Que nous dit `git status` ?
20. Exécutez `git restore file.txt`
21. Quel est le contenu de `file.txt`?
22. Que nous dit `git status` ?

## Useful commands

- `git add`
- `git commit`
- `git commit -m "My lazy short commit message"`
- `git log`
- `git log -n 5`
- `git log --oneline`
- `git log --oneline --graph`
- `git restore --staged`

## Aliases

You can set up aliases as such:
`git config --global alias.lol 'log --oneline --graph --all'`
This might be useful to you.
