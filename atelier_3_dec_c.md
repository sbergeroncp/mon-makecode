# atelier_3_dec_c

# Un circuit électrique avec un servomoteur! 

## @showdialog 

Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs. 

Sébastien Bergeron - Conseiller pédagogique 

Journée du numérique du 3 décembre 2021

## @showdialog 

Transforme ton micro:bit en un circuit électrique avec un servomoteur! 
 
![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_b_7.jpg?raw=true) 

## Étape 1 

Supprime les blocs ``|| basic:au démarrage ||`` et ``|| basic:toujours ||``. 


## @showdialog 

Ajoute une commande lorsque le bouton A est pressé. 

## Étape 2 

 Ajoute le bloc ``|| pins: régler position servo  ||`` dans le bloc ``||input:lorsque le bouton A est pressé||``. 
 
Modifie les valeurs du bloc ``|| pins: régler position servo  ||``.

Inscris à "45" degrés.
 

```blocks 

input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 45)
})

``` 

## @showdialog 

Ajoute une commande lorsque le bouton B est pressé.   

## Étape 3 
 
Ajoute le bloc ``|| pins: régler position servo  ||`` dans le bloc ``||input:lorsque le bouton B est pressé||``. 
 
Modifie les valeurs du bloc ``|| pins: régler position servo  ||``.

Inscris à "90" degrés.
 

```blocks 

input.onButtonPressed(Button.B, function () {
    pins.servoWritePin(AnalogPin.P0, 90)
})

``` 

## @showdialog 

Ajoute une commande lorsque le bouton B est pressé.   

## Étape 4 
 
Ajoute le bloc ``|| pins: régler position servo  ||`` dans le bloc ``||input:lorsque le bouton A+B est pressé||``. 
 
Modifie les valeurs du bloc ``|| pins: régler position servo  ||``.

Inscris à "0" degrés.
 

```blocks 

input.onButtonPressed(Button.AB, function () {
    pins.servoWritePin(AnalogPin.P0, 0)
})

``` 

## @showdialog 

Félicitations! Tu as terminé de programmer ton circuit! 

Ensuite, appuie sur le bouton "Télécharger" pour accéder à l'application MakeCode/Micro:bit.

## @showdialog 

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_b_1.jpg?raw=true) 

Branche une pince alligator dans le port "P0" du micro:bit.

## @showdialog 

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_b_2.jpg?raw=true) 

Branche une pince alligator dans le port "3V" du micro:bit.

## @showdialog 

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_b_3.jpg?raw=true) 

Branche une pince alligator dans le port "GND" du micro:bit.


Félicitations! Tu as terminé ton premier circuit électrique et numérique.

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_c_6.jpg?raw=true) 

Teste maintenant ton circuit!