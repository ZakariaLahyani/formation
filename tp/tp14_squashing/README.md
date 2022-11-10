# Squash commet

Dans ce kata je voudrais nettoyer un peu mon histoire.

Les cinq derniers s'engagent tous à bricoler avec file.txt qui contient évidemment ma fonctionnalité.

Je voudrais que ces commits soient écrasés en un seul commit!

Pendant que vous y êtes, j'aimerais vraiment que les vilains caractères `\n` à l'intérieur de `file.txt` soient supprimés de l'historique.

## Installer

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. _Squash_ les cinq commits pertinents en un seul et faites un bon message de commit (voir Informations complémentaires).
2. À quoi ressemble `git log` maintenant?
3. Nettoyez les caractères `\n` dans `file.txt` sans ajouter à l'historique de validation.

## Commandes utiles

- `git rebase -i <ref>`
- "git add"
- `git commit --amend`

## Further information

### The seven rules of a great Git commit message

From [How to Write a Git Commit Message](https://chris.beams.io/posts/git-commit/)

1. Séparez le sujet du corps avec une ligne vide
2. Limitez la ligne sujet à 50 caractères
3. Mettez une majuscule dans la ligne sujet
4. Ne terminez pas la ligne sujet par un point
5. Utilisez le mode impératif dans la ligne sujet
6. Enveloppez le corps à 72 caractères
7. Utilisez le corps pour expliquer quoi et pourquoi vs comment

Example
```
Summarize changes in around 50 characters or less

More detailed explanatory text, if necessary. Wrap it to about 72
characters or so. In some contexts, the first line is treated as the
subject of the commit and the rest of the text as the body. The
blank line separating the summary from the body is critical (unless
you omit the body entirely); various tools like `log`, `shortlog`
and `rebase` can get confused if you run the two together.

Explain the problem that this commit is solving. Focus on why you
are making this change as opposed to how (the code explains that).
Are there side effects or other unintuitive consequences of this
change? Here's the place to explain them.

Further paragraphs come after blank lines.

 - Bullet points are okay, too

 - Typically a hyphen or asterisk is used for the bullet, preceded
   by a single space, with blank lines in between, but conventions
   vary here

If you use an issue tracker, put references to them at the bottom,
like this:

Resolves: #123
See also: #456, #789
```
