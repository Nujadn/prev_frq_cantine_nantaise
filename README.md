# Prédire la fréquentation des cantines scolaires nantaises

## Contexte

C'est un projet personnel qui a été réalisé dans le cadre de la formation "Développeur/se en Intelligence Artificielle de Simplon-Microsoft. Il s'agit d'un appel de projet de la Métropole de Nantes afin de prédire le nombre de repas à servir dans les cantines scolaires. Avec pour objectif d'ajuster la production de la cantine centrale pour réduire le gaspillage alimentaire et de réduire les dépenses sur les matières premières. 

Dans le schéma ci-dessous, on peut observer le processus actuel de leur organisation actuelle pour le service de repas dans les cantines. Il s’agit d’un processus qui remonte à 1 mois avant de servir les repas le jour J.

![image](https://github.com/Nujadn/prev_frq_cantine_nantaise/assets/142103183/47a5973c-af42-4aef-9436-e6844d37f52e)

L’organisation des repas scolaires se fait dans une suite chronologique d’évènements suivant :
- constitution des menus ; 
- commandes des matières premières auprès des fournisseurs ;
- réception des ingrédients auprès de chaque fournisseur ;
- constitution des repas ;
- envois des repas dans chaque établissement ;
- si les repas sont insuffisants, la cantine fera une demande à la cuisine centrale pour récupérer plus de repas.


## Besoin du client

![image](https://github.com/Nujadn/prev_frq_cantine_nantaise/assets/142103183/7df948d4-cc41-4245-94ae-c3433724b14b)

L'objectif du projet est de mettre un outil à la disposition des agents de restauration de chaque école pour qu'ils puissent prédire la fréquentation des élèves à leur cantine. Ensuite ils transmettront leur estimation du nombre de repas à servir à la cantine centrale.
La cuisine centrale livre tous les jours entre 12 000 et 15 000 repas à environ 87 cantines scolaires sur la métropole nantaise. Ils ont pour objectif de réduire le gaspillage alimentaire mais sans faire de prévisions "trop-juste". En effet, des prévisions trop justes impliquerait que des enfants n’aient pas à manger certains midi. 

La problématique principale est de prédire 3 semaines à l'avance les repas. Ces prédictions sont journalières et se font en fonction des menus.

Pour remplir cet objectif, ils ont récolté et constitué un dataset allant de 2011 à 2019 sous format .csv. Ce dataset est disponible sur leur site et contient des informations sur la date et la constitution du repas.

A l’heure actuel, ils ont un gaspillage d’environ 1 250 repas par jour. Ils avaient en moyenne 5 % de gâchis alimentaire entre 2011 à 2016, puis en moyenne 8 % entre 2017 à 2019. 


