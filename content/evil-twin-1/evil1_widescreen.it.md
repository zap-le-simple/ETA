---
title: "Giocare in widescreen"
author: "Zap' le Simple"
lang: it
slug: widescreen
---

# Giocare in widescreen

È possibile modificare ogni versione di Evil Twin per giocare a schermo intero e godere di miglior campo visivo. Se giocate su un vero Dreamcast, fate attenzione agli alti cali di framerate.

![Widescreen example](/images/widescreen-simu.gif "Giocare in widescreen")
{.center-bloc}

## Dreamcast

Se si utilizza un file .gdi o .cdi è necessario modificare con un editor esadecimale il file *track05.bin*. Potete usare su qualunque sistema operativo [ImHex](https://github.com/WerWolv/ImHex).


Trova

```
ABAAAA3F 01D00B00 09000000 B03D1B8C
```

Sostituisci

```
398EE33F 01D00B00 09000000 B03D1B8C
```

Trova

```
0B00F9FF 00000040 08B7198C
```

Sostituisci

```
0B00F9FF 5555D53F 08B7198C
```

Trova

```
D0000000 00000040 14A6198C 78AE198C
```

Sostituisci

```
D0000000 5555D53F 14A6198C 78AE198C
```

Source : [http://retro-magic.de/](http://retro-magic.de/Dreamcast_Hex_Patches_en)

## Windows

Esegui la stessa procedura descritta per la versione Dreamcast. Modificare *fnx_core.dll* nella cartella del gioco.

Trova

```
C9 7F 7F 9E C9 7F FF 80 02 00 00 E0 01 00 00 10 00
```

Sostituisci

```
C9 7F 7F 9E C9 7F FF 90 06 00 00 1A 04 00 00 10 00
```

Adesso configurate il gioco in 640x480, in questo modo otterrete una risoluzione di 1680x1050.

Source : [WSGF](https://www.wsgf.org/dr/evil-twin-cypriens-chronicles)

## Playstation 2

![PCSX2 Cheats screenshot](/images/pcsx2.it.png)


Questo è facile! Eseguite il gioco, dirigete il mouse su *Impostazioni*, cliccate su *Proprietà del gioco*, poi su *Patch* e abilitate il widescreen.