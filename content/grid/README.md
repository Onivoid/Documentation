# CSS Grid (Très Simplifié - Essentiel)
> CSS Grid est une méthode de disposition en grille en CSS, qui permet de créer des mises en page complexes avec des arrangements de colonnes et de lignes. Il permet de placer des éléments dans des cellules de grille, de spécifier leur taille, de les aligner, de les répartir, etc. Le modèle de disposition en grille est basé sur une grille (élément parent) et ses cellules (éléments enfants), qui sont disposés en fonction des propriétés spécifiées dans le CSS.

# Propriétés de CSS Grid
 * `display: grid;` : Indique que l'élément parent est une grille CSS.
 * `grid-template-rows: <track-size>...;` : Définit la hauteur des lignes de grille, en spécifiant une liste de tailles de piste séparées par des espaces ou des barres obliques. Vous pouvez également utiliser des mots-clés comme `auto`, `min-content`, `max-content` ou `fit-content`.
 * `grid-template-columns: <track-size>...;` : Définit la largeur des colonnes de grille, en spécifiant une liste de tailles de piste séparées par des espaces ou des barres obliques. Vous pouvez également utiliser des mots-clés comme `auto`, `min-content`, `max-content` ou `fit-content`.
 * `gap: <row> <gap>;` : Une abréviation pour les deux propriétés précédentes, en spécifiant l'espace vertical et horizontal en une seule ligne.

## Exemples d'applications : 

### Application N°1 de Grid
> Nous voulons faire une grille avec un nombre de colonne automatique selon la disponible

<iframe width="100%" height="300" src="//jsfiddle.net/Skullyfox/hokzrx4n/2/embedded/html,css,result/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>

Dans cet exemple nous utilisons : 
* `grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));` : la valeur `repeat()` qui prend en compte 2 paramêtres, le premier paramêtre définit le nombre de répétitions, ici nous avons utilisé "auto-fit", qui vas créer automatiquement le nombre de colonne requise pour remplir l'espace disponible, puis en deuxième paramêtres, nous avons défini la largeur **qu'une colonne doit avoir**, ici nous avons utilise la méthode **minmax()** qui prend en premier paramêtre le minimum et en deuxième le maximum. 
> _**Rappel :** 1fr = une fraction => **Exemple :** repeat(2, 1fr) de 300px, grid fera 2 colonne de 150px de largeur_
* `gap: 10px;` : Défini l'espacement entre les blocs de 10px sur l'axe vertical et horizontal.
> _**Note :** Dans cet exemple édité le **06 Mai 2023**, nous utilisons `gap`, hors sur la documentation officielle de grid, vous verrez certainement `grid-gap`, qui fonctionnera toujours mais `grid-gap` est devenue obsolète et a été remplacé par `gap`._

### Application N°2 de Grid
> Cette fois-ci nous voulons juste avoir une grille de 2 colonnes

<iframe width="100%" height="300" src="//jsfiddle.net/Skullyfox/2u63xzo0/4/embedded/html,css,result/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>

### Application N°3 de Grid avec Flex
> Avec l'exemple précédent, en rajoutant du contenu dans les boxs, j'aimerais organiser le contenu en le centrant dans mes blocs

<iframe width="100%" height="650" src="//jsfiddle.net/Skullyfox/2u63xzo0/10/embedded/html,css,result/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>