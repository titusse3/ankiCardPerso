# TP2

## CSS

Que veut dire **CSS** ?

%

**Cascade Style Sheets**

## CSS

Donner les deux moyens d'inclusion de fichier CSS ?

%

Dans l'html :
<link rel="stylesheet" type="text/css" href="url_css.css" />

Dans un fichier css :
@import url(url_fichier.css);

## Media

A quoi sert media dans une feuille css ?

%

Il s'agit du type d'écran sur lequelle le docuement html va être rendu. On peut donc faire varier le style en fonction de la valeur de cette attribut.

## CSS 

Que fais le Selecteur ```e1 e2``` en CSS ?

%

Il selectionne tous les ```e2``` descendants de ```e1```.

## CSS

Que fais le selecteur ```e1 > e2``` en CSS ?

%

Il selectionne tous les ```e2``` fils directs de ```e1```.

## CSS

Que fais le selecteur ```e1 + e2``` en CSS ?

%

Il selectionne tous les ```e2``` successeurs de ```e1```.

## CSS

Que fais le selecteur ```e1 ~ e2``` en CSS ?

%

Il selectionne tous les ```e2``` suivant indirectement un ```e1```.

## CSS

Que fais le selecteur ```e1, e2, e3 ...``` en CSS ?

%

Il selectionne tout noeuds satisfaisant au moins une des expressions de ```e1, e2, e3, ...```.

## CSS

Définir ce qu'est la propriété de **cascade** en CSS.

%

La **cascade** est la propriété d'une rêgle CSS, qui permet ou non a cette rêgle de ce propager dans ces sous-arbres (enfant mais aussi enfant de ces enfants ect).

## CSS

Si deux rêgle CSS on la même priorité laquelle s'applique ?

%

Il s'agit de la dernière qui est appliquer.

## CSS

Expliquer comment est calculer la priorité d'une rêgle CSS ?

%

La priorité d'une rêgle est un nombre a quatre 'chiffre' (pas vraiment):

\\(x_4x_3x_2x_1\\)

où :
- x_4 vaut 1 si le style est prioritaire (en ligne c-a-d dans le html ou qu'il contient ```!important```) ;
- x_3 est le nombre d'identifiants (ids) dans le sélecteur ;
- x_2 est le nombre de classes dans le sélecteur ;
- x_1 est le nombre d'éléments séparés par des espaces dans le sélecteur ;

## CSS

Dans qu'elle ordre sont placer les éléments décrit par la propritété ```float``` en CSS.

%

Dans l'ordre d'appartition dans le html
exemple : 
HTML
```
      <div class="test1"></div>
      <div class="test2"></div>
      <p>je suis un gros texte qui n'attend rien</p>
```
CSS
```
.test1, .test2 {
  width: 3vw;
  height: 3vh;
  background-color: red;
}
.test1 {
  float: right;
  background-color: pink;
}
.test2 {
  float: right;
}
```
Alors c'est test1 tout a droite et test2 a la gauche de test1

## CSS

Que fais la propritété ```clear:<val>``` en CSS ?

%

Elle clear le buffer pour les floats.
Si le buffer clear est celui de droite alors retour a la ligne pour la droite. 
Si celui de gauche la même mais a gauche.

## CSS 

Pour qu'elle type de poisition la position absolute ne se réfère pas a son parent directe ?

%

Pour la position static (celle par défaut).

## CSS

Comment sont comparer les valeurs de z-index ? autrement dis quelle sont les valerus mise en avant ?

%

Les valeurs les plus grands sont celle que l'on met en avant. Par exemple : 999 sera un plan avant le z-index 1.
