# Les Chemins de fichiers
**_Dans cette partie, vous verrez la façon d'écrire vos chemins de fichiers dans le cadre du Développement Web_**

## Importation dans un fichier HTML
### Architecture de dossier pris pour l'exemple : 
> Pour les exemples qui suivront, nous allons prendre en exemple cette architecture de dossier :
```sh
| Index.html
|
| img
|   |--/logo.png
|   |--/avatar.png
|   |--/banner.jpg
|
| css
|   |--/index.css
|   |--/reset.css
|   |--/colors.css
|
| js
|   |--/index.js
|   |--/animations.js
```
### Lier une image au HTML
> Pour lier une image qui se trouve dans le dossier `img` voici le chemin que vous devriez faire :
```html
    <!-- index.html -->
    <img src="./img/logo.png" />
```
> Explication du lien :
> L'instruction `./` désigne le fait de rechercher dans le dossier du fichier dans lequel nous faisons appel à cette instruction,
> dans notre cas, nous faisons appel à cette instruction dans le fichier `index.html` se trouve au même niveau que nos dossiers `img`, `css` et `js`.

Ensuite après l'instruction `./` nous écrivont l'instruction `img/`, quand nous écrivons un nom tel que `img`suivit d'un `/` cela veut dire que nous allons
chercher un dossier du nom de `img`, du coup l'instruction complète `./img/` veut dire que nous cherchons un dossier `img` qui est au même niveau que le fichier
`index.html`.

Maintenant que nous sommes rentré dans le dossier `img/` nous lui renseignons le fichier que nous voulons, et pour cela nous allons l'appeler par son nom et son extension comme cela : `logo.png`.

**Il est important de bien respecter la casse, les noms de dossiers et de fichiers doivent être écrits à l'identique.**

### Lier une image dans un fichier CSS
> Ci-dessous vous verrez un exemple de chemin pour allez chercher une image dans le dossier `img` en partant du dossier `css` :

```css
/* css/index.css */
div{
    background: url('../img/logo.png');
}
```
> Explication du lien : L'instruction `../` désigne le fait de sortir du dossier actuel, donc une fois qu'on sort du dossier `css` en faisant `../`,
> nous pouvons allez chercher notre image dans le dossier `img`

## Lexique
* `./` : Ce dossier
* `../` : Sortir du dossier
* `img/` : Dossier qui s'appel `img`
* `img/logo.png` : Image au format `.png`, qui se nomme `logo`, et qui se trouve dans le dossier `img/`