## Sources

### niveaux_nappes (piézométrie)
Endpoint : https://hubeau.eaufrance.fr/api/v1/niveaux_nappes/chroniques_tr

- **Fréquence réelle observée** : horaire. Prouvé sur 6 mesures consécutives du point `00035X0210/PZO1` — dates 2026-09-07T23:00Z à 2026-09-08T04:00Z, écart constant d'1 heure.
- **Granularité temporelle** : à prouver J187
- **Clé** : `code_bss` = `00035X0210/PZO1` · `bss_id` = `BSS000ACKJ`
- **Champs obligatoires vs optionnels** : à prouver J187
- **Valeurs de qualification** : à prouver J187
- **Volumétrie sur le Var** : à prouver J187

### qualite_nappes
Endpoint : https://hubeau.eaufrance.fr/api/v1/qualite_nappes/analyses

- **Fréquence réelle observée** : à prouver J187
- **Granularité temporelle** : à prouver J187 (champ `date_debut_prelevement` — chercher s'il existe une date de fin)
- **Clé** : à prouver J187
- **Champs toujours null observés** : `limite_quantification`, `limite_detection`, `seuil_saturation`, `incertitude_analytique`
- **Valeurs de qualification** : `code_statut_analyse` = `2`, `nom_statut_analyse` = « Donnée contrôlée niveau 1 »
- **Volumétrie** : `count` = 951371 — périmètre non confirmé, appel probablement non filtré par département