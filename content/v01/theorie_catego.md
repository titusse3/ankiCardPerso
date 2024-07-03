# Catégorie

## Fonction injective

Quand dis t'on qu'une fonction $f : E \to F$ est __injective__ ?

%

$f$ est __injective__ ssi $\forall x, x' \in E^2, f(x) = f(x') \Rightarrow x = x'$

[#math](./math.md)

## Fonction surjective

Quand dis t'on qu'une fonction $f : E \to F$ est __surjective__ ?

%

$f$ est __surjective__ ssi $\forall y \in F, \exists  x \in E$ tel que 
$f(x) = y$

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

## Catégorie

Donnez la définition d'une __catégorie__ ?

%

Une __catégorie__ est un certain nombre d'__objet__ et de __flèche__ (appelé 
__morphisme__). Les flèches doivent pouvoir être composé, la composition doit 
être __associative__. Tous les objets doivent avoir une __flèche d'identité__, 
servent de l'indentité dans la composition.

[#categorie](./categorie.md)

## __Hask__

Qu'est ce qu'un __Hask__ ?

%

Un __Hask__ est la cathegory des types en _Haskell_, où les objets sont des 
_ensembles_ contenant tousse l'élément $\bot$. Tous morphisme peut alors 
renvoyer $\bot$ généralement utilisé pour représenter un calcule infini.

[#categorie](./categorie.md) [#programmation](./programmation.md)

## Fonction pure

Donnez la définition d'une __fonction pure__ ?

%

Une fonction est __pure__ ssi :
 - Pour la même entrée, elle retourne toujours le même résultat;
 - La fonction n'utilise et ne produit pas __d'effet de bords__;

[#programmation](./programmation.md)

## Fonction Void

Comment appelle-t-on une fonction de signature $\emptyset \to a$ avec $a$ un 
ensemble quelconque et $\emptyset$ l'ensemble ne contenant aucun élément.

%

Une fonction $f : \emptyset \to a$ porte le nom de __absurde__ 
(_ex falso sequitur quodlibet_).

[#categorie](./categorie.md)

## Fonction vers le type Bool

Comment peut'on appeler une fonction à pour ensemble d'arrivé $\mathbb{B}$.

%

On peut nommés __predicat__ toutes fonction aillant pour ensemble d'arrivé 
$\mathbb{B}$.

[#programmation](./programmation.md) [#math](./math.md)

## Free category

Qu'est-ce qu'une __free category__ ?

%

Une __free category__ est une catégory tel que :
- les objets sont les sommets d'un graphs orienté;
- les morphisms sont les couples de sommet représentant un arc de ce graph;

[#categorie](./categorie.md)

## Préordre

Qu'est ce qu'un __préordre__ ?

%

Un __préordre__ est une relation binaire __réfléxive__ et __transitive__ :
- $\forall x \in E, x \mathcal{R}x$, __réflexivité__;
- $\forall x,y,z \in E, x \mathcal{R} y \land y \mathcal{R} z \Rightarrow x  \mathcal{R} z$, __transitivité__;

[#math](./math.md)

## Ordre partiel

Qu'est ce qu'un __ordre paritel__ ?

%

Un __ordre paritel__ est une relation binaire __réfléxive__, 
__anti-symétrie__ et __transitive__ :
- $\forall x \in E, x \mathcal{R}x$, __réflexivité__;
- $\forall x, y \in E, x \mathcal{R}y \land y \mathcal{R} x \Rightarrow x = y$, 
__anti-symétrie__;
- $\forall x,y,z \in E, x \mathcal{R} y \land y \mathcal{R} z \Rightarrow x  \mathcal{R} z$, __transitivité__;

[#math](./math.md)

## Ordre total

Qu'est ce qu'un __ordre total__ ?

%

Un __ordre total__ est un relation binaire tel que :
$$\forall x, y\in E, x \mathcal{R} y \lor y \mathcal{R} x$$

[#math](./math.md)

## Thin category

Qu'est-ce qu'une __thin category__ ?

%

Une __thin category__ est une catégorie telle qu'il existe au plus un 
__morphisme__ depuis n'importe quel objet $a$ vers n'importe quel objet $b$.

[#categorie](./categorie.md)

## Hom-set

Qu'est ce qu'un __hom-set__ ?

%

Un __hom-set__ est un ensemble de __morphitms__ d'un objet $a$ à un objet $b$ 
dans une catégorie $C$, on le note $C(a,b)$ ou même $Hom_C(a,b)$.

[#categorie](./categorie.md)

## Préordre hom-set

Qu'elle propriété y a t'il sur un __hom-set__ dans un __préordre__ ?

%

Un __hom-set__ dans un __préordre__ est soit vide, soit ne contient qu'un seul 
élément.

[#categorie](./categorie.md)

## Monoid

Qu'est ce qu'un __monoid__ ?

%

Un __monoid__ est définie comme un ensemble muni d'un opérateur binaire. 
Cette opérateur doit être __associatif__ et l'ensemble doit contenir un 
__élément neutre__.

[#categorie](./categorie.md)

## Monoid catégorie

Qu'est ce qu'une __catégorie monoid__ ?

%

Un __monoid__ est une catégorie d'un seul objet, avec des __morphismes__ qui 
suivent les règles appropriées.

[#categorie](./categorie.md)

## Extraction monoid

Expliquer comment à partir d'une catégorie d'un seul élément on peut obtenir 
un __monoid__ ?

%

On prend l'__homo-set__ $M(m, m)$, de seul objet $m$ de la catégorie $M$. 
L'opérateur binaire est celui de la composition des éléments de l'__homo-set__.
- Cette composition de fonction _existe toujours_ par la propriété d'existance
de la composition de morphisme.
- Cette composition est _associative_ par propriété de morphisme.
- Le morphisme d'_identité_ est l'élément neutre.

On peut donc à partir d'une catégorie d'un seul élément, créer un __monoid__.

[#categorie](./categorie.md)

## Catégorie localement petite

Quand dis t'on qu'une catégorie est __localement petite__ ?

%

On dit qu'une catégorie est __localement petite__ lorsque les morphismes entre 
deux objets quelconque forme un ensemble.

[#categorie](./categorie.md)