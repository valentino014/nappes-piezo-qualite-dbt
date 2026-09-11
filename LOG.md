Produit : entrée DECISIONS.md « spec MetricFlow », section Sources de CONTRAT.md, fréquence piézométrie prouvée
Décidé : Projet 3 sur la spec YAML récente, Projet 2 laissé tel quel
Appris : une fréquence se prouve sur un écart entre deux dates du même point, jamais sur une date seule
Garé : format du contrat à reprendre en puces, appels à refiltrer sur le Var


## J186 · jeudi 10/09 · INFRA

- **Produit** : infra Snowflake complète du Projet 3 (rôle TRANSFORMHUBEAU, database DATABASE_HUBEAU, 7 schémas, warehouse WH_HUBEAU XS, resource monitor RM_HUBEAU, grants, stage, file format) · auto-suspend de COMPUTE_WH ramené de 300 s à 60 s · .gitignore complété
- **Décidé** : monitor de portée warehouse (RM_HUBEAU sur WH_HUBEAU) plutôt qu'au niveau du compte · quota 10 crédits/mois, SUSPEND à 100 %
- **Appris** : un resource monitor ne réserve rien, il compte les crédits et déclenche une action à un seuil — la puissance vient de la taille du warehouse · un « Authorization Hold » relâché est une pré-autorisation de carte, pas une facture
- **Garé** : utilisateur de service CI · option dbt de compatibilité v2 introuvable · changement possible de la question d'analyse

### État des 6 lignes
1. COMPUTE_WH — **cochée** : RM_AGRIBALYSE déjà attaché, auto-suspend passé à 60 s
2. Le 20 € — **cochée** : Authorization Hold → Released, pré-autorisation de carte, aucun prélèvement
3. Utilisateur de service CI — **parkée** : la CI tourne aujourd'hui avec mon compte personnel, pas un compte TYPE = SERVICE
4. Sécurité des clés — **cochée** : `git log --all -- '*.p8'` vide, `*.p8` et `*.pem` ajoutés au .gitignore
5. Branche feat/semaine-27-docs — **cochée** : inexistante, dépôt agribalyse sur main
6. dbt parse v2 — **parkée** : l'option `--use-v2-parser` n'existe pas sur ma version de dbt Core