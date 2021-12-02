# atelier_3_dec_e

# Transforme ton micro:bit en thermomètre.

## @showdialog 

Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs. 

Sébastien Bergeron - Conseiller pédagogique 

Journée du numérique du 3 décembre 2021

## @showdialog 

Transforme ton micro:bit thermomètre.
 
![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_c_7.jpg?raw=true) 

## Étape 1 

Supprime le bloc ``|| basic:au démarrage ||``. 


## @showdialog 

Ajoute une commande lorsque le micro:bit est activé. 

## Étape 2 

 Ajoute le bloc ``|| input:température  ||`` dans le bloc ``|| basic:montrer un nombre ||``.

 Ajoute cette nouvelle séquence dans le bloc ``|| basic:toujours ||``.


```blocks 

basic.forever(function () {
    basic.showNumber(input.temperature())
    
})

``` 

## @showdialog 

Ajoute une autre commande lorsque le micro:bit est activé. 

## Étape 3 

 Ajoute le bloc ``|| basic:pause ms (500)  ||`` et le bloc ``|| basic:effacer l'écran ||`` dans le bloc ``|| basic:toujours ||``.

 
```blocks 

basic.forever(function () {
    basic.showNumber(input.temperature())
    basic.pause(500)
    basic.clearScreen()
})

``` 

## @showdialog 

Ajoute une condition à la séquence de programmation.   

## Étape 4 
 
Ajoute le bloc ``|| input: température  ||`` dans le bloc ``|| logic:"0 >= 0"||``. 
 
Modifie la valeur de droite ``|| logic:"0 >= 0"||`` à 30.

Autrement dit, "si la température est supérieure ou égale à "30"... un événement doit de produire.
 
```blocks 

basic.forever(function () {
    basic.showNumber(input.temperature())
    basic.pause(500)
    basic.clearScreen()
    if (input.temperature() >= 30) {
    	
    } else {
    	
    }
})

``` 

## @showdialog 

Ajoute la condition "si".   

## Étape 4 
 
Ajoute le bloc ``|| basic: afficher l'icône  ||`` sous la condition ``|| logic: "si alors sinon"  ||``. 
 
Sélectionne l'icône du t-shirt.

 ```blocks 

basic.forever(function () {
    basic.showNumber(input.temperature())
    basic.pause(500)
    basic.clearScreen()
    if (input.temperature() >= 30) {
        basic.showIcon(IconNames.TShirt)
    } else {
    	
    }
})

``` 

## @showdialog 

Ajoute la condition "sinon".   

## Étape 6 
 
Ajoute le bloc ``|| basic: afficher l'icône  ||`` sous la condition ``|| logic: "si alors sinon"  ||``. 
 
Sélectionne l'icône du parapluie.

 
```blocks 

basic.forever(function () {
    basic.showNumber(input.temperature())
    basic.pause(500)
    basic.clearScreen()
    if (input.temperature() >= 30) {
        basic.showIcon(IconNames.TShirt)
    } else {
        basic.showIcon(IconNames.Umbrella)
    }
})

``` 

## @showdialog 

Félicitations! Tu as terminé de programmer ton thermomètre numérique! 

Ensuite, appuie sur le bouton "Télécharger" pour accéder à l'application MakeCode/Micro:bit.

Prends le micro:bit dans tes mains. Qu'observes-tu?

Teste ton programme!