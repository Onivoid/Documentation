# Les Medias Queries
> Les media queries en CSS permettent de modifier la présentation d'un site web en fonction de certaines caractéristiques du périphérique utilisé pour visualiser la page, telles que la taille de l'écran, l'orientation de l'appareil, etc. Les media queries permettent ainsi de créer des mises en page réactives et adaptives, qui s'ajustent automatiquement aux différents périphériques utilisés par les visiteurs.

## Synthaxe
> La media query suivante applique des styles CSS spécifiques lorsque la largeur de l'écran est inférieure ou égale à 768 pixels :
```css
@media screen and (max-width: 768px) {
  /* styles à appliquer si la condition est vraie */
}
```
## Exemples d'utilisation
### Media queries basées sur la largeur de l'écran
> Les media queries basées sur la largeur de l'écran permettent de définir des styles différents en fonction de la taille de l'écran. Par exemple, vous pouvez définir des styles pour les écrans de petite taille, les écrans de taille moyenne et les écrans de grande taille.
```css
/* Styles pour les écrans de petite taille */
/* Exemple : Le Téléphone */
@media screen and (max-width: 767px) {
  /* styles à appliquer si la condition est vraie */
}

/* Styles pour les écrans de taille moyenne */
/* Exemple : La Tablette */
@media screen and (min-width: 768px) and (max-width: 991px) {
  /* styles à appliquer si la condition est vraie */
}

/* Styles pour les écrans de grande taille */
/* Exemple : Les PC / Télé etc... */
@media screen and (min-width: 992px) {
  /* styles à appliquer si la condition est vraie */
}
```
### Exemple concrêt
> Dans cet exemple concrèt, nous avons une section avec une grille, nous voulons que sur PC il y ai 4 colonnes, sur tablette qu'il y en ai 2, et que sur mobile il n'y ai qu'une seule colonne.
> 
> **⚠️ INUTILE de recopier tout les paramètres dans les media queries, copier uniquement les paramètres que vous voulez changer ⚠️**

<iframe width="100%" height="700" src="//jsfiddle.net/Skullyfox/hokzrx4n/12/embedded/html,css,result/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>


