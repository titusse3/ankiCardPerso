# TP1

## Q1 
Comment identifiez le répertoire personnel, ainsi que le groupe par défaut d'un utilisateur sur linux ?

%

cat /etc/passwd

## Q2

Quelle(s) commande(s) permet(tent) d'ajouter un groupe au système ?

%

groupadd

## Q3

Quelle commande permet d'associer un utilisateur déjà existant à un autre groupe ?

%

usermod -a -G <group> <user>

## Q4

Quelle commande permet d'obtenir la liste des groupes auxquels un utilisateur appartient ?

%

groups <user>

## Q5

Si un utilisateur appartient à plusieurs groupes, comment peut-il choisir son groupe actif par défaut ?

%

usermod -g <group>

## Q6

Que fais su -l <user> ?

%

prend l'identiter du user depuis un login shell

## Q7

Que fais su -m <user> ?

%

préserve l'environement du user qui execute la commande. Donc ne modifie pas HOME, SHELL ect..

## Q8

A quoi correspond $HOME ?

%

Le répertoire par défaut 

## Q9

A quoi correspond le fichier /var/log/auth.log ?

%

Il référence les tentatives d'authentification. Que ce soit local, ssh ect...

## Q10

Pour quelle faut t'il priviliger sudo a su root ?

%

dans su root on a pas le log des commandes executer en tant que root alors que sudo si
## Q11

Que fais la commande lastb ?

%

elle affiche les derniers compte connecter sur le système

## Q12

Que fais la commande chage ?

%

elle affiche les informations relative au mdp d'un user (validiter, durée dernier changement ect, info contenu dans /etc/shodow)

## Q13

Que fais umask ?

%

equivalent a chmod mais avec des masques.

## Q14

Que fais chmod a+s ?

%

donne les droit d'andosement a un binaire, il permet a l'executable d'avoir les droit sudo

## Q15

Comment afficher toutes les variables d'environement ?

%

printenv

## Q16

Comment modifier le fichier /etc/sudoers ?

%

il ne faut pas le modifier, il faut créer ou modifier des fichier dans le repertoire /etc/sudoers.d/

## Q17

Comment exporter de manière permanent la valeur d'une variable d'environement ?

%

En utilisant la commande export <VARIABLE>=<VALUE>

## Q18

Donner le contenu des d'env variables suivantes LANG, LC_TIME, HOME, PATH

%

- LANG => Langue utilisé et encodage
- LC_TIME => Format du temps 
- HOME => repertoire maison du user
- PATH => Les chemin de recherche de commande

## Q19

A quoi sert la commande visudo ?

%

elle permet d'éditer le fichier /etc/sudoers qui gère les changements d'identité a l'aide de la commande sudo

## Q20

Comment donner les droit sudo a un user ?

%

usermod -aG sudo tux
