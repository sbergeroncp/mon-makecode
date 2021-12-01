# atelier_3_dec_d

# Transforme ton micro:bit en veilleuse.

## @showdialog 

Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs. 

Sébastien Bergeron - Conseiller pédagogique 

Journée du numérique du 3 décembre 2021

## @showdialog 

Transforme ton micro:bit veilleuse.
 
![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_c_7.jpg?raw=true) 

## Étape 1 

Supprime le bloc ``|| basic:au démarrage ||``. 


## @showdialog 

Ajoute une commande lorsque le bouton A est pressé. 

## Étape 2 

 Ajoute le bloc ``|| pins: Écrire sur la broche  ||`` dans le bloc ``||input:lorsque le bouton A est pressé||``. 
 
Modifie les valeurs du bloc ``|| pins: Écrire sur la broche  ||``.

Écrire sur la broche "P0" la valeur "1".
 

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

Écrire sur la broche "P0" la valeur "0".
 
```blocks 

input.onButtonPressed(Button.B, function () {
    pins.digitalWritePin(DigitalPin.P0, 0)
})

``` 

## @showdialog 

Félicitations! Tu as terminé de programmer ton premier circuit électrique! 

Ensuite, appuie sur le bouton "Télécharger" pour accéder à l'application MakeCode/Micro:bit.

## @showdialog 

Insère le micro:bit dans le bouclier.

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_c_1.jpg?raw=true) 

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_c_2.jpg?raw=true) 

## @showdialog 

Branche la lumière LED dans le bouclier dans le port "P0".

Assure-toi de brancher la lumière LED dans le bon sens.

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_c_3.jpg?raw=true) 

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_c_4.jpg?raw=true) 

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_c_5.jpg?raw=true) 

## @showdialog 

Félicitations! Tu as terminé ton premier circuit électrique.

Teste maintenant le circuit électrique.

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_c_6.jpg?raw=true)  