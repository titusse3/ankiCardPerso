# Catégorie

## Fonction injective

Quand dis t'on qu'une fonction $f : E \to F$ est __injective__ ?

%

$f$ est __injective__ ssi $\forall x, x' \in E^2, f(x) = f(x') => x = x'$

[#math](./math.md)

## Fonction surjective

Quand dis t'on qu'une fonction $f : E \to F$ est __surjective__ ?

%

$f$ est __surjective__ ssi $\forall y \in F, \exists  x \in E$ tel que $f(x) = y$

[#math](./math.md)

## Fonction bijective

Quand dis t'on qu'une fonction $f : E \to F$ est __bijective__ ?

%

$f$ est une __bijection__ de $F$ vers $E$ si tous les éléments de l'ensemble 
d'arriver $F$ a exactement un __antécédent__ dans $E$ par $f$, ce qui 
s'écrit formellement :
$$\forall x \in E, \exists! x \in E,  f(x) = y$$

[#math](./math.md)

## Ensemble dénombrable

Quand dis t'on qu'un ensemble $E$ est __dénombrable__ ?

%

$E$ est __dénombrable__ ssi $\exists f, f : E \to \mathbb{N}$ avec $f$ une 
__bijection__.

[#math](./math.md)

## Propriété composition catégorie

Quelle sont les propritées qu'une __composition__ d'une __catégorie__ doit 
satisfaire ?

%

1. La __composition__ doit être __associative__. Soit $f, g, h$ trois 
  __morphisms__ qui peuvent être composer, alors
  $$h \circ (g \circ f) = (h \circ g) \circ f = h \circ g \circ f$$
2. Pour toutes objets $A$, il doit y avoir le __morphisme d'indentité__ notée 
  $id_A$ qui doit vérifier pour une fonction $f : A \to B$ :
  $$f \circ  id_A = f \text{ et } id_B \circ f = f$$

[#math](./math.md) [#categorie](./categorie.md)

## Catégorie

Donnez la définition d'une __catégorie__ ?

%

Une __catégorie__ est un certain nombre d'__objet__ et de __flèche__ (appelé 
__morphisme__). Les flèches doivent pouvoir être composé, la composition doit 
être __associative__. Tous les objets doivent avoir une __flèche d'identité__, 
servent de l'indentité dans la composition. 

## __Hask__

Qu'est ce qu'un __Hask__ ?

%

Un __Hask__ est une catégorie générallement de type, où les objets sont des 
_ensembles_ contenant tousse l'élément $\bot$. Tous morphisme peut alors renvoyer $\bot$ (généralement utilisé pour représenter un calcule infini).

