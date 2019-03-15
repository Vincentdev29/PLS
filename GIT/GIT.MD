# Git

# Commande Basique
Clone d'un repository distant
```
git clone repoURL (ex : https://github.com/Vincentdev29/PLS.git)
```

Synchroniser le repository local au repository distante
```
git fetch origin
```

# Branche
Affiche les branches du repository local
```
git branch
```

Affichage des branches locales et distantes
```
git branch -A
```

Création d'une nouvelle branche
```
git branch NomDeBranche
```

Changement de branche de travail
```
git checkout NomDeBranche
```

Ajout d'une branche distante au repository local
```
git checkout  -b branchName origin/branchName
```
