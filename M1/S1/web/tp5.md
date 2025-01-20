# TP5

## Reponse HTTP

Donner la structure d'une réponse à partir d'HTTP 1.0.

%

```
Version Status_Code Status_Text\r\n
Response_Header\r\n
\r\n
Ressource_Data
```

## Réponse HTTP

Quelle header permet de spécifier dans une réponse HTTP que la connection doit 
être close après ?

%

`Connection: close`

## HTTP

Rappelez comment s’effectue une redirection avec le protocole HTTP ?

%

Il s'agit d'un champs d'header donner en réponse par le serveur à une requête 
HTTP. Ces redirections sont prise automatiquement par les navigateurs, mais pas 
par les CGI. Exemple de réponse de redirection :

```CONNECT vcsa-dpi.dptinfo.univ-rouen.fr:443 HTTP/1.1
User-Agent: Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:131.0) Gecko/20100101 Firefox/131.0
Proxy-Connection: keep-alive
Connection: keep-alive
Host: vcsa-dpi.dptinfo.univ-rouen.fr:443


```

## HTTPS

Qu'est transmi en claire dans une requête HTTPS ?

%

Le champs `Host` car sinon, le serveur ne serait pas a qu'elle serveur virtuelle
faire transmettre la requette.

## Serveur Mandataire

Qu'est ce qu'un serveur mandataire ?

%

Un serveur mandataire, ou proxy, est un intermédiaire qui se place entre un 
client (par exemple, un navigateur web) et un serveur cible (par exemple, un 
site web). Il reçoit les requêtes du client, les transmet au serveur cible, 
puis retourne la réponse du serveur au client.