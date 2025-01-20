# TP 6

## session_start

Pourquoi est ce que `session_start()` doit être placer avant tous code de 
constructions dans body en php ?

%

Car Le code de création de body (les `echo`) partent du principe que l'entête 
de la réponse a déjà été créer et que donc on ne peut rien ajouter a l'entête 
or une session contient généralement un cookie.

## php_self

A quoi correspond `$_SERVER['PHP_SELF']` ?

%

Le chemin vers le fichier php.

## session

Comment accéder ou mettre une valeur dans un session php ?

%

Ajout : `$_SESSION['name'] = value;`

Lecture : `issset($_SESSION['name']) ? $_SESSION['name']`

## session

Que faut t'il ne pas oublier lorsque l'on met en place une session php ?

%

De ne pas oubliter de fermer la session (c'est n'est pas la détruire) avec 
`session_write_close()`.