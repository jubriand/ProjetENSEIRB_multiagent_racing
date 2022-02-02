# IA pour les jeux vidéos
Julien Briand

Pour faire évoluer le programme j'ai décidé de me concentrer sur la gestion de collisions et la création de safety cars/ambulances. 

### Collisions
Les voitures se crash lorsqu'elles se rentrent dedans, leurs vitesses devient nulle et pour avoir un visuel nous passons la culeur de rouge à bleue. Celles-ci sont donc présentent sur le circuit. Leur status est traduit par un booléen _collision. / Une fois accidentées, les voitures sont arretées sur le circuit et elles créent un carambolange lorsque les autres voitures rentrent dedans.

### Ambulance
Intervient alors la sous-classe de véhicule: les ambulances. Elles se difféerncient des autres par leurs tailles plus imposantes, leur couleur verte, leur vitesse plus faible et la présence d'un halo autour d'elle représentant la zone de soin. Lorsqu'une voiture rentre dans ce halo, elle peut repartir. Une ambulance ne peut pas avoir d'accident et les voitures ne peuvent techniuement pas avoir d'accident avec les ambulances puisqu'elles sont dans le halo de soin.\
Le halo de soin fais ralentir les véhicules à la même allure que les ambulances. Lorsqu'une ambualnce soigne elle devient jaune en guise de témoin et les véhicules dans le cercle aussi.

### Améliorations possibles
Une voiture pourrait ralentir voire s'arreter devant un accident pour éviter de l'agrandir et créer un carambolage.

<img src="./pictures/beforeAcc.png">
<img src="./pictures/afterAcc.png">
![plot](./pictures/beforeAcc.png)