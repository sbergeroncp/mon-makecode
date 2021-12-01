# atelier_3dec

## @showdialog
Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs.

Sébastien Bergeron - Conseiller pédagogique

Journée du numérique - 3 décembre 2021

## @showdialog
Transforme ce porte-nom ordinaire en porte-nom numérique!

![CSSBF](https://github.com/sbergeroncp/tuto/blob/master/dice.png?raw=true)

## @showdialog

Ajoute ``|| basic:Montrer l'icône ||`` dans le bloc ``|| basic:Toujours ||``.

Sélectionne l'icône de ton choix. 

Tu peux également choisir ``|| basic:Montrer LEDs ||`` afin de personnaliser l'icône.

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

## Étape

Ajoute ``|| basic:Afficher texte ||`` dans le bloc ``|| input:Lorsque le bouton A est pressé ||``.

Remplace le texte "Hello" par ton prénom.

```blocks
input.onButtonPressed(Button.A, function () {
    basic.showString("Sebastien")
})
```

## Étape

Ajoute ``|| basic:Afficher texte ||`` dans le bloc ``|| input:Lorsque le bouton B est pressé ||``.

Remplace le texte "Hello" par ton nom de famille.

```blocks
input.onButtonPressed(Button.B, function () {
    basic.showString("Bergeron")
})
```

## Étape

Ajoute trois blocs ``|| basic:Montrer LEDs ||`` dans le bloc ``|| Loops:Répéter 2 fois||``.

Ensuite, ajoute ces derniers dans le bloc ``|| input:Lorsque le bouton A+B est pressé ||``. 

Personnalise les trois icônes.

Ajoute un bloc ``|| basic:Pause (100ms) ||`` après chaque icône.

```blocks
input.onButtonPressed(Button.AB, function () {
    for (let index = 0; index < 2; index++) {
        basic.showLeds(`
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            `)
        basic.pause(100)
        basic.showLeds(`
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            `)
        basic.pause(100)
        basic.showLeds(`
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            . . . . .
            `)
        basic.pause(100)
    }
})
```

## Étape

Teste le programme à l'aide du simulateur. Fonctionne-t-il ?

Télécharge le programme dans le micro:bit!

Teste le programme. Fonctionne-t-il ?

Montre le porte-nom aux autres !