---
title: "Giocare Evil Twin su Windows 10"
author: "Zap' le Simple"
lang: it
slug: giocare-evil-twin-su-windows-10
---

# Giocare Evil Twin su Windows 10

Ecco un veloce tutorial che spiega come giocare a Evil Twin su Windows 10, tramite un controller moderno e una risoluzione decente (migliore di 1024x768)

## Installare il gioco e configurare l'eseguibile



- Installa il gioco da un disco originale o da un'immagine disco via [WinCDEmu](https://github.com/sysprogs/WinCDEmu).

- Scarica e installa l'[update1](/files/), in questo modo puoi lanciare il gioco da Windows XP in su.

- Scarica e installa [no-CD](/files/), perché Windows 10 non supporta più il DRM.

- Configura gli eseguibili EvilTwin.exe, Video.exe, Splash.exe e SuperPadCfg.exe con la modalità di compatibilità denominata Windows XP SP2, in fine spunta su *Disabilita ottimizzazioni schermo intero* ed esegui come amministratore.

![](/images/eviltwin_properties.png)

Ora il gioco può essere lanciato, però manca il supporto agli odierni gamepad e una risoluzione migliore di 1024x768.

## Usare controller moderni

Forse hai ancora un vecchio Guillemot Dual Analog controller, ma probabilmente usi un gamepad Xbox o Dualshock ed essi non vengono riconosciuti da questo programma. Inoltre, non c'è modo di giocare a Evil twin con una tastiera.

Fortunatamente, esiste esiste uno strumento che fa al caso nostro, ossia [Xidi](https://github.com/samuelgr/Xidi). Scaricalo e sposta dinput.dll, dinput8.dll e winmm.dll nella cartella del gioco.

Tutto qui! Lancia SuperCfg.exe e configura il controller.

### Risoluzione elevata

Il gioco arriva al un massimo a 1024x768, però con il wrapper [dgVoodoo2](https://dege.freeweb.hu/dgVoodoo2/dgVoodoo2/#latest-stable-version) possiamo oltrepassare questo limite. Per di più, offre un filtro anisotropico e l'MSAA (un tipo di antialiasing).

Dalla cartealla MS/x86 di dgVoodoo spostate DDraw.dll, D3Dlmm.dll e D3D9.dll nella cartella del gioco. Copia nella medesima cartella anche dgVoodooCpl.exe ed eseguilo come aministratore.

Nella scheda DirectX ci sono diverse opzioni per aggiornare la grafica (eccetto il widescreen). Salva ed esci. Adesso nella cartella del gioco si trova un file chiamato dgVoodoo.conf. La prossima volta che avvierai il gioco, la risoluzione sarà data da questo wrapper.

![](/images/eviltwin_dgvoodoo.png)