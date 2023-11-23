- BACKEND (api 1): 
    - Créer une route + controller pour aller cher un article en fonction de l'id donné
        /:id

- FRONTEND : 
    - mettre en place les routes dynamiques pour afficher le détail d'un article (exemple /1 => ressort le détail de l'article qui a l'id 1) =:> fetcher les données en mode ISR
    - Sur la homepage : affecter les liens de chaque item de la grile
    - Sur le header : affecter les liens à chaque résultat de recherche

- REPLICATION DATA :
    - doc : https://github.com/redis/node-redis/blob/master/docs/pub-sub.md
    - Créer une image docker redis
        - Rajouter une configs avec l'ajout d'un mdp
    - Dans l'API (express) :
        - installer package "redis"
        - Se connecter à la base de données (container)
        - Créer un endpoint /replicate-data
        -  Ajouter un Controller et publier une channel  avec les données de la bdd sql
    - Dans l'API (Fastify)
        - Souscrire au channel pour insérer les données dans la base de données redis
        - Envoyer les données reçues dans le endpoint (/search)
            
        