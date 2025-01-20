# TP 2

## Raid 

Quel est le principe de fonctionnement d'une configuration de type "bloc-level 
striping with distributed parity" ? A quel numéro RAID est-elle associée ?

%

- Tu découpe ta donner en n-1 groupe et le n ème permet la récupération des 
donners.
- Il s'agit d'un raid de numéro 5.

## Raid

Quel est l'intérêt de monter la structure RAID sur des partitions plutôt que 
d'utiliser directement les disques ?

%

Pour pas que des os comme windows veulent le formater... Grâce au type présente 
pour la partition.

## Raid

Donner la commande pour la création d'un raid 5 avec un spaire.

%

```sh
mdadm --create --verbose /dev/md0 --level=5 --raid-devices=3 /dev/sda1 /dev/sdb1 /dev/sdc1 --spare-devices=1 /dev/sdd1
```

- Avec `/dev/md0`, le nom du raid

## Raid

Comment vérifier qu'un raid est actif ?

%

Il suffit de regarder le fichier `/proc/mdstat`.

## Time

Le `man` de la fonction `time` affiche :

```sh
...
SYNOPSIS
       time   [ -apqvV ] [ -f FORMAT ] [ -o FILE ]
              [ --append ] [ --verbose ] [ --quiet ] [ --portability ]
              [ --format=FORMAT ] [ --output=FILE ] [ --version ]
              [ --help ] COMMAND [ ARGS ]
```
cependant la commande `time --verbose ls` renvoie :

```sh
zsh: command not found: --verbose
--verbose ls  0,00s user 0,00s system 66% cpu 0,002 total
```

Pourquoi ?

%

Car le time exécuter n'est pas celui associer au man de la commande time. Pour 
en avoir le coeur nette on peut utiliser la commande `which` qui renvoie alors 
`time: shell reserved word`. Donc le `time` executer n'est pas une commande 
donc n'a pas de man associer.

## RAID 5

Si je fais un disque raid 5 avec des disque de taille 20go, 1go et 1go, quelle 
sera la taille final de mon raide ?

%

2go, car le raid se calque sur le min(20, 1, 1) et il y a un disque pour la
redondance ce qui fais 2go.

