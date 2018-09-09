# Boot2docker

- boot2docker ssh : lance la VM docker
- boot2docker ip: Permet de trouver l'IP de la machine virtuelle
- boot2docker stop: Arrête j'arrête docker
- repertoire persistant: /var/lib/boot2docker
- shell executé à chaque redémarrage : /var/lib/boot2docker/bootlocal.sh

# Docker

- --rm : supprime le conteneur lorsque l'on sort du run

docker ps -a : liste les conteneurs
se connecter avec un shell: docker exec -ti nomConteneur bash: 

# Sauvegarder les données

- dans la VM faire un partage de disque avec montage automatique 

