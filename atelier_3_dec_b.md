# atelier_3_dec_b

# Un circuit électrique et numérique! 

## @showdialog 

Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs. 

Sébastien Bergeron - Conseiller pédagogique 

Journée du numérique du 3 décembre 2021

## @showdialog 

Transforme ton micro:bit en un circuit électrique et numérique! 
 
![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_a_5.jpg?raw=true) 

## Étape 1 

Supprime les blocs ``|| basic:au démarrage ||`` et ``|| basic:toujours ||``. 


## @showdialog 

Ajoute une commande lorsque le bouton A est pressé. 

## Étape 2 

 Ajoute le bloc ``|| pins: Écrire sur la broche  ||`` dans le bloc ``||input:lorsque le bouton A est pressé||``. 
 
Modifie les valeurs du bloc ``|| pins: Écrire sur la broche  ||``.

Remplace la valeur sur la broche "P0" par "1".
 

```blocks 

input.onButtonPressed(Button.A, function () {
    pins.digitalWritePin(DigitalPin.P0, 1)
})

``` 

## @showdialog 

Ajoute une commande lorsque le bouton B est pressé.   

## Étape 3 
 
Ajoute le bloc ``|| pins: Écrire sur la broche  ||`` dans le bloc ``||input:lorsque le bouton B est pressé||``. 
 
Modifie les valeurs du bloc ``|| pins: Écrire sur la broche  ||``.

Remplace la valeur sur la broche "P0" par "0".
 
```blocks 

input.onButtonPressed(Button.B, function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
})

``` 

## @showdialog 

Félicitations! Tu as terminé de programmer ton circuit! 

Ensuite, appuie sur le bouton "Télécharger" pour accéder à l'application MakeCode/Micro:bit.

## @showdialog 

Branche une pince alligator au port "P0" du micro:bit.

La couleur n'a pas d'importance!

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_a_1.jpg?raw=true) 

## @showdialog 

Relis la même pince alligator à une lumière LED à la broche positive. Il s'agit de la plus longue.

La couleur n'a pas d'importance!

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_a_2.jpg?raw=true) 

## @showdialog 

Branche une autre pince alligator dans le port "GND" du micro:bit. 

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_a_3.jpg?raw=true) 

## @showdialog 

Relis la même pince alligator de la lumière LED à la broche négative. Il s'agit de la plus petite.

Attention, les deux broches ne doivent pas se toucher!

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_a_4.jpg?raw=true) 

## @showdialog 

Félicitations! Tu as terminé ton premier circuit électrique et numérique.

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_a_5.jpg?raw=true) 

Teste maintenant ton circuit!