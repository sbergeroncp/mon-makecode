# atelier_3_dec_f

# Transforme ton micro:bit en veilleuse. (Microbit seulement)

## @showdialog 

Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs. 

Sébastien Bergeron - Conseiller pédagogique 

Journée du numérique du 3 décembre 2021

## @showdialog 

Transforme ton micro:bit en veilleuse.
 
![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_c_7.jpg?raw=true) 

## Étape 1 

Supprime le bloc ``|| basic:au démarrage ||``. 


## @showdialog 

Ajoute une commande lorsque le micro:bit est activé. 

## Étape 2 

 Ajoute le bloc ``|| logic: "Si alors sinon"  ||`` dans le bloc ``|| basic:Toujours ||``. 
 

```blocks 

basic.forever(function () {
    if (true) {
    	
    } else {
    	
    }
})

``` 

## @showdialog 

Ajoute une condition à la séquence de programmation.   

## Étape 3 
 
Ajoute le bloc ``|| input: niveau d'intensité lumineuse  ||`` dans le bloc ``|| logic:"0 < 0"||``. 
 
Modifie la valeur de droite ``|| logic:"0 < 0"||`` à 40.

Autrement dit, "si l'intensité de lumière est inférieure à "40"... un événement doit de produire.
 
```blocks 

basic.forever(function () {
    if (input.lightLevel() < 40) {
    	
    } else {
    	
    }
})

``` 

## @showdialog 

Ajoute la condition "si".   

## Étape 4 
 
Ajoute le bloc ``|| pins: Écrire sur la broche  ||`` sous la condition ``|| logic: "Si alors sinon"  ||``. 
 
Modifie les valeurs du bloc ``|| pins: Écrire sur la broche  ||``.

Écrire sur la broche "P0" la valeur "1".

 
```blocks 

basic.forever(function () {
    if (input.lightLevel() < 40) {
        pins.digitalWritePin(DigitalPin.P0, 1)
    } else {
    	
    }
})

``` 

## @showdialog 

Ajoute la condition "sinon".   

## Étape 6 
 
Ajoute le bloc ``|| pins: Écrire sur la broche  ||`` sous la condition ``|| logic: "Si alors sinon"  ||``. 
 
Modifie les valeurs du bloc ``|| pins: Écrire sur la broche  ||``.

Écrire sur la broche "P0" la valeur "0".

 
```blocks 

basic.forever(function () {
    if (input.lightLevel() < 40) {
        pins.digitalWritePin(DigitalPin.P0, 1)
    } else {
        pins.digitalWritePin(DigitalPin.P0, 0)
    }
})

``` 

## @showdialog 

Félicitations! Tu as terminé de programmer ta veilleuse numérique! 

Ensuite, appuie sur le bouton "Télécharger" pour accéder à l'application MakeCode/Micro:bit.

