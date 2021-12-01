# atelier_3dec

## @showdialog
Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs.

Sébastien Bergeron - Conseiller pédagogique

Journée du numérique - 3 décembre 2021

## @showdialog
Transforme ce porte-nom ordinaire en porte-nom numérique!

![CSSBF](https://github.com/sbergeroncp/tuto/blob/master/dice.png?raw=true)

## Étape 1

Ajoute ``|| basic:Montrer l'icône... ||`` dans le bloc ``|| basic:Toujours... ||``

Sélectionne l'icône de ton choix. 

Tu peux également choisir ``|| basic:Montrer LEDs... ||`` afin de personnaliser l'icône.

```blocks
basic.forever(function () {
    basic.showIcon(IconNames.Heart)
})

basic.forever(function () {
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
})
```

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
```
## Étape 2

