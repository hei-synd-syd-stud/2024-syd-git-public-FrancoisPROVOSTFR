# Answers of Francois PROVOST FrancoisPROVOSTFR

## Basics
### Task 1
Après le clonage du Git Repo, le répertoire contient :
- `answers.md` : Fichier pour noter les réponses aux questions du TP.
- `img/` : Dossier pour stocker des images ou fichiers annexes pour le TP.
- `.git/` : Dossier caché contenant les informations de suivi de version pour le dépôt.


### Task 2
- `git status` : Le fichier `README.md` apparaît comme "untracked" (non suivi), car il a été créé mais pas encore ajouté au suivi de version.
- `git log --oneline` : Aucun changement n'apparaît car `README.md` n’a pas encore été ajouté ni commité, donc il ne figure pas dans l'historique.

### Task 3
Après avoir ajouté `README.md` au stage avec la commande `git add README.md`, `git status` montre que le fichier est maintenant en "staged" (prêt pour le commit) au lieu de "untracked". Il est listé sous "Changes to be committed".

### Task 4
Après avoir modifié `README.md` avec du texte, `git status` montre que le fichier est listé sous "Changes not staged for commit" (modifié mais non ajouté au stage), car il a été modifié depuis le dernier ajout au stage.

### Task 5
La première ligne dans `git log --oneline` montre le commit que je viens de faire. Elle contient :
- Une chaîne de caractères (le SHA1 abrégé) qui identifie de manière unique le commit.
- `HEAD` indique que c’est le dernier commit de la branche actuelle.
- `main` montre la branche sur laquelle je travaille.
- Le message du commit qui décrit les modifications : "ADD: README file with initial content".

### Task 6
Après avoir utilisé `git checkout` pour revenir au premier commit, le répertoire reflète l'état du projet à ce moment-là. Certains fichiers peuvent ne pas être présents s'ils ont été ajoutés dans des commits ultérieurs. En revenant ensuite sur la branche principale avec `git checkout main`, tous les fichiers et modifications récentes sont restaurés.

## Gitgraph

### Task 7
1. Nommer tous les éléments visibles dans la Fig. 13 (points 1 à 10) :
   - 1 : Branche `develop`
   - 2 : SHA du commit `baa6795`
   - 3 : Message de merge "Merge branch 'feature-auth' into 'develop'"
   - 4 : Auteur du commit `ByteMe Bob <bob.byteme@hevs.ch>`
   - 5 : Tag `v1.0.0`
   - 6 : Branche `feature-auth`
   - 7 : SHA du commit `c93cfcc`
   - 8 : SHA du commit `b205e38`
   - 9 : SHA du commit `e209ecc`
   - 10 : SHA du commit `79bc77a`

![Gitgraph](img/gitgraph.svg)