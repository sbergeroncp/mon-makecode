# atelier_3_dec_a
# Un porte-nom numérique!

## @showdialog 

Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs. 

Sébastien Bergeron - Conseiller pédagogique 

Journée du numérique du 3 décembre 2021

## @showdialog 

Transforme un porte-nom ordinaire en un porte-nom numérique! 
 
![CSSBF](https://pxt.azureedge.net/blob/3d8dede227b23aeefbdf98d433f3be87dca060ea/static/mb/projects/name-badge/header.png) 

## Étape 1 

Supprime le bloc ``|| basic:au démarrage ||``. 


## @showdialog 

Ajoute une commande lorsque le micro:bit est activé. 

## Étape 2 

 
Ajoute le bloc ``|| basic: montrer LEDs ||`` ou le bloc ``|| basic: montrer l'icône ||`` dans le bloc ``||basic:toujours||``. 

 Dessine un symbole dans le bloc ``|| basic: montrer LEDs ||`` au besoin. 
 
```blocks 

basic.forever(function () {
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
})

basic.forever(function () {
    basic.showIcon(IconNames.Heart)
})

``` 

## @showdialog 

Ajoute une commande lorsque le bouton A est pressé.   


## Étape 3 

 
Ajoute le bloc ``|| basic: afficher le texte "Hello!" ||`` dans le bloc ``||input:lorsque le bouton A est pressé||``. 
 

Modifie le bloc ``|| basic: Afficher texte ||`` et écris ton prénom. 
 

```blocks 

input.onButtonPressed(Button.A, function () {
    basic.showString("Hello!")
})

``` 

## @showdialog 

Ajoute une commande lorsque le bouton B est pressé.   


## Étape 4 

 
Ajoute le bloc ``|| basic: afficher le texte "Hello!" ||`` dans le bloc ``||input:lorsque le bouton B est pressé||``. 

 

Modifie le bloc ``|| basic: Afficher texte ||`` et écris ton nom de famille.
 

```blocks 

input.onButtonPressed(Button.B, function () {
    basic.showString("Hello!")
})

``` 

## @showdialog 

Ajoute une commande lorsque le bouton A+B est pressé.   


## Étape 5 

 
Ajoute le bloc ``|| basic: montrer LEDs ||`` et le bloc ``|| basic: pause (ms) "100" ||`` dans le bloc ``||input:lorsque le bouton A+B est pressé||``. 

 
Crée une petite animination avec trois blocs ``|| basic: montrer LEDs ||`` et trois blocs ``|| basic: pause (ms) "100" ||``.
 

```blocks 

input.onButtonPressed(Button.AB, function () {
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
    basic.pause(100)
})

``` 

## @showdialog 

Félicitations! Tu as terminé de programmer ton porte-nom numérique! 

Ensuite, appuie sur le bouton "Télécharger" pour accéder à l'application MakeCode/Micro:bit.

Teste ton code et amuse-toi bien!