## Sources

### niveaux_nappes (piézométrie)
Endpoint : https://hubeau.eaufrance.fr/api/v1/niveaux_nappes/chroniques_tr

- **Fréquence réelle observée** : horaire. Prouvé sur 6 mesures consécutives du point `00035X0210/PZO1` — dates 2026-09-07T23:00Z à 2026-09-08T04:00Z, écart constant d'1 heure.
- **Granularité temporelle** : à prouver semaine 30
- **Clé** : `code_bss` = `00035X0210/PZO1` · `bss_id` = `BSS000ACKJ`
- **Champs obligatoires vs optionnels** : à prouver semaine 30
- **Valeurs de qualification** : à prouver semaine 30
- **Volumétrie sur le Var** : à prouver semaine 30

### qualite_nappes
Endpoint : https://hubeau.eaufrance.fr/api/v1/qualite_nappes/analyses

- **Fréquence réelle observée** : à prouver semaine 30
- **Granularité temporelle** : à prouver semaine 30 (champ `date_debut_prelevement` — chercher s'il existe une date de fin)
- **Clé** : à prouver semaine 30
- **Champs toujours null observés** : `limite_quantification`, `limite_detection`, `seuil_saturation`, `incertitude_analytique`
- **Valeurs de qualification** : `code_statut_analyse` = `2`, `nom_statut_analyse` = « Donnée contrôlée niveau 1 »
- **Volumétrie** : `count` = 951371 — périmètre non confirmé, appel probablement non filtré par département

### Clé de jointure

Le code BSS a-t-il la même forme dans les deux API ?
question ouverte : semaine 30

Un code présent d'un côté est-il toujours présent de l'autre ?
question ouverte : semaine 30

Un code peut-il désigner plusieurs points de mesure ?
question ouverte : semaine 30

Y a-t-il des renommages ou des codes historiques ?
question ouverte : semaine 30