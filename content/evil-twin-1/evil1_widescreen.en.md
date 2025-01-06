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

This hack doesn't work anymore on Windows 10. It's too technical for me to figure out the reason why.

Do the same thing as described on the Dreamcast part. Edit *fnx\_core.dll* inside the game folder.

Find

```
C9 7F 7F 9E C9 7F FF 80 02 00 00 E0 01 00 00 10 00
```

Replace

```
C9 7F 7F 9E C9 7F FF 90 06 00 00 1A 04 00 00 10 00
```

Now, configure the game to 640x480 video mode and you'll get 1680x1050.

Source : [WSGF](https://www.wsgf.org/dr/evil-twin-cypriens-chronicles)

## Playstation 2

![PCSX2 Cheats screenshot](/images/pcsx2.en.png)

The easy one !  

- Right-clic on the game
- Properties > Patchs
- Check *Widescreen*