# halloween
# Un Micro:bit d'Halloween! 

## @showdialog 

Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs. 

Sébastien Bergeron - Conseiller pédagogique 

Mélanie Bourque - Enseignante 

## @showdialog 

Voici un exemple de projet réalisé par un élève. 
 
![CSSBF](https://github.com/sbergeroncp/tuto/blob/master/costume_halloween_microbit.png?raw=true) 

## Étape 1 

Supprime les blocs ``|| basic:au démarrage ||`` et ``||basic:toujours||``. 


## Étape 2 

 
Ajoute le bloc ``|| basic: montrer LEDs ||`` dans le bloc ``||input:lorsque "secouer"||``. 

 
Dessine un symbole dans le bloc ``|| basic: montrer LEDs ||``. 

 

```blocks 

input.onGesture(Gesture.Shake, function () { 

    basic.showLeds(` 

        . . . . . 

        . . . . . 

        . . . . . 

        . . . . . 

        . . . . . 

        `) 

}) 

``` 

## @showdialog 

Fais apparaître un symbole lorsque tu inclines à gauche ton oeuvre d'art.  

 

## Étape 3 

 

Ajoute le bloc ``|| basic: montrer LEDs ||`` dans le bloc ``||input:lorsque "incliner à gauche"||``. 

 

Dessine un symbole dans le bloc ``|| basic: montrer LEDs ||``. 

 

```blocks 

input.onGesture(Gesture.TiltLeft, function () { 

    basic.showLeds(` 

        . . . . . 

        . . . . . 

        . . . . . 

        . . . . . 

        . . . . . 

        `) 

}) 

``` 

## Étape 4 
 
Ajoute le bloc ``|| basic: montrer LEDs ||`` dans le bloc ``||input:lorsque "incliner à droite"||``. 

 

Dessine un symbole dans le bloc ``|| basic: montrer LEDs ||``. 

 

```blocks 

input.onGesture(Gesture.TiltRight, function () { 

    basic.showLeds(` 

        . . . . . 

        . . . . . 

        . . . . . 

        . . . . . 

        . . . . . 

        `) 

}) 

``` 

 

## Étape 5 


Ajoute le bloc ``|| basic: afficher texte ||`` dans le bloc ``||input:lorsque le bouton "A" est pressé||``. 

 

Remplace le texte "Hello!" par une onomatopée. 

 

```blocks 

input.onButtonPressed(Button.A, function () { 

    basic.showString("Hello!") 

}) 

``` 

 

## Étape 6 

Ajoute le bloc ``|| basic: afficher texte ||`` dans le bloc ``||input:lorsque le bouton "B" est pressé||``. 

 

Remplace le texte "Hello!" par "Joyeuse Halloween!". 

 

```blocks 

input.onButtonPressed(Button.B, function () { 

    basic.showString("Hello!") 

}) 

``` 

## Étape 7 

Invente une commande avec les blocs de ton choix lorsque tu appuies simmultanément sur les boutons A + B. 

```blocks 

input.onButtonPressed(Button.AB, function () {
    basic.showIcon(IconNames.Target)
    basic.pause(100)
    basic.showString("Hello!")
}) 

``` 

 

## @showdialog 

Félicitations! Tu as terminé de programmer ton Micro:bit d'Halloween! 

Une fois terminé, fais valider le travail par un adulte.

Ensuite, appuie sur le bouton "Télécharger" pour accéder à l'application MakeCode/Micro:bit.

Teste ton code et amuse-toi bien!