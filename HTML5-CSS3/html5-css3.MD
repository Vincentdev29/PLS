# Documentation HTML5 - CSS3

Source : [Openclassrooms](https://openclassrooms.com/fr/courses/1603881-apprenez-a-creer-votre-site-web-avec-html5-et-css3)

HTML : HyperText Markup Language (Fond, contenu logique) - CSS  : Cascading Style Sheets (Forme, habillage)

## Les Bases
Doctype
```html
<!DOCTYPE html>
```

Corps par défaut d'une page HTML
```html
<html>
  <head>Informations de la page : titre, encodage...</head>
  <body>Corps de la page Web</body>
</html>
```

L'encodage
```html
<!-- Il existe de multiples encodages :  ISO-8859-1, OEM 775, Windows-1253, ANSI, UNICODE-->
<meta charset="utf-8" />
```

Le titre de la page
```html
<!-- Le titre est affiché dans l'onglet du navigateur -->
<title>Titre</title>
```

## Organisation du texte
###### Les paragraphes
```html
<p>Un paragraphe quelconque</p>
```

###### Saut de ligne
```html
<p>Un paragraphe quelconque 1</p>
<p>Un paragraphe quelconque 2</p>
```
On peut aussi utiliser <br /\>

###### Les titres
Il ne définisse pas une taille ou une police par défaut mais des niveaux de titres, c'est pour structurer. (Max h6)
```html
<h1>Titre 1</h1>
<h2>Titre 2</h2>
```

###### Mise en valeur
```html
Emphase                            (défaut : italique)  : <em></em>
Importance                         (défaut : gras)      : <strong></strong>
Marquer le texte, visuel percutant (défaut : surligner) : <mark></mark>
```

###### Les listes
Liste non ordonnée, puce sans numéro
```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>
```

Liste ordonnée, puce numérotée
```html
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
</ol>
```

## Création de lien
##### Les liens
```html
<a href="https://unsitedevente.com">Le lien</a>
Si dans le lien il y a '&' remplacer par '&amp' (format HTML5)

<a href="https://unsitedeventep2.com">La page 2 du site</a>
<a href="site/unsitedeventep2.html">On peut pointer aussi un fichier</a>
Recap lien possible : URL, chemin relatif ou absolu
```

##### Les ancres



```
```
