# docker
Le but de ce projet est que je monte en compétences sur Docker.


### Voici les commandes à suivre pour télécharger une image Docker depuis GitHub Packages et la lancer sur une machine :
1. Assurez-vous que Docker est installé sur votre machine.
2. Connectez-vous à GitHub Packages en utilisant la commande suivante :

```
docker login https://docker.pkg.github.com -u USERNAME -p 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
```
Remplacez `USERNAME` par votre nom d'utilisateur GitHub.
3. Téléchargez l'image Docker en utilisant la commande suivante :
```
docker pull ghcr.io/alexandre-daumail/docker:0.0.1
```
4. Lancez le conteneur Docker en utilisant la commande suivante :
```
docker run -p HOST_PORT:CONTAINER_PORT -d docker
```
Remplacez `HOST_PORT` par le port de votre machine que vous souhaitez associer au port du conteneur `CONTAINER_PORT` (ex: 80:80)

Voilà, votre image Docker est téléchargée et en cours d'exécution sur votre machine.

Vous pouvez tester la bonne résolution de ces opérations en vous rendant à l’adresse localhost:80/deprecated.php sur votre navigateur internet.
