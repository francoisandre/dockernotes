# Boot2docker

- boot2docker start puis boot2docker ssh : lance la VM docker et s'y connecte
- boot2docker ip: Permet de trouver l'IP de la machine virtuelle
- boot2docker stop: Arrête j'arrête docker
- repertoire persistant: /var/lib/boot2docker
- shell executé à chaque redémarrage : /var/lib/boot2docker/bootlocal.sh

# Docker

- --rm : supprime le conteneur lorsque l'on sort du run

docker ps -a : liste les conteneurs
se connecter avec un shell: docker exec -ti nomConteneur bash: 

# Compose

## Installation

- Récupérer le binaire via curl
- Copier le fichier dans /var/lib/boot2docker
- Dans /var/lib/boot2docker/bootlocal.sh rajouter les lignes suivantes afin de positionner le binaire à l'endroit voulu à chaque redemarrage

<code>
  cp /var/lib/boot2docker/docker-compose /usr/local/bin/docker-compose
  
  chmod +x /usr/local/bin/docker-compose                              
</code>

## Utilisation

docker-compose up (dans le rep contenant docker-compose.yml)

# Sauvegarder les données

- dans la VM faire un partage de disque avec montage automatique 

