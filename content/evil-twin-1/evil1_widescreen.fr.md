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

*Mise à jour du 1/12/2025* : Il est maintenant possible de jouer en plein écran sans distorsion grâce au mod de AlphaYellow [sur Github](https://github.com/alphayellow1/AlphaYellowWidescreenFixes/releases/tag/eviltwincyprienschronicles).

-   Extraire les fichiers dans le répertoire du jeu.
-   Télécharger [ThirteenAG's Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader/releases) (dinput.dll 32-bit) et placer également le fichier dans le répertoire du jeu.
-   Définir une résolution et un FOV dans EvilTwinCypriensChroniclesWidescreenFix.ini.
-   Exécuter video.exe et choisir la nouvelle résolution dans la liste.

Download :
- [Evil.Twin.Cyprien.s.Chronicles.-.Widescreen.FOV.Fix.v1.0.rar](/files/Evil.Twin.Cyprien.s.Chronicles.-.Widescreen.FOV.Fix.v1.0.rar)
- [dinput-Win32.zip](/files/dinput-Win32.zip)

## Playstation 2

![PCSX2 Cheats screenshot](/images/pcsx2.png)

Le plus simple :-)
- Faites un clic-droit sur la jaquette du jeu
- Propriété > Patchs
- Cochez *Widescreen*