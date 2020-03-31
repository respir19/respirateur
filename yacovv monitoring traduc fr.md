# YACoVV Monitoring

 

La ventilation peut entraîner une multitude de problèmes qui doivent être détectés rapidement.

 

## Considérations

 

- La surveillance doit être indépendante du contrôle de la ventilation.

- L'atteinte de la pression de ventilation doit être détectée.

- Le maintien de la PEEP doit être surveillé

- Affichage des erreurs via des signaux acoustiques et optiques

 

## Implémentation

 

Dans une première approche, nous avons testé une mesure capacitive sur plusieurs hauteurs au niveau de la colonne d'eau.

La technologie de mesure consiste en un câble isolé qui est guidé dans la colonne d'eau du manomètre, ainsi que d'autres câbles isolés qui sont enroulés sur le manomètre en U, autour de l'emplacement des valeurs de pression à détecter.

 

Cette technique de mesure peut être utilisée pour déterminer si la pression oscille entre la pression de ventilation et la PEEP au cours de chaque cycle de ventilation. Avec ces mesures, les erreurs suivantes dans le système peuvent être détectées:

- La pression de ventilation n'est pas atteinte. Exemples : fuite dans le tuyau vers le patient ou sur le chemin vers la valve de sortie, colonne d'eau pour la pression de ventilation mal réglée, perte de fluide dans le régulateur de pression

- La PEEP n'est pas atteinte. Exemples : fuites dans le tuyau de ventilation, fuites entre la soupape de sortie et la colonne d'eau du détendeur, perte de fluide dans le détendeur.

- Fréquence de ventilation: La fréquence de respiration peut être calculée à partir de la fréquence à l'oscilloscope (fréquence d'oscillation de la colonne d'eau du manomètre en U). Une alarme peut être déclenchée via des valeurs min et max dans la surveillance si la fréquence respiratoire est inférieure ou dépassée.

 

[Video avec détection de 2 valeurs de pression](https://youtu.be/_2SUDyStXJM)

 

Une mesure capacitive permettrait également de mesurer la hauteur absolue du liquide dans le manomètre en U, mais cela nécessiterait un étalonnage complexe du système. De plus, les points de mesure fixes peuvent être facilement déplacés sur le manomètre pour ajuster les valeurs. Si, par exemple, la pression de ventilation d'un patient doit être augmentée, il suffit de déplacer le point de mesure vers le haut.

 

## Affichage des erreurs

 

L'état du système peut être affiché de plusieurs manières.

 

### LED colorées

 

- rouge: défaut

- vert: la ventilation est stable

- jaune: il y a eu une erreur de ventilation, mais celle-ci a disparu d'elle-même. L'erreur peut être réinitialisée en appuyant sur un bouton.

Les LED vertes et jaunes peuvent également clignoter en même temps que la ventilation. Cela permet de reconnaître la fréquence même à une plus grande distance.

 

### Affichage

 

La fréquence respiratoire et une description plus précise d'une erreur peuvent être affichées sur un écran. L'affichage n'est pas un remplacement pour les LED mais un ajout.

 

### Alarme acoustique

 

Une alarme acoustique doit absolument être installée. Conjointement aux LED, un système défectueux peut [ainsi] être identifié rapidement et clairement, même avec un grand nombre d'appareils proches les uns des autres.

 

---------------

- fichier d'origine : https://github.com/auenkind/YACoVV/blob/master/MONITORING_DE.md
