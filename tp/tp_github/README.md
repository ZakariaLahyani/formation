# Github simulation

## Préparation
Séparez-vous en équipes de 3-4. Si vous êtes dans un groupe de 3, alors le Release Manager jouera également le rôle de Développeur 3.

- Release Manager - Responsable de la gestion du référentiel distant, de la fusion des branches
- Développeur 1
- Développeur 2
- Développeur 3

## Exercice

### Release Manager
1. Créez un référentiel public dans votre compte GitHub
2. Ajoutez les 2-3 développeurs supplémentaires de votre équipe en tant que collaborateurs

### Toute l'équipe
1. Clonez le référentiel nouvellement créé sur votre ordinateur (vous pouvez utiliser n'importe quel emplacement pour cet exercice, votre bureau par exemple)
2. Dans le terminal, accédez au répertoire de travail que vous venez de cloner


### DÉVELOPPEUR 1
1. Créez une nouvelle branche appelée fondation et basculez vers celle-ci
2. Créez un fichier nommé index.html
3. Ajoutez la structure HTML de base dans la page, ne vous souciez pas d'inclure quoi que ce soit d'autre
4. Préparez le fichier pour votre prochain commit
5. Valider le fichier
6. Arrêtez-vous et réfléchissez : les autres développeurs ont-ils déjà accès au fichier que vous avez créé ?
7. Poussez la branche vers le référentiel distant et créez une demande d'extraction


### Release Manager
1. Accédez à GitHub et affichez le référentiel que vous avez créé pour votre équipe
2. Sur le côté droit, cliquez sur "Pull requests"
3. Passez en revue les modifications proposées par le développeur 1
4. S'ils semblent bons, approuvez les changements en fusionnant la nouvelle branche de fondation dans le maître

### DÉVELOPPEUR 2
1. Extrayez les dernières modifications du référentiel distant
2. Créez une nouvelle branche nommée quotes et basculez vers celle-ci
3. La page a besoin de contenu. Ajouter un élément <h1> avec un titre pour la page
4. De plus, ajoutez un élément <blockquote> à la page avec votre citation préférée, assurez-vous d'inclure l'auteur
5. Allez-y et créez un fichier nommé style.css, mais ne vous souciez pas encore d'y ajouter quoi que ce soit
6. Organisez vos modifications pour le prochain commit
7. Validez vos modifications
8. Poussez la branche vers le référentiel distant et créez une demande d'extraction

### Release Manager
1. Accédez à GitHub et affichez le référentiel que vous avez créé pour votre équipe
2. Sur le côté droit, cliquez sur "Pull requests"
3. Passez en revue les modifications proposées par le développeur 1
4. S'ils semblent bons, approuvez les changements en fusionnant la nouvelle branche de fondation dans le maître

### DÉVELOPPEUR 3
1. Extrayez les dernières modifications du référentiel distant
2. Créez une nouvelle branche nommée styles et basculez-y
3. Ajoutez quelques styles très basiques dans index.html (par exemple, ajoutez une couleur d'arrière-plan, stylisez la citation)
4. Organisez vos modifications pour le prochain commit
5. Validez vos modifications
6. Vous pensez que l'auteur attribué à la citation est incorrect. Vous croyez que c'est censé être Justin Bieber. Changer l'auteur pour refléter cela
7. Organisez vos modifications pour le prochain commit
8. Validez vos modifications
9. Poussez la branche vers le référentiel distant et créez une demande d'extraction

### Release Manager
1. Accédez à GitHub et affichez le référentiel que vous avez créé pour votre équipe
2. Sur le côté droit, cliquez sur "Pull requests"
3. Passez en revue les modifications proposées par le développeur 3
4. S'ils semblent bons, approuvez les changements en fusionnant la nouvelle branche de fondation dans le maître

### DÉVELOPPEUR 1
1. Votre plus gros client remarque que l'auteur de la citation est complètement incorrect. Le développeur 3 est en vacances et vous êtes chargé de résoudre ce problème
2. Extrayez les dernières modifications du référentiel distant
3. Créez une nouvelle branche nommée hotfix1 et basculez vers celle-ci
4. Corrigez l'auteur
5. Organisez vos modifications pour le prochain commit
6. Validez vos modifications
7. N'envoyez PAS encore vos modifications au référentiel distant

### DÉVELOPPEUR 2
1. Extrayez les dernières modifications du référentiel distant
2. Créez une nouvelle branche nommée authorupdate et basculez vers celle-ci
3. Votre responsable vous a demandé de mettre le nom de l'auteur en majuscules, alors allez-y et faites-le.
4. Organisez vos modifications pour le prochain commit
5. NE validez PAS vos modifications ou ne les poussez pas encore vers le référentiel distant

### DÉVELOPPEUR 1
Poussez la branche hotfix1 vers le référentiel distant et créez une demande d'extraction

### Release Manager
1. Accédez à GitHub et affichez le référentiel que vous avez créé pour votre équipe
2. Sur le côté droit, cliquez sur "Pull requests"
3. Passez en revue les modifications proposées par le développeur 1
4. Approuvez les modifications en fusionnant la nouvelle branche hotfix1 dans master

### DÉVELOPPEUR 2
1. Passer à la branche master
2. Extrayez les dernières modifications du référentiel distant
3. Vous avez remarqué que certains fichiers ont changé et vous souhaitez que la nouvelle branche sur laquelle vous travaillez ait également ces modifications
4. Basculez vers la branche authorupdate existante sur laquelle vous travaillez encore
5. Exécutez git merge master pour obtenir ces mises à jour
6. Vous devriez maintenant avoir un conflit avec les nouvelles modifications qui entrent en conflit avec les vôtres. Résoudre ces conflits
7. Organisez vos modifications pour le prochain commit
8. Validez vos modifications
9. Poussez la branche vers le référentiel distant et créez une demande d'extraction

### Release Manager
1. Accédez à GitHub et affichez le référentiel que vous avez créé pour votre équipe
2. Sur le côté droit, cliquez sur "Pull requests"
3. Passez en revue les modifications proposées par le développeur 2
4. Approuvez les modifications en fusionnant la nouvelle branche authorupdate dans master


### DÉVELOPPEUR 3
1. Extrayez les dernières modifications du référentiel distant
2. Créez une nouvelle branche nommée hotfix2 et basculez vers celle-ci
3. Vous êtes absolument certain que le nom de l'auteur est censé être Justin Bieber. Changez-le à nouveau
4. Organisez vos modifications pour le prochain commit
5. Validez vos modifications
6. Poussez la branche vers le référentiel distant et créez une demande d'extraction

### Release Manager
1. Accédez à GitHub et affichez le référentiel que vous avez créé pour votre équipe
2. Sur le côté droit, cliquez sur "Pull requests"
3. Passez en revue les modifications proposées par le développeur 3
4. Cette fois, vous avez appris votre leçon et au lieu de fusionner, vous laissez un commentaire sur la façon dont cela est incorrect et fermez simplement la demande sans fusionner.
5. Demandez au développeur 3 d'arrêter de faire ça et dites-leur qu'il y a plus dans la vie que Justin Bieber

