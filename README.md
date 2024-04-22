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

|             centralisé            |     décentralisé                |
| --------------------------------- | ---------------------------     |
| client/serveur disctinct          |     client serveur non distinct |
|        branche = dossier          |        branche = référence      | 
|  ![svnrepo](assets/svn-repo.png)  | ![gitrepo](assets/git-repo.png) |

cycle des lignes de commande git :

![cycle](assets/git.png)

### Workflow

- Master only
   - <font color="red"> Pas adapter au travail collaboratif </font>
   - <font color="red"> Développement non isolé </font>
   - <font color="red"> Déploiement continue impossible </font>
   
![master](assets/master-only.png)

- Feature branch
   - <font color="green"> Adapter au travail collaboratif </font>
   - <font color="green"> Développement isolé </font>
   - <font color="red"> Déploiement continu toujours impossible </font>

![feature](assets/feature-branch.png)

- Gitflow
   - <font color="green"> Adapter au travail collaborative </font>
   - <font color="green"> Développement isolé </font>
   - <font color="green"> Déploiement continue possible </font>

![gitflow](assets/gitflow.png)

### Bonnes pratiques

- .gitignore (pas de fichier de conf de l'application, de votre IDE, de dépendance, ...)
- message de commit et nom de branche standardisé
- pas d'identifiant/mot de passe
- pas de code commenté 
- commit atomique

## Pratique

- Revert et reset : https://github.com/mchanimb/git-revert-and-reset ou https://gitlab.com/mchanimb/git-revert-and-reset
- Merge : https://github.com/mchanimb/git-merge ou https://gitlab.com/mchanimb/git-merge 
- Rebase et merge : https://github.com/mchanimb/git-rebase-and-merge ou https://gitlab.com/mchanimb/git-rebase-and-merge 
- Amend
- Au secours, il a commit avant moi !
