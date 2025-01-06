---
title: "Jouer en plein écran"
author: "Zap' le Simple"
lang: fr
slug: widescreen
---

# Jouer en plein écran

Il est possible sur chacune des versions du jeu (PS2, Windows, Dreamcast) de configurer l’affichage en 16:9. Il s'agit évidemment d'élargir le champ visuel et non d'étirer l'image. Le jeu s'y prête bien avec ses grands espaces. Sur Dreamcast, si vous jouez sur la console, vous aurez par contre de gros ralentissements.

![Exemple de Widescreen](/images/widescreen-simu.gif "Exemple d'affichage panoramique")
{.center-bloc}

## Dreamcast

Sur Dreamcast vous devez éditer le fichier .cdi du jeu ou le .gdi (et travailler alors sur *track05.bin*). Ça n'est pas bien compliqué, il suffit de faire des *Chercher / Remplacer* en ouvrant le fichier dans un éditeur hexadécimal. En gratuit il y'a [Hex Fiend](https://hexfiend.com/) sur Mac et [HxD](https://mh-nexus.de/en/hxd/) sur Windows.

Cherchez et remplacez les chaînes suivantes : (et n'oubliez pas ensuite de configurer l'émulateur en écran 16:9)

Chercher

```
ABAAAA3F 01D00B00 09000000 B03D1B8C
```

Remplacer

```
398EE33F 01D00B00 09000000 B03D1B8C
```

Chercher

```
0B00F9FF 00000040 08B7198C
```

Remplacer

```
0B00F9FF 5555D53F 08B7198C
```

Chercher

```
D0000000 00000040 14A6198C 78AE198C
```

Remplacer

```
D0000000 5555D53F 14A6198C 78AE198C
```

Source : [http://retro-magic.de/](http://retro-magic.de/Dreamcast_Hex_Patches_en)

## Windows

La technique permettant de jouer en plein-écran sur PC, fonctionnait parfaitement à l'époque de Windows XP. Une raison trop technique pour l'auteur de ces lignes l'empêche de fonctionner correctement sur Windows 10.

Même exercice que sur Dreamcast, avec un éditeur hexadécimal ouvrez le fichier *fnx\_core.dll* présent dans le répertoire du jeu. Ensuite :

Chercher

```
C9 7F 7F 9E C9 7F FF 80 02 00 00 E0 01 00 00 10 00
```

Remplacer

```
C9 7F 7F 9E C9 7F FF 90 06 00 00 1A 04 00 00 10 00
```

Maintenant en sélectionnant la résolution 640x480, le jeu se lance en 1680x1050.

Source : [WSGF](https://www.wsgf.org/dr/evil-twin-cypriens-chronicles)

## Playstation 2

![PCSX2 Cheats screenshot](/images/pcsx2.png)

Le plus simple :-)
- Faites un clic-droit sur la jaquette du jeu
- Propriété > Patchs
- Cochez *Widescreen*