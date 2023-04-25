---
title: "G!RO"
tags: ["Personal project"]
date: 100 #Use as "importance" to show on recent
languages: ["C#"]
engines: ["Unity"]
#showSummary: true
draft: false

---

{{< youtube si6tVLTcYVo >}}

<span></span>

{{< alert icon="download">}}
This game is playable on [itch.io](https://negone.itch.io/giro)
{{< /alert >}}

<span></span>

{{< button href="https://negone.itch.io/giro" target="_blank" >}}
Try this game!
{{< /button >}}

## What is G!RO?
As last year students, some of my classmates and I decided to create small, addictive mobile games so we could iterate easily and test different concepts. We tried several prototypes with the idea of having only the "tapping" input available. G!RO is the result of one of those prototypes.

In G!RO you are in control of a spaceship that has lost one of its motors and spins endlessly while trapped in an unknown planet. Your role is to survive for as long as possible using your main weapon for movement and defense.

## My role in G!RO
 - As we started testing different concepts, we needed tools to iterate fast. I was in charge of researching the most commonly used features of hypercasual games, designing and developing an in-engine tool that provided most of the implementations hypercasual-arcade games for mobile usually need, while being fully customizable. The tool is fully interchangeable between different games, supports 2D and 3D and only requires minimum configuration to work. This means:
    - Menu functionality (responsive, provided default menus and means to customize them).
    - Store
    - Player selection
    - Inventories
    - Ads and IAPs (In-App purchases)
    - Several minor implementations (volume buttons, basic graphical quality settings)
    - Hard & soft currency
    - Hooks menu<->game so all the developer had to do was listen to specific events (e.g. starting the game)
    - Saving/Loading locally (playerprefs, encrypted/unencrypted JSON)
- Improving gameplay feedback:
    - Dynamically displaying current user weapon charge, limiting UI and implementing it into the game design.
    - Screen shake
- Creating a procedural world different for each playthrough
- Implementing different biomes made by the artists
- Implementing different spaceship types/weapons
- Optimizing game world so the game could be played in low-end games
- Bug fixing

 #### Honorable mentions
 - Awarded "Most enjoyable game" @ Indie Burger Awards, hosted at BIG, formerly Fun&Serious Bilbao
 - Nomination for "Best old school arcade game" @ Indie Burger Awards, hosted at BIG, formerly Fun&Serious Bilbao
