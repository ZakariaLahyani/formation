# Git Kata : Marquage des commits
## Installer:

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## Motivation

[Tags](https://git-scm.com/book/en/v2/Git-Basics-Tagging) sont pratiques pour
garder une trace des commits qui dépassent un numéro de version. Une façon de les utiliser est
avec les branches, où nous pouvons marquer les commits dans une branche s'ils heurtent le
numéro de version, par exemple, une branche appelée `version/1.1` peut avoir les balises `1.1.1`,
`1.1.2` etc. Les balises peuvent également être utilisées sans branches.

Il existe deux types de balises, les balises annotées et les balises non annotées. Balises annotées
peut contenir des informations supplémentaires, c'est-à-dire que vous pouvez ajouter une sortie de journal, dans
complément du nom. Outre les balises annotées, vous pouvez créer des balises non annotées
qui n'ont que le nom. Dans certains cas, les balises sans annotations fonctionnent bien,
car le nom de la balise et les modifications du commit contiennent les informations nécessaires.

## La tâche

Pour plus de simplicité, nous allons simplement travailler avec la branche master dans ce kata. Un couple
de balises sont déjà créées.

1. Voir quelles balises ont été créées.
2. Faites un nouveau commit et introduisez une nouvelle balise annotée.
3. Nous avons fait quelques commits. Pouvez-vous ajouter une balise à un commit arbitraire?
4. Le référentiel d'exercices contient une balise annotée. Quel est le message?
5. Peut-être que toutes les balises ne sont pas nécessaires. Supprimez-en quelques-uns.

## Useful commands
- `git tag`
- `git tag -d <tag>`
- `git tag --list <pattern>`
- `git push --tags <branch>`
- `git rev-parse <tag>`
- `git show`
