- Severless fonction 
    -> Utilisation Sam Aws 
    -> use case : 
        - Créer formulaire de newsletter (champs email)
        - Soumission de ce formulaire appel une serverless function
            -> Brevo : newsletter 
            -> clefs API + doc 
        - Insérer l'email dans liste de diffusion Brevo

- Frontend :
    - Routes uniques pour chaque article de blog 
        -> param router /:id
        -> param router = /:slug (string de caractère unique = "my-best-cloud-solutions")
        -> adapter sur ces pages la solution de render (pas de csr)

- Travailler une autre base de données 
    - NoSql -> sql (inversement)
    - Base de données est allouée au service de recherche (api-search)
    - Mettre en place un sytème de syncronisation entre les 2 bdds
    -> Data replication

