# Git Kata: fusion inversée

Dans ce kata, nous explorons les problèmes liés à l'annulation d'un commit de fusion.

## L'histoire

Votre équipe utilise cette incroyable bibliothèque-1.2.3 pour son développement, qui est
entretenu par une autre équipe.

À un moment donné, votre équipe intègre une nouvelle version de la bibliothèque-1.2.4. Parce que vous êtes
prudent, vous faites cela sur une branche `integrate-library-1.2.4`.

Malheureusement, vous découvrez après votre fusion que la bibliothèque a un bogue, qui
doit être réparé par cette autre équipe. Pour éviter que le bogue ne soit publié dans
production, vous décidez d'annuler le commit de fusion.

## Installer

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Annulez le commit de fusion. Pour résoudre le conflit, vous devez déterminer ce que
les fonctionnalités doivent être incluses dans `mymodule.txt`.
   * Vous pouvez dire si la fonctionnalité X doit être incluse ou non selon le moment où elle a été
     engagé.
   * Vous pouvez supposer que la fonctionnalité Y fonctionne également avec l'ancienne version de la bibliothèque.
2. Prenez le rôle de l'équipe de la bibliothèque et corrigez le bogue dans la bibliothèque sur le
   branche intégrée, par ex. changez `lib.txt`.
3. Ensuite, nous explorons comment vous pouvez obtenir les modifications de la branche dans le maître
   encore. Essayez d'abord de fusionner pour voir ce qui se passe. Le fichier `lib.txt` change comme
   attendu, mais '`mymodule.txt` ne le fait pas. Pour une discussion approfondie de
   la raison pour laquelle, consultez cet essentiel: [Reverting a faulty merge](https://github.com/git/git/blob/master/Documentation/howto/revert-a-faulty-merge.txt).

> annuler également un commit de fusion
> annule les _data_ que le commit a changé, mais c'est absolument le cas
> rien aux effets sur l'_histoire_ que la fusion a eus.
>
> Ainsi, la fusion existera toujours, et elle sera toujours considérée comme une adhésion
> les deux branches ensemble, et les futures fusions verront cette fusion comme
> le dernier état partagé

4. Annuler la fusion avec une réinitialisation --hard
5. Annulez le retour et réessayez la fusion. Cette fois ça marche.

## Useful commands

* `git revert -m 1 <merge-sha1>`
* `git log --oneline --graph --all`
* `git add <file-name>`
* `git revert --continue`
* `git switch <branch-name>`
* `git merge <branch-name>`
* `git reset --hard <sha1>`
* `git revert <sha1>`
