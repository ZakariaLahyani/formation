
## Téléchargement et installation sous Windows

* Téléchargez sur [https://git-scm.com/download/win](https://git-scm.com/download/win) (ou utilisez [Chocolatey](https://chocolatey.org/))
* Installer en utilisant les valeurs par défaut présélectionnées
* Après l'installation, ouvrez Git Bash pour suivre les étapes de configuration

## Configuration initiale de Git

Git veut savoir qui il doit écrire en tant que committer des modifications, etc.
Pour ce faire, configurez le nom d'utilisateur et l'e-mail de l'utilisateur vers Git avec les commandes suivantes :

1. `git config --global user.name "John Doe"`
2. `git config --global user.email "johndoe@example.com`

### Configuration de l'éditeur

Parfois, Git a besoin que vous éditiez un fichier qu'il crée, par ex. le message d'un commit que vous créez.
Par défaut, Git est configuré avec VIM, mais cela a une courbe d'apprentissage abrupte, donc vous pourriez être mieux avec un autre outil de votre choix :

Si vous souhaitez utiliser l'éditeur basé sur cli nano :
- `git config --global core.editor nano`

Pour les potes Windows :
- `git config --global core.editor bloc-notes`

Ou bien d'autres outils que vous connaissez déjà :

- `git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst -notabbar -nosession -noPlugin"`

### Authentification SSH

- Voir https://help.github.com/articles/generating-an-ssh-key pour plus de détails sur l'authentification par rapport aux référentiels compatibles SSH
- Ou exécutez `ssh-keygen` pour générer une paire de clés SSH dans `%USERPROFILE%/.ssh/` :

  `ssh-keygen -t rsa -b 4096 -C "johndoe@example.com"`

  Cela génère des clés publiques/privées nommées `id_rsa.pub`/`id_rsa`, respectivement)
- La clé publique `id_rsa.pub` doit être téléchargée sur votre serveur de dépôt :
  - Pour GitHub, c'est dans _Settings_ -> _SSH and GPG keys_
  - Pour le serveur BitBucket, c'est dans _Gérer le compte_ -> _Clés SSH_