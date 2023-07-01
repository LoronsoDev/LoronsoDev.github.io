---
title: "Galaxy Forces"
tags: ["Personal project"]
date: 45
languages: ["C#"]
engines: ["Unity"]
#showSummary: true
draft: false
---

{{< youtube EZgih4_2SQw >}}

<span></span>

{{< alert icon="download">}}
This game is playable on [itch.io](https://loronso.itch.io/galaxy-forces)
{{< /alert >}}

<span></span>

{{< button href="https://loronso.itch.io/fade" target="_blank" >}}
Try this game!
{{< /button >}}

## What is GALAXY FORCES?
Galaxy Forces was a video game created for a degree assignment. It got out ouf hand for me, as I was really liking the smoothness of the gameplay, so I spent much, much longer than needed polishing it up and creating a fun product to play.

The game is designed to be played with joysticks, but it also supports virtual mobile joysticks and keyboard. Due to the nature of the gameplay, using keyboard is the least preferred option.

The goal of the game is to finish in the least amount of time possible, killing the most enemies possible throughout the play. The score system is designed to reflect it, giving more score if you go faster.

An obvious inspiration for this game is Starfox (Nintendo).

## My role in GALAXY FORCES

I made all the code related parts of this project alone (gameplay, UI, tools...), using Unity. All art excluding the spaceship is bought from the Unity Asset Store. The spaceship was modelled by a colleague.

## What am I proud of developing here?

I especially liked how the feeling turned out. I experimented a lot with feedback and FX. To give the player a good sense of speed, I spawned particles all around the camera, speeding them up when the user went faster and increased the FOV dramatically. I also experimented with postprocess in this regard, adding things like blur and chromatic aberration when going faster.

Adding the crosshair was also a really tricky part, as representing 3D spaces in a 2D space (screen space) while also giving the user the sense of control is very tricky. I ended up drawing a virtual line from the tip of the spaceship to the usual attack length, taking that position and translating it to the screen space, drawing the crosshair there. It felt really good.

A good challengue here was performance too, as spawning a big number of enemies, with their own logic and with the ability to spawn bullets was giving a good toll on performance. I ended up going around this by hiding all enemies that were occluded by any of the geometry or that were behind the player (dot(player, enemy) < 0). I also pooled all spawnable objects and enemies, so I didn't need to allocate memory every time I needed to instantiate one of them, and also avoiding the performance hit of destroying gameobjects by only disabling and reusing them.