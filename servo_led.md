# servo_led

# Un circuit électrique avec un servomoteur! 

## @showdialog 

Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs. 

Sébastien Bergeron - Conseiller pédagogique 

Journée du numérique du 3 décembre 2021

## @showdialog 

Transforme ton micro:bit en un circuit électrique avec un servomoteur et des lumières LED. 
 
![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_h_1.jpg?raw=true) 

## Étape 1 

Supprime le bloc  ``|| basic:toujours ||``. 

## @showdialog 

Ajoute une commande lorsque le micro:bit est activé. 

## Étape 2 

 Ajoute le bloc ``|| pins: écrire sur la broche P1  ||`` dans le bloc ``||basic:au démarrage||``. 
 
Modifie les valeurs du bloc ``|| pins: écrire sur la broche P1 la valeur 1  ||``.

Ajoute le bloc ``|| pins: écrire sur la broche P2  ||`` dans le bloc ``||basic:au démarrage||``. 
 
Modifie les valeurs du bloc ``|| pins: écrire sur la broche P2 la valeur 0  ||``.
 
```blocks 
pins.digitalWritePin(DigitalPin.P1, 1)
pins.digitalWritePin(DigitalPin.P2, 0)

``` 

## @showdialog 

Ajoute une commande lorsque le bouton A est pressé. 

## Étape 3 

 Ajoute le bloc ``|| pins: régler position servo  ||`` dans le bloc ``||input:lorsque le bouton A est pressé||``. 
 
Modifie les valeurs du bloc ``|| pins: régler position servo  ||``.

Inscris à "90" degrés.
 
```blocks 

input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 90)
})

``` 

## @showdialog 

Ajoute une autre commande lorsque le bouton A est pressé.   

## Étape 4

Ajoute le bloc ``|| pins: écrire sur la broche P1  ||`` dans le bloc ``||input:lorsque le bouton A est pressé||``. 
 
Ajoute le bloc ``|| pins: écrire sur la broche P2  ||`` dans le bloc ``||input:lorsque le bouton A est pressé||``.

Ajoute le bloc ``|| basic: pause (ms) 500  ||`` dans le bloc ``||input:lorsque le bouton A est pressé||``.

Modifie les valeurs du bloc ``|| pins: écrire sur la broche "P1" la valeur "0"  ||``.

Modifie les valeurs du bloc ``|| pins: écrire sur la broche "P2" la valeur "1"  ||``.

```blocks

input.onButtonPressed(Button.A, function () {
    pins.servoWritePin(AnalogPin.P0, 90)
    pins.digitalWritePin(DigitalPin.P1, 0)
    basic.pause(500)
    pins.digitalWritePin(DigitalPin.P2, 1)
})

```

## @showdialog 

Ajoute une commande lorsque le bouton B est pressé. 

## Étape 5 

 Ajoute le bloc ``|| pins: régler position servo  ||`` dans le bloc ``||input:lorsque le bouton B est pressé||``. 
 
Modifie les valeurs du bloc ``|| pins: régler position servo  ||``.

Inscris à "0" degrés.
 
```blocks 

input.onButtonPressed(Button.B, function () {
    pins.servoWritePin(AnalogPin.P0, 0)
})

``` 

## @showdialog 

Ajoute une autre commande lorsque le bouton A est pressé.   

## Étape 6

Ajoute le bloc ``|| pins: écrire sur la broche P1  ||`` dans le bloc ``||input:lorsque le bouton B est pressé||``. 
 
Ajoute le bloc ``|| pins: écrire sur la broche P2  ||`` dans le bloc ``||input:lorsque le bouton B est pressé||``.

Ajoute le bloc ``|| basic: pause (ms) 500  ||`` dans le bloc ``||input:lorsque le bouton B est pressé||``.

Modifie les valeurs du bloc ``|| pins: écrire sur la broche "P1" la valeur "1"  ||``.

Modifie les valeurs du bloc ``|| pins: écrire sur la broche "P2" la valeur "0"  ||``.

```blocks

input.onButtonPressed(Button.B, function () {
    pins.servoWritePin(AnalogPin.P0, 0)
    pins.digitalWritePin(DigitalPin.P2, 0)
    basic.pause(500)
    pins.digitalWritePin(DigitalPin.P1, 1)
})

```

## @showdialog 

Félicitations! Tu as terminé de programmer ton circuit! 

Ensuite, appuie sur le bouton "Télécharger" pour accéder à l'application MakeCode/Micro:bit.

Construis un support pour le servomoteur et un support pour les lumières LED.

Une fois terminé, teste la programmation.

