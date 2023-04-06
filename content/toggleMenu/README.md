# Toogle Menu
> Ici, vous aurez un snipet de code Javascript qui vous permet de faire un Menu Burger

## Exemple 

> Pour voir ce que sa donne, **redimmensionnez votre navigateur** ou **cliquez** sur **"Edit in JSFiddle"**

<iframe width="100%" height="300" src="//jsfiddle.net/Skullyfox/ndrqe9x1/86/embedded/js,html,css,result/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>

## Explication du fonctionnement

### En HTML
> Dans cet exemple j'ai décider de faire ma navigation comme cela : 
<iframe width="100%" height="300" src="//jsfiddle.net/Skullyfox/ndrqe9x1/86/embedded/html/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>

* `<i class="fas fa-bars" id="menuToggler"></i>` : Ce sera le bouton qui activera notre navigation mobile. 
> Lien de la version actuelle de Font Awesome : `https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css`
> À utiliser comme ceci : `<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">`
* `<ul id="navigation">` : Une liste `ul` avec l'ID navigation pour pouvoir la récupérer en JavaScript.
  
### En CSS
> Voici le CSS Responssive de la navigation
<iframe width="100%" height="750" src="//jsfiddle.net/Skullyfox/ndrqe9x1/86/embedded/css/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>

### En JS
> Le javascript à mettre dans la balise `<script> </script>` à la fin de la balise `Body`.
<iframe width="100%" height="300" src="//jsfiddle.net/Skullyfox/ndrqe9x1/86/embedded/js/dark/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>

* `const menuToggler = document.querySelector('#menuToggler');` : On stock l'élément avec l'ID `menuToggler`, comme en CSS, on appel un ID en commençant par `#`.
* `const navigation = document.querySelector('#navigation');` : On stock l'élément avec l'ID `navigation`.
* `menuToggler.addEventListener()` : Fonction qui permet d'écouter un événement sur un élément, là il nous permet d'écouter un événement sur l'élément du bouton de Menu. Cette fonction prend 2 paramètres, le nom de l'évènement puis, une Fonction, qu'on appel généralement un `callback`.
* `menuToggler.classList.toggle('fa-bars');` : On change l'état de la classe `fa-bars`, si elle est présente on l'enlève, sinon on la rajoute. `fa-bars` c'est la classe qui fait appel à l'icone de burger de **FontAwesome**
* `menuToggler.classList.toggle('fa-bars');` : On change l'état de la classe `fa-close`, si elle est présente on l'enlève, sinon on la rajoute. `fa-bars` c'est la classe qui fait appel à l'icone de burger de **FontAwesome**
* `menuToggler.classList.toggle('fa-bars');` : On change l'état de la classe `active`, si elle est présente on l'enlève, sinon on la rajoute.