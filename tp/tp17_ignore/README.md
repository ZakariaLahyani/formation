# Git Kata: Ignorer de base
Nous allons travailler un peu avec le fichier `.gitignore` dans ce kata.
Dans ce fichier, vous pouvez spécifier à la fois les extensions de fichier et les structures de dossiers que vous ne souhaitez pas que Git suive.
Vous pouvez toujours `git add` les fichiers et dossiers qui sont ignorés dans le fichier `.gitignore`.

Nous travaillerons également avec `git rm`, qui est la commande Git remove. `git rm` fait exactement la même chose que supprimer un fichier de votre répertoire de travail, puis mettre en scène ce changement en émettant un `git add filename` sur le fichier qui vient d'être supprimé.
Parfois, vous ajoutez accidentellement un fichier qui n'était pas destiné à Git, par exemple. fichiers binaires, fichiers de classe, etc.

Si vous voulez signaler à Git qu'un fichier doit être supprimé de git, mais que vous le voulez toujours dans votre répertoire de travail, utilisez alors `git rm --cached` pour émettre une commande de suppression sur la zone de staging, mais pas dans votre travail annuaire.


## Installer:

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Créez un fichier avec le nom `foo.s`
2. Quelle est la sortie de `git status`?
3. Créez un fichier `.gitignore` dans votre répertoire de travail contenant `*.s`
4. Quelle est la sortie de `git status`?
5. Validez le fichier `.gitignore`
6. Validez `file1.txt`
7. Ajoutez les fichiers `txt` à `.gitignore` en ajoutant une ligne dans le fichier contenant `*.txt`
8. Que nous dit `git status` ?
9. Modifiez `file1.txt`
10. Que nous dit `git status` ? Pourquoi le fichier a-t-il été suivi alors que l'extension "txt" se trouve dans le fichier ignoré?
11. Créez un autre fichier texte dans le référentiel, à quoi ressemble `git status` maintenant? Pourquoi n'est-il pas suivi ?
12. Étape la suppression de `file1.txt` avec la commande `git rm --cached`
13. Que dit `git status` ?
14. Créez un nouveau fichier appelé `file2.txt` et ajoutez la ligne `!file2.txt` à `.gitignore`. (Voir note ci-dessous)
15. Que dit `git status` ? Pouvez-vous penser à un cas d'utilisation pour suivre un fichier bien que l'extension soit ignorée?

## Useful commands
- `git rm`
- `git add`
- `git commit`
- `git commit -m`
- `git rm --cached`

