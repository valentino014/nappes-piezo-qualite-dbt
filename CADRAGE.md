## Les 2 API 
Piézométrie 

API : https://hubeau.eaufrance.fr/api/v1/niveaux_nappes

Call : /chroniques_tr
Lister les chroniques piézométriques en temps réel


### Ensuite choix de la deuxième API

Qualité des nappes d'eau souterraine
Lien direct avec la piézométrie car on pourrait voir la qualité de l'eau par région en faisant un lien entre nappe (API piézométrie) et qualité (API Qualité des nappes d'eau souterraine)

API : https://hubeau.eaufrance.fr/api/v1/qualite_nappes

Call : /analyses
Lister les analyses

## LA question d'analyse

Y a-t-il un lien entre quantité d'eau dans la nappe phréatique et qualité ?


## L'utilisateur visé
Un hydrologue. À contacter

## Le bloc technique

Incrémental : à traiter
Dimension SCD2 : à traiter 
Ce que contient le runbook : à traiter 
Sur quoi porte l'alerte : trop de choix :(

candidates de clé métier : piézométrie colonnes bss_id OU code_bss OU urn_bss

## À traiter 

écarts de fréquence entre les deux sources : à traiter