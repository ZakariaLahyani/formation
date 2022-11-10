# Git kata: s'engager sur la mauvaise branche II

## L'histoire

Vous développez une nouvelle fonctionnalité sur la branche `new-feature`. Tu as déjà
implémenté la première partie d'une fonctionnalité, lorsque vous êtes averti d'un problème critique
bogue qui doit être corrigé immédiatement sur la branche `master`.

Après la correction du bogue, vous continuez à travailler sur la nouvelle fonctionnalité. Après vous être engagé
la deuxième partie de la fonctionnalité, vous vous rendez compte que vous avez fait votre commit sur
la branche `master` au lieu de la branche feature.

## Installer:

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Déplacez le commit défectueux de la branche `master` vers la branche `new-feature`.
2. Comment apporteriez-vous également le correctif à votre branche de fonctionnalité?

## Useful Commands

* `git reset HEAD~1` to move the current branch one step back. This has the consequence of _removing_ the newest commit from a branch
* `git stash` to temporarily save your changes so that you can switch branches
* `git cherry-pick` to add changeset from commit on current branch
