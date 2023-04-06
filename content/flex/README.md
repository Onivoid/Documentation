# Flexbox

> Flexbox est une méthode de disposition flexible en CSS, qui permet de créer des mises en page efficaces et responsives. Il permet de placer des éléments en ligne ou en colonne, de les aligner, de les répartir, etc. Le modèle de disposition en Flexbox est basé sur un conteneur (élément parent) et ses enfants (éléments enfants), qui sont disposés en fonction des propriétés spécifiées dans le CSS.

# Propriétés de Flexbox

* `display: flex;` : Indique que l'élément parent est un conteneur Flexbox.
* `flex-direction: row | row-reverse | column | column-reverse;` : Définit la direction dans laquelle les éléments enfants sont disposés, soit horizontalement (row), verticalement (column), en inversant l'ordre (row-reverse, column-reverse).
* `flex-wrap: nowrap | wrap | wrap-reverse;` : Définit si les éléments doivent être disposés sur une seule ligne (nowrap), sur plusieurs lignes (wrap) ou sur plusieurs lignes en inversant l'ordre (wrap-reverse).
* `justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;` : Définit l'alignement horizontal des éléments enfants, soit à gauche (flex-start), à droite (flex-end), au centre (center), en les espaçant de manière égale entre eux (space-between), en les espaçant avec un espace supplémentaire à gauche et à droite (space-around), ou en les espaçant avec un espace égal entre eux et autour d'eux (space-evenly).
* `align-items: stretch | flex-start | flex-end | center | baseline;` : Définit l'alignement vertical des éléments enfants, soit en les étirant pour remplir toute la hauteur (stretch), en les alignant en haut (flex-start), en bas (flex-end), au centre (center), ou en alignant leurs baselines (baseline).
* `align-content: stretch | flex-start | flex-end | center | space-between | space-around;` : Définit l'alignement vertical des éléments enfants sur plusieurs lignes, soit en les étirant pour remplir toute la hauteur (stretch), en les alignant en haut (flex-start), en bas (flex-end), au centre (center), en les espaçant de manière égale entre eux (space-between), ou en les espaçant avec un espace supplémentaire en haut et en bas (space-around).

## Exemples d'applications : 

### Application N°1 de Flexbox
> Nous avons une section et nous voulons centrer son contenu verticalement et horizontalement : 
<iframe width="100%" height="500" src="//jsfiddle.net/Skullyfox/jbhuz8r7/4/embedded/html,css,result/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>

Comme on le voit, pour centrer le contenu de la section **(enfants)** on applique le flex sur la section **(parents)**.

### Application N°2 de Flexbox

> Nous avons une grille avec plusieurs blocs à l'intérieur, et nous voulons organiser le contenu des blocs, nous voulons centrer celui-ci horizontalement et espacer les blocs entre eux sur l'axe vertical
> 
<iframe width="100%" height="650" src="//jsfiddle.net/Skullyfox/b4efcknm/25/embedded/html,css,result/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>