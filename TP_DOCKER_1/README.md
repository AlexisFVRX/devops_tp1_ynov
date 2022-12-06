3. Exécuter un serveur web (apache, nginx, ...) dans un container docker
    a. Récupérer l'image sur le docker hub

    Réponse : docker image pull nginx:latest

    b. Utiliser une commande pour vérifier que vous disposez bien de l'image en local

    Réponse : docker image ls

    c. Créer un fichier dans votre repo local ./html/index.html qui contient "Hello World"
    d. Démarrer un nouveau container et servir la page html créée précédemment à l'aide d'un volume
    e. Supprimer le container
    f. Relancez le même container sans le volume mais utilisez la commande cp pour servir votre fichier