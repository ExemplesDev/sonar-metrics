# Pré-requis

* PC sous windows 64 bits
* Répertoire de travail avec droits d'écriture et d'exécution
* Acces en lecture de projet(s) d'un serveur sonarQube

# Installation

- télécharger l'archive _exe.win-amd64-3.6.7z_ et le fichier _config.json_
- la décompresser dans un répertoire de travail
- remplir les champs de connexion d'accès au serveur sonarQube, en éditant le fichier _config.json_

```
{
     "sonar":
    {
      "url" : "https://path-to-sonarQubeServer",
      "username" : "sonar-username",
       "private_token": "sonar-token",
       "password" : "sonar-password"
     }
}
```
- ouvrir une console dans ce répertoire
- lancer cette commande 

`> sonar-metrics.exe --show_sonar_version`

la version du serveur devrait s'afficher comme suit:
```
> C:\Users\dom\AppData\Local\Programs\Python\Python36\build\exe.win-amd64-3.6>sonar-metrics.exe --show_sonar_version

> sonarQube server version: 5.6.7 (status: UP)

```
