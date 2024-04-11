Deux clé à configurer:
    - Première clé pour la base de données comme demandé sur le point bonus:

        kubectl create secret generic mongodb-password --from-literal=password=admin

    - Seconde clé pour accéder aux image de mon repo privé DockerHub:

        kubectl create secret docker-registry myregistrykey \
        --docker-server=https://index.docker.io/v1/ \
        --docker-username=sadademba \
        --docker-password=dckr_pat_jE3AH3VNIz3agZAF1KhG2aA0nhQ \
        --docker-email=sadadembat9@gmail.com
