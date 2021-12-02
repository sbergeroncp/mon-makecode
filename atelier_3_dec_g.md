# atelier_3_dec_g

# Transforme ton micro:bit radio numérique.

## @showdialog 

Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs. 

Sébastien Bergeron - Conseiller pédagogique 

Journée du numérique du 3 décembre 2021

## @showdialog 

Transforme ton micro:bit en radio numérique.
 
![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_g_1.jpg?raw=true) 

## Étape 1 

Supprime les blocs ``|| basic:au démarrage ||`` et ``|| basic:toujours ||`` 


## @showdialog 

Ajoute une commande lorsque le bouton A est pressé. 

## Étape 2 

 Ajoute le bloc ``|| music: "jouer la mélodie"  ||`` dans le bloc ``|| input:lorsque le bouton A est pressé ||``. 
 
Sélectionne une mélodie.

```blocks 

input.onButtonPressed(Button.A, function () {
    music.playMelody("- - - - - - - - ", 120)
})

``` 

## @showdialog 

Ajoute une commande lorsque le bouton B est pressé.  

## Étape 3 
 
Ajoute le bloc ``|| music: "jouer la mélodie"  ||`` dans le bloc ``|| input:lorsque le bouton B est pressé ||``. 
 
 Sélectionne une mélodie

```blocks 

input.onButtonPressed(Button.B, function () {
    music.startMelody(music.builtInMelody(Melodies.Dadadadum), MelodyOptions.Once)
})

``` 

## @showdialog 

Ajoute une commande lorsque le bouton A+B est pressé.  

## Étape 4 
 
Ajoute le bloc ``|| music: "jouer la mélodie"  ||`` dans le bloc ``|| input:lorsque le bouton A+B est pressé ||``. 
 

```blocks 

input.onButtonPressed(Button.AB, function () {
    music.stopAllSounds()
})

``` 

### @showdialog 

Félicitations! Tu as terminé de programmer ta radio numérique! 

Ensuite, appuie sur le bouton "Télécharger" pour accéder à l'application MakeCode/Micro:bit.

### @showdialog

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_g_2.jpg?raw=true) 

Insère le micro:bit dans le bouclier.

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_g_3.jpg?raw=true)

### @showdialog

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_g_4.jpg?raw=true)

Branche le buzzer dans le port "P0" du bouclier.

![CSSBF](https://github.com/sbergeroncp/mon-makecode/blob/master/atelier_g_4.jpg?raw=true)

## @showdialog 

Félicitations! Tu as terminé de brancher ta radio numérique! 

Teste maintenant ta programmation!