---
title: "Jouer à Evil Twin sur Windows 10"
author: "Zap' le Simple"
lang: fr
slug: evil-twin-on-modern-windows
---

# Jouer à Evil Twin sur Windows 10

Un tutoriel rapide pour jouer à Evil Twin sur Windows 10, avec une manette actuelle (par exemple Xbox One) et en haute résolution.

## Installer et préparer les .exe

- Installer le jeu, soit depuis les CDs d'origine soit depuis des images disques via WinCDEmu.

- Récupérer et installer la [mise à jour update1](/files/)  afin de lancer le jeu sur Windows XP et ultérieur.

- [Installer le no-CD](/files/) car depuis Windows 10, ni SafeDisc ni SecuROM fonctionnent.

- Changer les propriétés de EvilTwin.exe, Video.exe, Splash.exe et SuperPadCfg.exe avec les réglages suivants : Compatibilité Windows XP SP2, Exécuter en tant qu'administrateur, Désactiver les optimisations du mode plein écran. 

![](/images/eviltwin_properties.png)

Vous pouvez désormais lancer le jeu, mais il ne pourra dépasser la résolution 1024x768 ni reconnaître votre manette.

## Utiliser une manette

À moins que vous ayez une manette analogique des années 2000 comme la Guillemot Dual Analog, le jeu ne reconnaîtra pas votre gamepad. Et personne ne veut jouer à ce jeu au clavier.

Heureusement il existe un super utilitaire nommé [Xidi sur Github](https://github.com/samuelgr/Xidi/releases/tag/v4.2.0). Une fois télécharger, glisser les fichiers dinput.dll, dinput8.dll et winmm.dll dans le répertoire du jeu.

Et c'est tout ! Lancez SuperPadCfg.exe puis configurer votre gamepad.

### Améliorer la résolution.

Par défaut vous ne pouvez dépasser la résolution de 1024 x 768. Cependant avec [le wrapper dgVoodoo2](http://dege.freeweb.hu/dgVoodoo2/dgVoodoo2/) c'est possible ! Une fois téléchargé, copiez les fichiers contenu dans le répertoire MS/x86 (DDraw.dll, D3DImm.dll, D3D8.dll, D3D9.dll).

Copiez ensuite l'application dgVoodooCpl.exe dans le répertoire du jeu. Lancez-le avec les droits administrateurs.

Dans l'onglet DirectX vous pouvez choisir la résolution qui vous convient ainsi que l'anti-aliasing.

![](/images/eviltwin_dgvoodoo.png)

Sauvegardez, quittez. Un fichier nommé dgVoodoo.conf se trouver désormais dans le répertoire d'Evil Twin.

Désormais, quans vous lancerez le jeu, il aura la résolution indiquée dans dgVoodoo.

-------

Le readme recommande les manettes suivantes : 

- Microsoft Sidewinder 3D PRO

- Thrustmaster Fusion

- InterAct PC PowerPad Pro

- MadCatz-Panther XL

- Guillemot Dual Analog

- Interact MakoPad