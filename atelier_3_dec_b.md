# atelier_3_dec_b

# Une lampe de poche numérique!

## @showdialog 

Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs. 

Sébastien Bergeron - Conseiller pédagogique 

Journée du numérique du 3 décembre 2021

## @showdialog 

Transforme ton micro:bit en lampe de poche numérique! 
 
![CSSBF](https://pxt.azureedge.net/blob/3d8dede227b23aeefbdf98d433f3be87dca060ea/static/mb/projects/name-badge/header.png) 

## Étape 1 

Supprime les blocs ``|| basic:au démarrage ||`` ``|| basic:toujours ||``. 


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
