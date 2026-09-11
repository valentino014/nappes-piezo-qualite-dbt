- J184 — le découpage était faux : le tableau à deux colonnes est illisible à remplir. Reprendre en une liste à puces par source, une source à la fois.
- J184 — appel piézométrie non filtré sur le Var (coordonnées relevées : Pas-de-Calais). Refaire les appels avec le paramètre de département avant toute volumétrie.


- J186 — Utilisateur de service CI : la CI Agribalyse se connecte avec mon compte personnel ONIZUKA01. Créer SVC_CI_HUBEAU avec TYPE = SERVICE, clé publique RSA, DEFAULT_ROLE = TRANSFORMHUBEAU, aucun mot de passe, puis basculer le secret GitHub.
- J186 — Compatibilité dbt v2 du Projet 2 : `dbt parse --use-v2-parser` renvoie « No such option ». Relever la version exacte (`dbt --version`), lire `dbt parse -h` en entier, et écrire le constat dans le README d'agribalyse. Pas de migration.
- J186 — Portée du resource monitor : RM_HUBEAU ne couvre que WH_HUBEAU. Décider si un monitor de compte est nécessaire une fois le Projet 3 en Phase 2.
- J186 — Nombre de schémas : 4 schémas CI créés (CI, CI_STAGING, CI_INTERMEDIATE, CI_MARTS) avant que le grain soit tranché. Rediscuter en Phase 2 si un schéma CI unique suffit.
- J185 — Question d'analyse du Projet 3 : envisager de la changer (évolution des nappes, autre API). À trancher en entrée DECISIONS.md, pas en passant. Vérifier d'abord si la nouvelle version garde deux sources à réconcilier et l'écart de fréquence.
- J185 — Réseau : message à une personne nommée (Les Olivades, ou hydrologue BRGM PACA / Agence de l'eau RMC / CEREGE) — reporté à la semaine du 14/09.
- J185 — Meetup data PACA : une date à mettre dans l'agenda, non trouvée dans les 15 min.