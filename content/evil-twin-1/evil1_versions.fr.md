---
title: "Différences entre les versions"
author: "Zap' le Simple"
lang: fr
slug: versions
---

# Différences entre les versions

Développé à l'origine pour la Dreamcast, le jeu est finalement porté sur Windows et Playstation 2. Ces deux versions sont publiées fin 2001 puis en mars 2002 sort finalement la version Dreamcast après l'abandon de celle-ci par SEGA. Il s'agit d'un des tout derniers jeux publiés en Europe. La version US est annulée.

Du fait des importantes différences matériels entre les trois plateformes et malgré l'usage d'un moteur multi-plateforme, le jeu s'en retrouve plus ou moins légèrement tronqué d'un support à l'autre.

<div class="juxtapose" id="horizontal"></div>

## Dreamcast

Bien que cible première du développement, il s'agit au final de la version la plus amputé du jeu. Il lui manque deux niveaux : la zone de cuisson sur l'île de Jocelyn et l'infirmerie sur l'île de Stéphane. Les cinématiques n'ont également pas de fond musical lorsque les personnages parlent du fait du moteur [ne pouvant gérer deux sources audio simultanées](https://twitter.com/ocornut/status/1171361852313370625) ([backup](/images/ocornut-twitter.png)). Il y a moins de personnages (notamment des ennemis) du fait de la mémoire vive et la disposition des têtes de Lenny est également différente. Les textures sont elles aussi beaucoup plus compressées, notamment sur certains éléments secondaires. Probablement pour tenir sur les 1 Go du GD-ROM. Par contre elle brille par ses effets de lumière absents de la version Playstation 2. 

Étonnamment la côte actuelle du jeu est délirante alors qu'il se trouvait à 2 euros dans les bacs fin 2002.

<div class="juxtapose" id="horizontal2"></div>

## Playstation 2 & Windows

Les versions PS2 et Windows sont bien plus proches l'une de l'autre. Les textures sont quand même un peu plus fines sur Windows, et surtout cette dernière possède bien plus d'effets de lumière absents de la version Playstation 2. L'ensemble des ressources graphiques et sonores y sont optimales. L'avantage de la version PS2 est qu'elle est[ jouable immédiatement via PCSX2](evil1_playing.md). Sur Windows il faudra bidouiller pour lancer un jeu de vingt ans d'âge.

<div class="juxtapose" id="horizontal3"></div>

<link rel="stylesheet" href="/css/juxtapose.css" type="text/css" />
<script src="/js/juxtapose.min.js"></script>
<script>
     slider_horizontal = new juxtapose.JXSlider('#horizontal', [{
        src: '/images/juxtapose_dc.jpg',
        label: 'Dreamcast'
    }, {
        src: '/images/juxtapose_ps2.jpg',
        label: 'PS2'
    }], {
        animate: true,
        showLabels: true,
        showCredits: false,
        startingPosition: "45%",
        makeResponsive: true,
        mode: "horizontal"
    });
</script>
<script>
     slider_horizontal = new juxtapose.JXSlider('#horizontal2', [{
        src: '/images/juxtapose_dc_02.jpg',
        label: 'Dreamcast'
    }, {
        src: '/images/juxtapose_ps2_02.jpg',
        label: 'PS2'
    }], {
        animate: true,
        showLabels: true,
        showCredits: false,
        startingPosition: "45%",
        makeResponsive: true,
        mode: "horizontal"
    });
</script>
<script>
     slider_horizontal = new juxtapose.JXSlider('#horizontal3', [{
        src: '/images/EvilTwin_Juxtapose_Infirmerie_PC.jpg',
        label: 'Windows'
    }, {
        src: '/images/EvilTwin_Juxtapose_Infirmerie_PS2.jpg',
        label: 'PS2'
    }], {
        animate: true,
        showLabels: true,
        showCredits: false,
        startingPosition: "45%",
        makeResponsive: true,
        mode: "horizontal"
    });
</script>	