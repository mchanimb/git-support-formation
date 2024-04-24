# GIT

- Théorie
   - Mode de fonctionnement
   - Workflow
   - Bonnes pratiques
- Pratique 
   - Revert et reset
   - Rebase et merge
   - Amend 
   - Au secours, il a commit avant moi !

## Théorie

### Mode de fonctionnement

| centralisé                        | décentralisé                    |
| --------------------------------- | ------------------------------- |
| client/serveur distinct           | client serveur non distinct     |
| branche = dossier                 | branche = référence             | 
| ![svnrepo](assets/svn-repo.png)   | ![gitrepo](assets/git-repo.png) |

cycle des lignes de commande git :

![cycle](assets/git.png)

### Workflow

#### Master only

![master](assets/master-only.png)

| point négatif                       | point positif | 
| ----------------------------------- | ------------- |
| Pas adapter au travail collaboratif |               |
| Développement non isolé             |               |
| Déploiement continue impossible     |               | 

#### Feature branch 

![feature](assets/feature-branch.png)

| point négatif                            | point positif                   | 
| ---------------------------------------- |-------------------------------- |
|                                          | Adapter au travail collaboratif |
|                                          | Développement isolé             |
| Déploiement continue toujours impossible |                                 |

#### Gitflow

![gitflow](assets/gitflow.png)

| point négatif | point positif                     | 
| ------------- | --------------------------------- |
|               | Adapter au travail collaboratif   |
|               | Développement isolé               |
|               | Déploiement continue possible     |

### Bonnes pratiques

- .gitignore (pas de fichier de conf de l'application, de votre IDE, de dépendance, ...)
- message de commit et nom de branche standardisé
- pas d'identifiant/mot de passe
- pas de code commenté 
- commit atomique

## Pratique

### Revert et reset : https://github.com/mchanimb/git-revert-and-reset 
- faire un revert du commit de la feature B 
- faire un reset jusqu'au commit du main code

### Merge : https://github.com/mchanimb/git-merge 
- faire un merge de la branche feature/b dans master

### Rebase et merge : https://github.com/mchanimb/git-rebase-and-merge 
- faire un rebase de la branche feature/b sur master
- faire un merge de la branche feature/b dans master 

### Amend : https://github.com/mchanimb/git-amend
- corriger le contenu du fichier README.md et du message de commit

### Au secours, il a commit avant moi ! : https://github.com/mchanimb/git-conflit
- en duo, faire un commit chacun et gérer le conflit chez le dernier qui a commit  

### Cherry pick : https://github.com/mchanimb/git-cherry-pick
- récupérer le commit de la feature A sur la branche de la feature B
