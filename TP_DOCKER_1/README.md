3. Exécuter un serveur web (apache, nginx, ...) dans un container docker
    a. Récupérer l'image sur le docker hub

    Réponse : docker image pull nginx:latest

    b. Utiliser une commande pour vérifier que vous disposez bien de l'image en local

    Réponse : docker image ls

    c. Créer un fichier dans votre repo local ./html/index.html qui contient "Hello World"

    Réponse : Dossier html créé, fichier index.html crée qui contient <p> Hello world </p>


    d. Démarrer un nouveau container et servir la page html créée précédemment à l'aide d'un volume

    Réponse : docker run nginx 
              docker volume create tp
              docker run -v "${PWD}/html":/usr/share/nginx/html -d -p 4300:80 nginx  

    e. Supprimer le container

    Réponse : docker rm angry_rosalind --force  

    f. Relancez le même container sans le volume mais utilisez la commande cp pour servir votre fichier

    Réponse : docker cp ./html/index.html laughing_wilson:/usr/share/nginx/html 