# chiffres_des
# Un Micro:bit au lieu d'un dé!

## @showdialog
Ce tutoriel a été réalisé par l'équipe d'intégration du numérique du Centre de services scolaire des Bois-Francs.

Sébastien Bergeron - Conseiller pédagogique

Mélanie Bourque - Enseignante

## @showdialog
Transforme le Micro:bit en dé !

![CSSBF](https://github.com/sbergeroncp/tuto/blob/master/dice.png?raw=true)

L'accéléromètre du microcontrôleur permet de réaliser cette fonction.

## @showdialog
Voici un exemple de projet réalisé par un élève.

![CSSBF](https://github.com/sbergeroncp/tuto/blob/master/micro_bit_lancer_de.gif?raw=true)

## Étape 1

Supprime les blocs ``|| basic:au démarrage ||`` et ``|| basic:toujours||``.

## Étape 2

Crée une variable ``|| variables:Créer une variable... ||``.

Nom de la nouvelle variable : ``|| variables:Nombre ||``.

Ajoute le bloc ``|| math:Choisir au hasard de 1 à 6 ||`` dans le bloc ``||Variables:Définir "Nombre"||``.

Insère cette séquence dans le bloc ``|| input:lorsque "secouer" ||``.

```blocks
let Nombre = 0
input.onGesture(Gesture.Shake, function () {
    Nombre = randint(1, 6)
})
```

## Étape 3

Ajoute un bloc ``|| logic:"0" "=" "0" ||`` dans un bloc ``|| logic:Si "vrai" alors ||``.

Remplace la valeur "0" de gauche par le bloc ``|| variables:"Nombre" ||``.

Remplace la valeur "0" de droite par le nombre "1".

Insère cette séquence de programmation à la suite de la ``|| input:séquence existante ||``.

```blocks
let Nombre = 0
input.onGesture(Gesture.Shake, function () {
    Nombre = randint(1, 6)
    if (Nombre == 1) {
        
    }
})
```

## Étape 4

Ajoute le bloc ``|| basic: montrer LEDs ||``,  ``|| basic: pause (ms) "100" ||`` et ``|| basic: montrer LEDs ||`` à l'intérieur de la séquence existante.

```blocks
let Nombre = 0
input.onGesture(Gesture.Shake, function () {
    Nombre = randint(1, 6)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . # . .
        . . . . .
        . . . . .
        `)
    basic.pause(100)
    basic.showLeds(`
        . . # . .
        . # # . .
        . . # . .
        . . # . .
        . # # # .
        `)
})
```

## @showdialog
Continue de programmer la séquence pour les autres nombres 2 - 3 - 4 - 5 - 6.

## @showdialog
Félicitations! Tu as terminé de programmer ton Micro:bit! 

Une fois terminé, fais valider le travail par un adulte.

Ensuite, appuie sur le bouton "Télécharger" pour accéder à l'application MakeCode/Micro:bit.

Teste ton code et amuse-toi bien!