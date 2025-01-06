---
title: "Play Evil Twin on Windows 10"
author: "Zap' le Simple"
lang: en
slug: evil-twin-on-modern-windows
---

# Play Evil Twin on Windows 10 

Here is a quick tutorial to play Evil Twin on Windows 10 with a modern controller and a decent resolution (better than 1024x768).

## Install the game & configure executables

- Install the game from the original discs or disk images via WinCDEmu.
- Download and install [update1](/files/) so the game can be launched from Windows XP and above.
- Download and install the [no-CD](/files/) because Windows 10 dropped DRM support.
- Change executables configs from EvilTwin.exe, Video.exe, Splash.exe and SuperPadCfg.exe with Windows XP SP2 compatibility mode, execute as admin and remove full screen optimisations.

![exe properties](/images/eviltwin_properties.png)

Now the game can be launched. But you will miss modern controller support and a better resolution than 1024x768.

## Use a modern controller

Maybe you still have an old Guillemot Dual Analog controller. But you probably use a Xbox or Dualshock controller and they are not recognized by the program. And there is no way you want to play Evil Twin on a keyboard.

Fortunately, there is a tool that you can download, it's [Xidi on Github](https://github.com/samuelgr/Xidi/releases/tag/v4.2.0). Download it and move dinput.dll, dinput8.dll and winmm.dll to the game folder.

That's all! Launch SuperPadCfg.exe and configure the controller.

## High resolution

The game is locked to a maximum of 1024x768. But with the [wrapper dgVoodoo2](http://dege.freeweb.hu/dgVoodoo2/dgVoodoo2/) you will be able to unlock that. And also add some anisotropic and MSAA stuffs.

From the MS/x86 dgVoodoo folder, move DDraw.dll, D3DImm.dll, D3D8.dll, D3D9.dll to the game folder. Copy also dgVoodooCpl.exe in the same directory. Now launch the exe with admin privileges.

In the DirectX tab, there is many options to update the graphic rendition (except widescreen)

![Config screen](/images/eviltwin_dgvoodoo.png)

Save & quit. A file called dgVoodoo.conf is now located next to the program. Next time you will launch the game, the resolution will be given by dgVoodoo.

---

The original readme file recommends theses controllers :

- Microsoft Sidewinder 3D PRO
- Thrustmaster Fusion
- InterAct PC PowerPad Pro
- MadCatz-Panther XL
- Guillemot Dual Analog
- Interact MakoPad