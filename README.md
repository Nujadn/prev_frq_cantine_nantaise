# Prédire la fréquentation des cantines scolaires nantaises

## Contexte

C'est un projet personnel qui a été réalisé dans le cadre de la formation "Développeur/se en Intelligence Artificielle de Simplon-Microsoft. Il s'agit d'un appel de projet de la Métropôle de Nantes afin de prédire le nombre de repas à servir dans les cantines scolaires. Avec pour objectif d'ajuster la production de la cantine centrale pour réduire le gaspillage alimentaire et de réduire les dépenses sur les matières premières. 

Dans le schéma ci-dessous, on peut observer le processus actuel de leur organisation actuelle pour le service de repas dans les cantines Il s’agit d’un processus qui remonte à 1 mois avant de servir les repas le jour J.

![image](https://github.com/Nujadn/prev_frq_cantine_nantaise/assets/142103183/94a6c479-7d69-43ac-8969-f5b02ee7b41a)


## Besoin du client

Le projet est de prédire la fréquentation des cantines pour que les agents puissent transmettre leurs besoins à la cantine centrale et que cette dernière puisse anticiper correctement. C’est un organisme qui livre à environ 87 cantines scolaires sur la métropole nantaise tous les jours. Ils ont pour objectif de réduire le gaspillage alimentaire sans faire de prévisions "trop-juste" car il n’est pas acceptable que des élèves n’aient pas à manger le midi. Pour remplir leur objectif ils ont lancé un appel à projet après avoir récolté et constitué un dataset de 2011 à 2019 sous format .csv disponible sur leur site, avec la date et le détail des menus. 

L’objectif est d’avoir des prévisions journalières en fonction des menus pour qu’ensuite ils puissent préparer la quantité de repas adaptée à chaque école. En sachant que les élèves sont inscrits le matin pour manger à la cantine le midi ce qui génère de forte variabilité. Et que les cantines sont contraintes d’estimer 3 semaines à l’avance le nombre de personnes à manger à la cantine afin d’évaluer les quantités à commander aux fournisseurs. 

A l’heure actuel, ils ont un gaspillage d’environ 1 250 repas par jour. Ils avaient en moyenne 5 % de gâchis alimentaire entre 2011 à 2016, puis en moyenne 8 % entre 2017 à 2019. 

L’organisation des repas scolaires se fait dans une suite chronologique d’évènements suivant : 
— constitution des menus ; 
— commandes des ingrédients auprès des fournisseurs ; 
— réception des ingrédients auprès de chaque fournisseur ; 
— constitution des repas ; 
— envois des repas dans chaque établissement ; 
— si les repas sont insuffisants, la cantine fera une demande à la cantine centrale pour récupérer plus de repas. 

La problématique principale est de prédire le nombre de repas à servir par jour afin de réduire le gaspillage alimentaire sans pour autant avoir des prévisions trop justes et ne pas pouvoir servir de repas aux élèves. 

La problématique secondaire est de fournir une application pour que les utilisateurs puissent utiliser le modèle pour constituer les commandes auprès des fournisseurs. Il faut donc un outil facile d’utilisation et de compréhension pour que les utilisateurs l’utilisent. L’application devra permettre de réaliser des prédictions journalières pour au global pour les commandes et au détail pour chaque cantine scolaire. 


