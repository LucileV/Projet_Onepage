# Mode d'emploi pour utiliser font-awesome sur son site internet

Aller sur le site de http://fontawesome.io/

1. Cliquer sur le bouton Download

2. Décliner la proposition de passer à Awesome Pro et cliquer sur bouton "No thanks, just download Font Awesome 4"

3. Un fichier zip nommé "font-awesome-4.7.0" est alors télécharger

4. Retrouver le fichier zip dans le dossier de téléchargement de votre ordinateur

5. Dezipper le fichier, celui ci contient un dossier principal (font-awesome-4.7.0) à l'intérieur duquel se trouve plusieurs sous-dossiers (css, fonts, less, scss) ainsi qu'un fichier texte HELP-US-OUT.txt.txt

6. Copier la totalité du dossier dézippé font-awesome-4.7.0 dans le dossier de votre projet.

7. Dans l'html placer cette ligne dans le head de votre page:

````html
<link rel="stylesheet" href="path/to/font-awesome/css/font-awesome.min.css">
````

**Attention:** Veillez à ce que le chemin vers le fichier awesome.min.css soit bien correct en fonction de la manière dont vous avez organisé les dossiers et sous-dossiers de votre projet.

8. Rendez-vous sur le site http://fontawesome.io/icons/ afin de choisir l'icone de vous désirez intégrer dans votre page web.

9. Cliquer sur l'icone qui vous intéresse. Sur la page dédiée à l'icone choisie, on vous indique un code à placer directement dans votre fichier html à l'endroit où vous voulez voir apparaitre l'icone.

On peut placer les icônes Font Awesome à peu près n'importe où en utilisant le préfixe CSS fa suivi du nom de l'icône. Font Awesome est conçu pour être utilisé avec des éléments inline (nous aimons la balise <i> pour la brièveté, mais l'utilisation d'un <span> est plus sémantiquement correct).

````html
<i class="fa fa-podcast" aria-hidden="true"></i>
````

10. On peut à présent ser rendre sur la page qui explique comment personnaliser les dimensions de l'icone selon nos besoins.Pour augmenter la taille des icônes par rapport à leur conteneur, utilisez les classes fa-lg (augmentation de 33%), fa-2x, fa-3x, fa-4x ou fa-5x.

````html
<i class="fa fa-camera-retro fa-5x"></i> fa-5x
````

11. Il est également possible d'utiliser l'option fa-fw pour définir une largeur fixe aux icones pour qu'elles s'alignent correctement sans décallage dans un menu par exemple.

````html
<i class="fa fa-home fa-fw" aria-hidden="true"></i>
````

12. On peut également utilisez fa-ul et fa-li pour remplacer facilement les puces par défaut dans les listes non ordonnées.

````html
<ul class="fa-ul">
  <li><i class="fa-li fa fa-check-square"></i>List icons</li>
  <li><i class="fa-li fa fa-check-square"></i>can be used</li>
  <li><i class="fa-li fa fa-spinner fa-spin"></i>as bullets</li>
  <li><i class="fa-li fa fa-square"></i>in lists</li>
</ul>
````

13. Utilisez fa-border et fa-pull-right ou fa-pull-left pour tirer facilement des citations ou des icônes d'articles.

````html
<i class="fa fa-quote-left fa-3x fa-pull-left fa-border" aria-hidden="true"></i>
...tomorrow we will run faster, stretch out our arms farther...
````

14. Utilisez la classe fa-spin pour faire pivoter n'importe quelle icône, et utilisez fa-pulse pour la faire pivoter de 8 pas. Fonctionne bien avec fa-spinner, fa-refresh et fa-cog.

````html
<i class="fa fa-refresh fa-spin fa-3x fa-fw"></i>
<span class="sr-only">Loading...</span>

<i class="fa fa-cog fa-spin fa-3x fa-fw"></i>
<span class="sr-only">Loading...</span>

<i class="fa fa-spinner fa-pulse fa-3x fa-fw"></i>
<span class="sr-only">Loading...</span>
````

15. Pour faire pivoter et inverser arbitrairement des icônes, utilisez les classes fa-rotate- * et fa-flip- *.

````html
<i class="fa fa-shield"></i> normal<br>
<i class="fa fa-shield fa-rotate-90"></i> fa-rotate-90<br>
<i class="fa fa-shield fa-rotate-180"></i> fa-rotate-180<br>
<i class="fa fa-shield fa-rotate-270"></i> fa-rotate-270<br>
<i class="fa fa-shield fa-flip-horizontal"></i> fa-flip-horizontal<br>
<i class="fa fa-shield fa-flip-vertical"></i> fa-flip-vertical
````

16. Pour empiler plusieurs icônes, utilisez la classe fa-stack sur le parent, la fa-stack-1x pour l'icône de taille régulière et fa-stack-2x pour l'icône plus grande. fa-inverse peut être utilisé comme une couleur d'icône alternative. Vous pouvez même lancer des classes d'icônes plus grandes sur le parent pour obtenir plus de contrôle sur le dimensionnement.

````html
<span class="fa-stack fa-lg">
  <i class="fa fa-square-o fa-stack-2x"></i>
  <i class="fa fa-twitter fa-stack-1x"></i>
</span>
fa-twitter on fa-square-o<br>
<span class="fa-stack fa-lg">
  <i class="fa fa-circle fa-stack-2x"></i>
  <i class="fa fa-flag fa-stack-1x fa-inverse"></i>
</span>
fa-flag on fa-circle<br>
<span class="fa-stack fa-lg">
  <i class="fa fa-square fa-stack-2x"></i>
  <i class="fa fa-terminal fa-stack-1x fa-inverse"></i>
</span>
fa-terminal on fa-square<br>
<span class="fa-stack fa-lg">
  <i class="fa fa-camera fa-stack-1x"></i>
  <i class="fa fa-ban fa-stack-2x text-danger"></i>
</span>
fa-ban on fa-camera
````



