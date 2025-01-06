---
title: "Versions comparison"
author: "Zap' le Simple"
lang: en
slug: versions
---

# Versions comparison

Dreamcast was the first target for Evil Twin's production. But In Utero used their middleware Phoenix3D to work simultaneously for the Playstation 2 & Windows PC version.

However, there are a few differences between them. 

<div class="juxtapose" id="horizontal"></div>

## Dreamcast

On Dreamcast, the game suffer from two missing levels and a higher texture compression. During ingame cinematics, [voices acting cuts the soundtrack](https://twitter.com/ocornut/status/1171361852313370625). Due to memory issue there is also less NPC. However lighting effects are quite good. Better than de PS2 version.

Whereas the game used to cost nothing in 2002/2003, it's now an expensive dreamcast game.

<div class="juxtapose" id="horizontal2"></div>

## Playstation 2 & Windows

Windows & PS2 versions are almost the same. Even if the texture compression is less destructive on PC. The main difference are the lighting effects. There is almost nothing on PS2.

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