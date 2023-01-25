---
jupyter:
  jupytext:
    formats: ipynb,md
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.3'
      jupytext_version: 1.14.1
  kernelspec:
    display_name: Python 3 (ipykernel)
    language: python
    name: python3
---

# Parcours 1 : des objets qui réagissent


Rendez-vous à l'adresse : https://amazon.quick-pi.org/ pour apprendre à programmer vos objets connectés en Python en réalisant les activités du Parcours 1.

Copier ci-dessous le code d'accès personnel que vous avez obtenu :


.........


<a id ="melodie"></a>
Lisez la présentation pour [programmer en Python](#programmer_python) , [écrire](#ecrire), [tester](#tester) puis [valider](#valider) votre programme avec [l'interface de FranceIOI](#interface).

> Au fur et à mesure que vous expérimentez et validez vos programmes **par simulation** pour chaque cdcf, recopier votre script dans les cellules de code vides ci-dessous...

## Mélodie :
![1-melodie/icon.png](https://static4.castor-informatique.fr/contests/quickpi_parcours_a_1p.1585649693/1-melodie/icon.png)
Lisez la présentation du [buzzer](#buzzer) et de [la gestion du temps](#sleep).


Écrire un programme qui active le buzzer pour jouer un son.

```python
from quickpi import *

```

Écrire un programme qui joue la note "la", à la fréquence 440Hz, pendant une seconde.

```python
from quickpi import *

```

Écrire un programme qui joue la mélodie “do ré mi ré do”, en jouant chaque note pendant 500ms, l'une après l'autre, puis éteint le buzzer.

Les fréquences des notes sont : Do : 523Hz, Ré : 587Hz, et Mi : 659Hz.

```python
from quickpi import *

```

<a id ="alternance"></a>
## Alternance
![2-allers-retours-de-LEDs/icon.png](https://static4.castor-informatique.fr/contests/quickpi_parcours_a_1p.1585649693/2-allers-retours-de-LEDs/icon.png)

Lisez la présentation de [la boucle de répétition avec l'instruction `for`](#boucles_for), des [LEDs](#leds) et de [la gestion du temps](#sleep).


Écrire un programme qui fait clignoter la LED cinq fois : c'est à dire l'allume pendant 1s, puis l'éteint pendant 1s, puis recommence quatre autres fois.

```python
from quickpi import *

```

Écrire un programme qui allume en alternance les LED rouge et bleue pendant 500ms chacune : la rouge pendant 500ms, la bleue pendant 500ms, etc.

Chacune des LEDs doit être allumée 5 fois au total.

Tout doit être éteint à la fin.

```python
from quickpi import *

```

Écrire un programme qui allume en alternance les LED rouge et bleue 5 fois au total, chaque fois pendant 500ms mais allumant la suivante 100ms avant d'éteindre la précédente : on allume la rouge au tout début, puis allume la bleue au temps 400ms, puis éteint la rouge au temps 500ms, puis allume la rouge au temps 800ms, etc.

```python
from quickpi import *

```

<a id ="show_lumineux_1"></a>
## Show lumineux 1
![3-light-show-1/icon.png](https://static4.castor-informatique.fr/contests/quickpi_parcours_a_1p.1585649693/3-light-show-1/icon.png)
Lisez la présentation de [la boucle de répétition avec l'instruction `for`](#boucles_for), des [LEDs](#leds) et de [la gestion du temps](#sleep).


Écrire un programme qui dans l'ordre :

- Allume la LED rouge pendant 1s
- Fait clignoter la LED bleue 5 fois : 500ms allumée puis 500ms éteinte.
- Allume la LED verte et la laisse allumée.

```python
from quickpi import *

```

Écrire un programme qui dans l'ordre :

- Allume la LED rouge pendant 1s
- Fait clignoter la LED verte 5 fois : 500ms allumée puis 500ms éteinte.
- Fait clignoter la LED bleue 3 fois : 500ms allumée puis 500ms éteinte.
- Rallume la LED verte et la laisse allumée.

```python
from quickpi import *
   
```

Écrire un programme qui joue la séquence suivante, où chaque tiret représente un état allumé de 500ms, et chaque point un état éteint de 500ms.

Notez que les deux lignes se jouent en même temps :
```
- LED rouge : -.-.-.--.-.-.
- LED verte : .......------
```
Les LEDs doivent être éteintes à la fin du programme.

```python
from quickpi import *

```

<a id ="direction"></a>
## Quelle direction ?
![4-afficher-la-direction/icon.png](https://static4.castor-informatique.fr/contests/quickpi_parcours_a_1p.1585649693/4-afficher-la-direction/icon.png)
Lisez la présentation de : [la boucle infinie](#boucle_infinie), [l'instruction if](#if), [l'écran](#ecran), [le bouton poussoir](#bouton_poussoir) et [la manette](#manette).


Écrire un programme qui laisse l'écran vide au début, puis affiche le texte "Bonjour" dès que l'on appuie sur le bouton, et le laisse affiché.

Votre programme devra boucler indéfiniment, et tester en permanence si le bouton est enfoncé. Notez qu'un texte affiché à l'écran y reste jusqu'à ce que l'on affiche autre chose.

```python
from quickpi import *

```

Écrire un programme qui :

- affiche le texte "Appuyez"
- affiche le texte "Merci" dès que l'on appuie sur le bouton, et le laisse affiché.

```python
from quickpi import *

```

Écrire un programme qui :

- affiche le texte "Direction ?" dès le début
- puis lorsque l'on appuie sur une direction, affiche le texte "Haut", "Droite", "Bas" ou "Gauche" selon la direction appuyée.



```python
from quickpi import *

```

<a id ="instrument"></a>
## Instrument
![5-instrument-de-musique/icon.png](https://static4.castor-informatique.fr/contests/quickpi_parcours_a_1p.1585649693/5-instrument-de-musique/icon.png)
Lisez la présentation de [la boucle infinie](#boucle_infinie), de [l'instruction if](#if), du [capteur de distance](#capteur_distance) et du [buzzer](#buzzer).


Écrire un programme qui allume le buzzer quand le capteur détecte un objet à moins de 100cm, et arrête le buzzer dès qu'il n'en détecte plus.

```python
from quickpi import *

```

Écrire un programme qui allume le buzzer quand le capteur détecte un objet à moins de 500cm.

Le buzzer doit jouer un son à une fréquence égale à la distance de l'objet en centimètres. Il doit être éteint s'il n'y a pas d'objet à moins de 500cm.

```python
from quickpi import *

```

Modifier le programme de la version précédente, avec la différence suivante : lorsque le bouton est enfoncé, la fréquence du buzzer doit être doublée.

```python
from quickpi import *

```

<a id ="show_lumineux_2"></a>
## Show Lumineux 2 :
![6-light-show-2/icon.png](https://static4.castor-informatique.fr/contests/quickpi_parcours_a_1p.1585649693/6-light-show-2/icon.png)
Lisez la présentation [des boucles imbriquées avec l'instruction for](#boucles_imbriquees), des [LEDs](#leds) et de [la gestion du temps](#sleep).


Écrire un programme qui fait 3 fois ces deux étapes :

- Faire clignoter la LED rouge 3 fois (200ms allumée puis 200ms éteinte)
- Attendre 1 seconde.

```python
from quickpi import *

```

Écrire un programme qui fait 3 fois ces deux étapes :

- Clignoter la LED rouge 3 fois (200ms allumée puis 200ms éteinte)
- Clignoter la LED verte 3 fois (200ms allumée puis 200ms éteinte)
- Clignoter la LED bleue 3 fois (200ms allumée puis 200ms éteinte)
- Attendre 1 seconde.

```python
from quickpi import *

```

Écrire un programme qui fait en même temps, et pendant 4 secondes au total :

- Clignoter la LED rouge : 1s allumée puis 1s éteinte
- Clignoter la LED verte : 500ms allumée puis 500ms éteinte
- Clignoter la LED bleue : 250ms allumée puis 250ms éteinte

```python
from quickpi import *

```

<a id ="avertisseur"></a>
## Avertisseur :
![7-avertisseur-de-recul/icon.png](https://static4.castor-informatique.fr/contests/quickpi_parcours_a_1p.1585649693/7-avertisseur-de-recul/icon.png)

Lisez la présentation de [la boucle infinie](#boucle_infinie), de [l'instruction if/else](#if/else), de [la boucle de répétition avec l'instruction `for`](#boucles_for), du [capteur de distance](#capteur_distance), du [buzzer](#buzzer), et de [la gestion du temps](#sleep).


Écrire un programme qui, dès qu'un objet passe à moins de 30cm du capteur, fait dans l'ordre :
- Jouer 3 bips de 100ms espacés de 100ms
- Attendre 500ms

```python
from quickpi import *

```

Modifiez le programme de la version précédente, pour qu'il arrête de jouer des bips dès qu'il n'y a plus d'objet.

S'il y a un bip en cours, il se termine, mais on ne joue pas le suivant.

```python
from quickpi import *

```

Modifiez le programme de la version précédente, pour que lorsqu'un objet passe à moins de 10cm du capteur alors qu'une série de bips n'est pas en cours, alors il joue un bip en continu.

Au dessus de cette distance, il doit faire comme dans la version précédente.

```python
from quickpi import *

```

<a id="servo_chronometre"></a>
##  Servo chronométré :
![8-servo-chronometre/icon.png](https://static4.castor-informatique.fr/contests/quickpi_parcours_a_1p.1585649693/8-servo-chronometre/icon.png)
Lisez la présentation du [servomoteur](#servomoteur), de [la boucle infinie](#boucle_infinie), de [l'instruction if/else](#if/else), de [la boucle de répétition avec l'instruction `for`](#boucles_for), de [la manette](#manette), du [buzzer](#buzzer), des [LEDs](#leds), et de [la gestion du temps](#sleep).


Écrire un programme qui met l'angle du servomoteur à 0°, puis lorsque l'on appuie sur le bouton :

- Augmente l'angle 18 fois de 10°, toutes les 50ms
- Joue un bip pendant 500ms
- Remet l'angle à 0°

```python
from quickpi import *

```

Écrire un programme qui met le servomoteur à 10°, puis lorsque que le stick est appuyé :

- À gauche : diminue de 2° puis attend 50ms
- À droite : augmente de 2° puis attend 50ms

Le programme doit ignorer les actions qui ne gardent pas l'angle entre 10° et 170°.

```python
from quickpi import *

```

Modifier le programme de la version précédente, pour qu'il arrête au bout de 5s, puis selon l'angle du servo :

- S'il vaut 90°, allume la LED verte
- S'il est inférieur à 90°, allume la LED rouge
- S'il est supérieur à 90°, allume la LED bleue

Le programme doit ensuite attendre 2s, puis éteindre les LEDs et tout recommencer.

```python
from quickpi import *

```

# Les instructions utiles en Python :

<!-- #region -->
<a id ="programmer_python"></a>
## Programmation :

Python permet de créer des programmes à partir d'instructions.

Par exemple, l'instruction `droite()` peut faire déplacer un robot d'une case vers la droite.

Un programme formé d'instructions les unes en dessous des autres, exécute ces instructions l'une après l'autre.
```python
from robot import *

droite()
haut()
droite()
```
Le programme ci-dessus fait déplacer le robot vers la droite, puis vers le haut, puis de nouveau vers la droite.

**>>> [Mélodie](#melodie)**
<!-- #endregion -->

<!-- #region -->
<a id ="if"></a>
### l'instruction if :

Avec l'instruction if, on peut exécuter une instruction uniquement dans certaines conditions.
```python
if caseMarquee():
    peindre()
```
Par exemple, le programme ci-dessus teste le contenu de la case du robot, et ne la peint que si elle est marquée.

On peut aussi placer plusieurs instructions dans une instruction if, comme illustré ci-dessous :

```python
if caseMarquee():
    peindre()
    droite()
```
**>>> [Quelle direction ?](#direction)   >>>  [Intrument](#instrument)**
<!-- #endregion -->

<!-- #region -->
<a id ="if/else"></a>
### l'instruction if/else

On peut utiliser une instruction if/else, pour effectuer des opérations différentes selon la situation. Par exemple :
```python
if caseMarquee():
    peindre()
else:
    haut()
```
Dans le programme ci-dessus, si la case du robot est marquée, le robot la peint, sinon il ne la peint pas mais se déplace vers le haut.

**>>> [Instrument](#instrument)  >>>  [Avertisseur](#avertisseur) >>>  [Servo_chronométré](#servo_chronometre)**
<!-- #endregion -->

<!-- #region -->
<a id ="boucle_infinie"></a>
## La boucle infinie :

On peut utiliser l'instruction `while True :` pour répéter sans fin une séquence d'instructions, comme dans l'exemple ci-dessous, qui allume et éteint une LED toutes les 500 millisecondes :
```python
while True :
    allumerLED()
    attendre(1000)
    eteindreLED()
    attendre(1000)
```
L'instruction `while True :` exécute en boucle les instructions placées en dessous, indentées vers la droite, sans s'arrêter, jusqu'à ce que l'on interrompe l'exécution du programme.

Ce type de boucle est utile pour les programmes qui ne doivent jamais s'arrêter, par exemple le programme d'un système d'alarme, qui doit être actif en permanence.

**>>>  [Quelle direction ?](#direction)  >>>  [Intrument](#instrument)  >>>  [Avertisseur](#avertisseur) >>>  [Servo_chronométré](#servo_chronometre)**
<!-- #endregion -->

<!-- #region -->
<a id ="boucles_for"></a>
## Boucle de répétition avec l'instruction `for` :

Pour exécuter plusieurs fois la même instruction, on peut utiliser l'instruction `for loop in range(...)`.

Par exemple, plutôt que de mettre 5 fois la même instruction :
```python
droite()
droite()
droite()
droite()
droite()
```
On peut écrire la boucle suivante :
```python
for loop in range(5):
    droite()
```   
On peut aussi mettre plusieurs instructions dans une boucle :
```python
for loop in range(5):
    droite()
    haut()
```
**>>>  [Alternance](#alternance) >>> [Show lumineux 1](#show_lumineux_1)  >>>  [Avertisseur](#avertisseur) >>>  [Servo_chronométré](#servo_chronometre)**
<!-- #endregion -->

<!-- #region -->
<a id ="boucles_imbriquees"></a>
### Boucles imbriquées :

Il est possible d'utiliser des boucles imbriquées, c'est-à-dire que l'on peut mettre des boucles for, à l'intérieur d'autres boucles for.

Par exemple :
```python
for loop in range(5):
    droite()
    for loop in range(3):
        haut()
    droite()
```    
Ce programme répétera 5 fois un déplacement d'1 case vers la droite, 3 cases vers le haut et 1 case vers la droite.

**>>>  [Show lumineux 2](#show_lumineux_2)**
<!-- #endregion -->

<a id ="interface"></a>
# L'interface FranceIOI :

L'interface comporte deux onglets EXPÉRIMENTER et VALIDER, qui correspondent à deux modes d'utilisation différents.

<img src="https://static4.castor-informatique.fr/help/quickpi_img/experimenter_p.png" alt="experimenter_p.png" title="experimenter_p.png" width="90%">

**>>> [Mélodie](#melodie)**


<a id ="ecrire"></a>
## Ecrire un programme :

C'est à droite dans l'éditeur que vous allez écrire vos programmes en langage python.

Votre programme doit toujours commencer par la ligne `from quickpi import *`.

Cette ligne de code permet de pouvoir utiliser les fonctions spécialement définies pour le module QuickPi.

Les fonctions et mots clés disponibles sont répertoriés dans des listes déroulantes.

Ensuite, vous écrivez les instructions de votre programme les unes en-dessous des autres.

**>>> [Mélodie](#melodie)**


<a id ="tester"></a>
## Tester un programme :

L'onglet EXPÉRIMENTER est en quelque sotre un "bac à sable". Il vous permet de mener des expérimentations avec les composants et les fonctions disponibles dans l'interface.

Un ou des composants sont mis à votre disposition sur l'interface.

<img src="https://static4.castor-informatique.fr/help/quickpi_img/onglet_experimenter.png" alt="onglet_experimenter.png" title="onglet_experimenter.png" width="30%">

Vous pouvez tester ces composants en cliquant dessus pour changer leur état.

Exemple : cliquer sur une LED pour l'allumer.

Pour exécuter votre programme, cliquez sur le bouton  en bas à gauche de l'écran.

<img src="https://static4.castor-informatique.fr/help/quickpi_img/interface_p.png" alt="interface_p.png" title="interface_p.png" width="90%">

N'importe quel programme que vous concevez est exécuté entièrement, avec une simulation visuelle ou auditive du fonctionnement des composants.

**>>> [Mélodie](#melodie)**


<a id ="valider"></a>
## Valider un programme :
	
Votre mission consiste à concevoir un programme qui permet d'effectuer la tâche demandée dans l'énoncé.

L'onglet VALIDER permet une validation automatique des programmes soumis : grâce à un test, le programme présent dans l'éditeur est automatiquement évalué.

Voici comment fonctionne ce test :

<img src="https://static4.castor-informatique.fr/help/quickpi_img/valider_p.png" alt="valider_p.png" title="valider_p.png" width="90%"> 

Une ligne du temps (en secondes) est présente pour chaque composant disponible.

Cette ligne du temps apparaît en gris lorsque le composant est activé pendant la période, sinon elle n'apparaît pas.

Au fur et à mesure de l'exécution du programme, un curseur se déplace horizontalement et vérifie que l'état des composants est conforme à ce qui est attendu.

Dans l'exemple, la LED doit être initialement éteinte (état OFF), puis allumée (état ON, ligne grise) entre les instants 0 et 3, puis à nouveau éteinte à l'instant 3.

**>>> [Mélodie](#melodie)**


# Les fonctions utiles des composants :

<!-- #region -->
<a id ="sleep"></a>
## Gestion du temps :

<img src="https://static4.castor-informatique.fr/help/quickpi_img/time.png" alt="time.png" title="time.png" width="15%">

- `sleep(milliseconds)`

    Cette fonction permet de stopper l'exécution du programme pendant une durée entrée en paramètre.
    
    Cette durée est exprimée en millisecondes.
    
    Exemple :
```python    
sleep(1000)
```
    Pour stopper l'exécution du programme pendant une durée de 1 seconde.
    
**>>> [Mélodie](#melodie) >>>  [Alternance](#alternance) >>> [Show lumineux 1](#show_lumineux_1) >>> [Show lumineux 2](#show_lumineux_2)  >>>  [Avertisseur](#avertisseur) >>>  [Servo_chronométré](#servo_chronometre)**
<!-- #endregion -->

<!-- #region -->
<a id ="buzzer"></a>
## Buzzer :
Un buzzer est un composant qui produit un son lorsqu'il est soumis à un tension électrique.
<a href="http://wiki.seeedstudio.com/Grove-Buzzer/"><img src="https://files.seeedstudio.com/wiki/Grove_Buzzer/img/buzzer_s.jpg"></a>
Un buzzer possède deux états :

- ON : le buzzer est soumis à une tension électrique, il sonne.
![buzzer-ringing.png](https://static4.castor-informatique.fr/modules/img/quickpi/buzzer-ringing.png)
- OFF : sans tension électrique, le buzzer reste silencieux.
![buzzer.png](https://static4.castor-informatique.fr/modules/img/quickpi/buzzer.png)

Le son peut être toujours le même ou être paramétrable.


**Fonctions disponibles :**

- `turnBuzzerOn()`

    Cette fonction permet d'allumer le buzzer.
    
    
- `turnBuzzerOff()`

    Cette fonction permet d'éteindre le buzzer.
    
- `setBuzzerNote(buzzer, frequency)`

    Pour le buzzer entré en paramètre, cette fonction permet de produire un son à une fréquence donnée.
    
    La fréquence est exprimée en Hertz.
    
    Exemple : 
```python    
setBuzzerNote("buzzer1", 264)
```
    permet de jouer la note DO.

**>>> [Mélodie](#melodie)   >>>  [Intrument](#instrument)  >>>  [Avertisseur](#avertisseur) >>>  [Servo_chronométré](#servo_chronometre)**
<!-- #endregion -->

<!-- #region -->
<a id ="leds"></a>	
## LEDs ou diodes électroluminescentes :

Une LED est un composant qui émet de la lumière quand il est parcouru par un courant électrique.
<a href="http://wiki.seeedstudio.com/Grove-Red_LED/"><img src="https://www.gotronic.fr/ar-led-rouge-5-mm-grove-104030005-19005.jpg"></a>
Une LED possède deux états :

- ON : le courant traverse la LED, elle est allumée :
![ledon-red.png](https://static4.castor-informatique.fr/modules/img/quickpi/ledon-red.png)

- OFF : il n'y a pas de courant, la LED est éteinte :
![ledoff.png](https://static4.castor-informatique.fr/modules/img/quickpi/ledoff.png)

Une LED ne laisse passer le courant électrique que dans un seul sens.

On trouve des LEDs qui émettent de la lumière rouge ou de la lumière verte, ou d'autres couleurs encore.

**Fonctions disponibles** :

- Les fonctions `turnLedOn()` et `turnLedOff()` permettent respectivement d'allumer et d'éteindre une LED.

    Elles ne peuvent servir que lorsqu'il n'y a qu'une seule LED utilisée.


- `setLedState(led,state)` :

    Cette fonction permet d'allumer ou éteindre une LED.
    
    Elle prend en paramètre le nom de la LED et l'état à considérer, True pour l'allumer, False pour l'éteindre.
    
    Exemple :
```python    
setLedState("led1",True)
```

- `toggleLedState(led)` :

    Cette fonction permet d'inverser l'état de la LED entrée en paramètre sous forme de chaine de caractères.
    
    Exemple :
```python    
toggleLedState("led1")
```

**>>>  [Alternance](#alternance) >>> [Show lumineux 1](#show_lumineux_1) >>> [Show lumineux 2](#show_lumineux_2) >>>  [Servo_chronométré](#servo_chronometre)**
<!-- #endregion -->

<!-- #region -->
<a id ="bouton_poussoir"></a>
## Bouton poussoir
<a href="http://wiki.seeedstudio.com/Grove-Button/"><img src="https://www.gotronic.fr/ar-module-bouton-grove-101020003-19052.jpg"></a>
Un bouton poussoir est un élément qui possède deux états, relevé et enfoncé.
- ON : le bouton est enfoncé :
![buttonon.png](https://static4.castor-informatique.fr/modules/img/quickpi/buttonon.png)
- OFF : le bouton est relevé :	
![buttonoff.png](https://static4.castor-informatique.fr/modules/img/quickpi/buttonoff.png)
	
**Fonctions disponibles :**

- `isButtonPressed()`

    Cette fonction renvoie `True` si le bouton est enfoncé, et `False` s'il est relevé.

    Cette fonction est utilisée seulement lorsqu'il n'y a qu'un seul bouton pressoir sur le montage.
    
<br>   

- `isButtonPressed(button)`

    Pour le bouton entré en paramètre sous forme de chaine de caractères, cette fonction renvoie `True` si le bouton est enfoncé, et `False` s'il est relevé.
    
    Exemple : 
```python    
isButtonPressed("button1")
```	

**>>> [Quelle direction ?](#direction)**
<!-- #endregion -->

<!-- #region -->
<a id ="ecran"></a>	
## Écran :

![screen.png](https://static4.castor-informatique.fr/modules/img/quickpi/screen.png)

L'écran de ce module est un petit écran monochrome de (132 x 33) pixels qui permet d'afficher deux lignes de 16 caractères.
<a href="http://wiki.seeedstudio.com/Grove-16x2_LCD_Series/"><img src="https://www.gotronic.fr/ar-afficheur-lcd-i2c-grove-104020113-28877.jpg"></a>
**Fonctions disponibles** :

- `displayText(line1, line2)`

    Cette fonction permet d'afficher deux lignes de texte sur un écran.
    
    Elle prend en paramètre une ou deux lignes à afficher, sous forme de chaines de caractères.
    
    Le paramètre de la deuxième ligne est optionnel. 

    Exemple : avec le code 
```python    
displayText("Hello", "World !")
```
    on affiche Hello sur la première ligne, et World ! sur la deuxième ligne de l'écran.

    
**>>>  [Quelle direction ?](#direction)**
<!-- #endregion -->

<!-- #region -->
<a id ="manette"></a>
## Manette :
![stick.png](https://static4.castor-informatique.fr/modules/img/quickpi/stick.png)

Une manette (stick en anglais) est un ensemble de 5 boutons, chacun correspondant à une direction : haut, droite, bas, gauche ou bien centre.

Il s'agit d'un seul composant, mais qui se programme comme 5 boutons différents :

- "stick1.up" pour la direction haut de la manette "stick1"
- "stick1.right" pour la direction droite
- "stick1.down" pour la direction bas
- "stick1.left" pour la direction gauche
- "stick1.center" pour la direction centre

Par exemple pour tester si la direction haut est enfoncée, on utilise :
```python 
buttonState("stick1.up")
```
**>>>  [Quelle direction ?](#direction) >>>  [Servo_chronométré](#servo_chronometre)**
<!-- #endregion -->

<!-- #region -->
<a id ="capteur_distance"></a>	
## Capteur de distance :
![range.png](https://static4.castor-informatique.fr/modules/img/quickpi/range.png)
Ce capteur permet de mesurer la distance sans contact grâce à un capteur à ultrasons ou à laser. Il a une portée de 3 centimètres à 5 mètres.
<a href="http://wiki.seeedstudio.com/Grove-Ultrasonic_Ranger/"><img src="https://www.gotronic.fr/ar-telemetre-a-ultrasons-grove-101020010-18976.jpg"></a>
**Fonctions disponibles :**
- `readDistance(range)`

    Cette fonction renvoie la distance captée par le capteur de distance entré en paramètre.
    Cette distance est exprimée en centimètres.

    Exemple : 
```python
readDistance("range1")
```
**>>> [Instrument](#instrument)  >>>  [Avertisseur](#avertisseur)**
<!-- #endregion -->

<!-- #region -->
<a id ="servomoteur"></a>	
## Servomoteur :
![servo-full.png](https://static4.castor-informatique.fr/modules/img/quickpi/servo-full.png)
Le Servomoteur est un petit moteur qui peut tourner précisément jusqu'à un angle donné, entre 0 et 180 degrés. On peut l'utiliser pour contrôler la direction des roues d'un petit véhicule, ou pour ouvrir ou fermer une barrière, etc.

**Fonctions disponibles :**

- `setServoAngle(servo, angle)`

    Cette fonction permet de modifier l'angle du servomoteur choisi. L'angle est exprimés en degrés, entre 0 et 180 degrés.

    Exemple :
```python
setServoAngle("servo1", 90)`
```


- `getServoAngle(servo)`

    Ce bloc permet de relire l'angle auquel on a réglé le servomoteur choisi. Ce n'est pas un capteur, mais simplement une mémorisation de la dernière valeur modifiée par une instruction.

    On peut par exemple l'utiliser pour augmenter l'angle de 1 degré.

    Exemple :
```python
setServoAngle("servo1", getServoAngle("servo1") + 1)
```
**>>>  [Servo_chronométré](#servo_chronometre)**
<!-- #endregion -->

****



<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />Ce document, basé sur du contenu de [France-IOI](http://www.france-ioi.org/), est mis à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Licence Creative Commons Attribution -  Partage dans les Mêmes Conditions 4.0 International</a>.

Pour toute question, suggestion ou commentaire : <a href="mailto:eric.madec@ecmorlaix.fr">eric.madec@ecmorlaix.fr</a>
