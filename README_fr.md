# Esk2C - Skateboard Electrique

**Coment en costruire un ?**

> Skateboard / Longboard électrique Open-source et accessible à tous
> 

# Hardware

**Un simple skateboard** peut être utilisé pour cela, il n'est pas nécessaire d'en avoir un spécifique ou d'en construire un de toutes pièces (mais c'est tout de même possible si vous le shouaitez).
Un skateboard est composé d'une planche, de Trucks, de roues, de roulements et d'un Grip. Vous pouvez le construire pièce par pièce, utiliser un ancien ou acheter un skateboard pré-monté.

## Motorisation

Il existe deux types de motorisation :
- Moteur-poulie
- Roue-moteur

### Moteur-poulie

Un moteur entraîne une courroie qui entraîne une roue. C'est un système apparent situé sous le skateboard ou à l'arrière du skateboard contrairement au système roue-moteur où le moteur est invisible. Avec ce système, de nombreux composants peuvent devoir être remplacés après de nombreuses utilisations. (Courroie, poulie, moteur). Ce système peut être composé d'un ou deux moteurs qui peuvent être modifiés, changés et améliorés.

| Composant | Spécifications |
| --- | --- |
| Le moteur doit être un moteur sans balais. La puissance peut varier et être calculée en fonction de la vitesse maximale souhaitée. Les moteurs peuvent être achetés sur différents sites spécialisés (https://www.mboards.co/collections/electric-skateboard-motors) ou auprès de fournisseurs tels qu'aliexpress.  Les moteurs les plus courants pour les projets de skatboard électrique sont des moteurs brushless de près de 200Kv. L'utilisation de deux moteurs au lieu d'un n'augmente pas la vitesse maximale mais permet une augmentation plus rapide de la vitesse.
| La courroie dépend de votre poulie, de votre support et de votre roue. Elle doit être achetée et vous ne pouvez pas la faire vous-même. Disponible sur plusieurs sites et dans toutes les tailles comme ici : https://www.mboards.co/collections/pulleys-and-mounts |
| La poulie de moteur peut être imprimée en 3D si le moteur n'est pas trop lourd et la vitesse pas trop élevée. Si vous l'imprimez, n'utilisez pas de PLA et utilisez un matériau résistant à la chaleur comme le filament de carbone. https://www.thingiverse.com/thing:2337126 Disponible sur différents sites comme ici : https://www.mboards.co/collections/pulleys-and-mounts |
| La taille varie en fonction du diamètre de votre roue. Peut être imprimée en 3D. Si vous l'imprimez, n'utilisez pas de PLA et utilisez un matériau résistant à la chaleur comme le filament de carbone. https://www.thingiverse.com/thing:2337126 Peut être acheté sur plusieurs sites comme ici : https://www.mboards.co/collections/pulleys-and-mounts |
| Support moteur : Peut être imprimé en 3D. Si vous l'imprimez, n'utilisez pas de PLA et utilisez un matériau résistant à la chaleur comme le filament de carbone. https://www.thingiverse.com/thing:2429445/files Peut être acheté sur de nombreux sites comme ici : https://www.mboards.co/collections/pulleys-and-mounts |

Attention, faites attention à la compatibilité des Trucks avec le support du moteur et ne prenez pas de roues complètement remplies de plastique mais avec des trous où vous pouvez visser la poulie.

### Roue-Moteur

Le moteur est directement intégré aux roues arrière. Ce système est plus esthétique car on ne voit pas le moteur. Cependant, les roues arrière et le moteur peuvent être compliqués à changer en cas de casse ou pour améliorer sans changer toute la roue.
L'utilisation de deux moteurs In-Wheel est préférable pour ce système contrairement au moteur-poulie qui peut se contenter d'un seul moteur.

| Composant | Spécifications |
| --- | --- |
| Roue-Moteur | On peut le trouver dans de nombreuses couleurs et tailles sur différents sites comme ici : http://www.diyeboard.com/hub-motor-8352mm-450w-75kv-for-diy-electric-skateboard-p-536.html?zenid=ka8sls2lth4h54md18q2bsi2i0 |.

## Electronique

De l'électronique est nécessaire pour utiliser le skateboard électrique. 

| Composant | Spécifications |
| --- | --- |
| ESC | *Electronic Speed Controller*. La carte la plus courante est une carte vESC pré-construite ou une simple carte ESC pour les skateboards électroniques. Cette carte peut être construite avec un raspberry pi ou un Arduino mais elle est plus complexe à réaliser. L'ESC dépend de la capacité de la batterie et des moteurs. |
| Batterie | Les plus utilisées sont les batteries LiPo avec 5000mAh minimum. La batterie utilisée peut être composée de plusieures cellules et est indiqué par un numéro et la lettre "s" ou "p" (connexion en série ou en parallèle). Préférez la batterie avec le plus d'éléments. |
| Télécommande | La plupart des cartes ESC ont une télécommande Radio fournie. Cependant, vous pouvez acheter différentes télécommandes, construire le vôtre ou simplement prendre une télécommande de console de jeu vidéo (comme le nunchuck de la Wii). Vous pouvez trouver plusieurs protocoles de communication utilisés par les contrôleurs. Radio 2.4GHz, filaire, Bluetooth ou Wifi. |

### ESC

*Electronic Speed Controller*. Cette carte régule l'électricité émise par les batteries pour modifier la vitesse du skateboard en fonction du signal émis par la télécommande. C'est un composant qui a tendance à chauffer et qui doit être refroidi.

Vous devez en choisir un et faire attention au support de la batterie et des moteurs.
Il existe de nombreuses solutions d'ESC :

- vESC avec le logiciel vESC
- ESC
- Arduino avec un circuit ESC
- Raspberry Pi avec un circuit ESC

**vESC**

Ce sont les tableaux les plus professionnels et ils utilisent un logiciel spécifique mais sont très coûteux. Ils ne sont pas trop complexes à utiliser et ont une grande communauté d'utilisateurs.

**ESC**

Ils sont similaires à la carte vESC mais avec un logiciel et un matériel différents. Ils sont abordables.

**Arduino / Raspberry ESC**

Ils sont très complexes à utiliser, vous devez rédiger un code et être sûr qu'il fonctionne. Il est dangereux d'utiliser du code dont on en est pas certain. Mais avec cette solution, le skateboard est entièrement personnalisé et open source.
Si vous utilisez cette solution, vous avez besoin d'un circuit ESC. Il s'agit simplement d'un circuit imprimé externe qui contrôle la puissance de la batterie en fonction des données envoyées par l'Arduino ou le Raspberry pi.

Vous pouvez retrouver des projets utilisants des ESC sous Raspberry Pi ou Arduino sur le web :
- [https://www.youtube.com/watch?v=2WLEur3M8Yk&t=1s](https://www.youtube.com/watch?v=2WLEur3M8Yk&t=1s)
- [https://www.youtube.com/watch?v=cYdv3y90FEM&t=616s](https://www.youtube.com/watch?v=cYdv3y90FEM&t=616s)

### Batterie

Ce sont des batteries LiPo. Elles doivent être de 5000mAh (ou 5Ah) et de 20V à 40V environ. Elles peuvent être achetées pré-construites ou vous pouvez le faire vous-même avec quelques petites cellules LiPo.

Les cellules forment plusieurs packs de cellules et sont connectés en série ou en parallèle. Cela est indiqué par un chiffre qui indique le nombre de cellules suivi d'une lettreune lettre ("s" ou "p").

Préférez la batterie Li-Po ayant la plus grande capacité et comportant le plus grand nombre d'éléments.

### Télécommande

La télécommande contrôle la vitesse du skateboard. Il en existe plusieurs types que vous pouvez acheter mais vous pouvez aussi construire la vôtre.

La télécommande communique avec l'ESC par radio, Bluetooth, fils ou parfois Wifi. 
Vous pouvez utiliser n'importe quelle télécommande ou manette comme la Manette de Xbox ou la Wiimote pour contrôler votre skateboard. Certaines personnes ont construit leur propre télécommande et publient leur travail sur le web.

Vous pouvez trouver certains projets de la communauté comme celui là sur le web :
- https://www.youtube.com/watch?v=ik0lJ54-LWc

## Boitier

Tous les appareils électroniques doivent être protégés et stockés. Le boîtier peut être acheté dans de nombreux magasins, peut être imprimé en 3D ou vous pouvez le faire vous-même avec une boîte en plastique, du bois et plus encore. Si vous l'imprimez, vous pouvez utiliser du PLA mais vous pouvez aussi le renforcer avec de la colle Epoxy pour le rendre "imperméable" si vous conduisez quand il pleut.

Un boîtier a besoin d'un emplacement pour le bouton On/Off ESC, le port de charge, l'indicateur de batterie et certaines fois, un bouton On/Off pour la batterie.

## Et plus …

Plusieurs “add-ons” et accessoires peuvent être ajouté à votre skateboard tels que :: 

- Un compteur de Vitesse VESC : [https://www.youtube.com/watch?v=x95_16zzV8s&t=29s](https://www.youtube.com/watch?v=x95_16zzV8s&t=29s)
- Des LEDs : [https://www.youtube.com/watch?v=NQ8VI-0C18U&t=407s](https://www.youtube.com/watch?v=NQ8VI-0C18U&t=407s)
- Des roues tout-terrain : [https://www.youtube.com/watch?v=B-Gqwqf2An0&t=306s](https://www.youtube.com/watch?v=B-Gqwqf2An0&t=306s)
- Et bien plus …
