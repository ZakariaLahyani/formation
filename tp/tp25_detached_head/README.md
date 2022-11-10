# État de la tête détachée

Lorsqu'un utilisateur se retrouve dans un état "tête détachée", c'est une situation effrayante, mais comme nous le savons, Git n'est pas effrayant.

## Installer:

1. Exécutez `source setup.sh` (ou `.\setup.ps1` dans PowerShell)

## La tâche

1. Exécutez `git status` et `git log --oneline --graph --all` pour voir ce qui se passe.
2. Restaurer la normalité dans ce référentiel en passant à `master`

Notez que cette tâche peut sembler plus confuse si vous n'avez pas exécuté `setup.sh` dans votre terminal.

Nous voulons avoir une branche appelée `the-beginning` qui est créée à partir du premier commit avec le message `A`.

3. Pouvez-vous le faire en causant d'abord une tête détachée?

## Useful commands

- `git status`
- `git log --oneline --graph --all`
- `git checkout <ref>` or `git switch --detach <ref>`
