---
title: "Widescreen"
author: "Zap' le Simple"
lang: en
slug: widescreen
---

# Playing Widescreen

On each version of Evil Twin, you can hack the game to play fullscreen and enjoy a better field of view. If you play on an original Dreamcast, beware of high fps drops.

![Widescreen example](/images/widescreen-simu.gif "Exemple d'affichage panoramique")
{.center-bloc}

## Dreamcast

On Dreamcast you need to edit with an hexa editor the *track05.bin* if you use a .gdi dump. Otherwise edit the .cdi disk. On Mac you can use the free [Hex Fiend](https://hexfiend.com/) and [HxD](https://mh-nexus.de/en/hxd/) on Windows.

You just need to find & replace the following values.

Don't forget to configure the video output of your emulator to widescreen.

Find

```
ABAAAA3F 01D00B00 09000000 B03D1B8C
```

Replace

```
398EE33F 01D00B00 09000000 B03D1B8C
```

Find

```
0B00F9FF 00000040 08B7198C
```

Replace

```
0B00F9FF 5555D53F 08B7198C
```

Find

```
D0000000 00000040 14A6198C 78AE198C
```

Replace

```
D0000000 5555D53F 14A6198C 78AE198C
```

Source : [http://retro-magic.de/](http://retro-magic.de/Dreamcast_Hex_Patches_en)

## Windows

*Update from the first of december 2025* : You can now play widescreen thanks to AlphaYellow by using this [mod on Github](https://github.com/alphayellow1/AlphaYellowWidescreenFixes/releases/tag/eviltwincyprienschronicles).

-   Extract all files to the game folder.
-   Download [ThirteenAG's Ultimate ASI Loader](https://github.com/ThirteenAG/Ultimate-ASI-Loader/releases)  (32-bit version of dinput.dll), and also extract it to the game folder.
-   Set the desired resolution and FOV factor in EvilTwinCypriensChroniclesWidescreenFix.ini.
-   Run video.exe and choose the new resolution in the list.

Download : 
- [Evil.Twin.Cyprien.s.Chronicles.-.Widescreen.FOV.Fix.v1.0.rar](/files/Evil.Twin.Cyprien.s.Chronicles.-.Widescreen.FOV.Fix.v1.0.rar)
- [dinput-Win32.zip](/files/dinput-Win32.zip)


## Playstation 2

![PCSX2 Cheats screenshot](/images/pcsx2.en.png)

The easy one !  

- Right-clic on the game
- Properties > Patchs
- Check *Widescreen*