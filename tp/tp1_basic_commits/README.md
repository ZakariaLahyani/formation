# Git Kata: Commits de base
Ce kata vous présentera les commandes `git add` et `git commit`.

C'est un kata très introductif. si vous avez utilisé `git status`, `git log --oneline --graph`, `git add` et `git commit` de manière intensive, vous devriez probablement les ignorer.

Vous pouvez regarder au bas de ce fichier, si vous n'avez pas encore fait la configuration de base de git.

## Installer:

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Utilisez `git status` pour voir sur quelle branche vous vous trouvez.
2. À quoi ressemble `git log`?
3. Créer un dossier
4. À quoi ressemble la sortie de `git status` maintenant?
5. `ajouter` le fichier à la zone de préparation
6. À quoi ressemble `git status` maintenant?
7. `commit` le fichier dans le référentiel
8. À quoi ressemble `git status` maintenant?
9. Modifiez le contenu du fichier que vous avez créé précédemment
10. À quoi ressemble `git status` maintenant?
11. `ajouter` le changement de fichier
12. À quoi ressemble `git status` maintenant?
13. Modifiez à nouveau le fichier
14. Faites un `commit`
15. À quoi ressemble le "statut" maintenant? Le "journal"?
16. Ajouter et valider la dernière modification

## Useful commands
- `git add`
- `git commit`
- `git commit -m "My commit message"`
- `git log`
- `git log -n 5`
- `git log --oneline`
- `git log --oneline --graph`
- `touch filename` to create a file (or `sc filename ''` in PowerShell)
- `echo content > file` to overwrite file with content (or `sc filename 'content'` in PowerShell)
- `echo content >> file` to append file with content (or `ac filename 'content'` in PowerShell)


## Git Initial Configuration
1. `git config --global user.name "John Doe"`
1. `git config --global user.email "johndoe@example.com`

For the vim scared:
- `git config --global core.editor nano`

For the windows peeps:
- `git config --global core.editor notepad`

Other editor options:
- `git config --global core.editor "atom --wait"`
- `git config --global core.editor "code --wait"`
- `git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst"`
