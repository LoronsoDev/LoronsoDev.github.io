---
title: "Sample post!"
tags: ["Tutorial"]
date: 50
#languages: ["C++", "SDL2", "Assimp"]
#engines: ["Sample"]
#externalUrl: ""
#showSummary: true
draft: false
---

## What is this engine?
Since I started making games, I've been deeply intrigued in the inner workings of more commercial engines. This was my first iteration of a game engine.

It supports 2D and 3D graphics using SDL2 for 2D and CPU rendering for 3D. The engine supports physics via a implementation of Box2D (2D) and Bullet Physics (3D).

The engine is built around an ECS (Entity-Component-System) architecture.

{{< github repo="loronsodev/GameEngine2" >}}

## Why do I consider this project important?
This project set my stepping stone to larger projects involving graphics and general game engine programming. It sparked enough curiosity in me to continue studying code architecture, computer graphics and proper GPU APIs like OpenGL or Vulkan.

## Why did I stop working on it?
At a point in its development, the engine needed reflection so I could translate the custom scene files into scenes that could be generated at runtime. I considered that instead of trying to implement it, I could just stop the work there, document everything clearly and use it for future reference in other engines if needed. I started working in this engine as a newbie with C++, so I feared that if I started implementing my own custom C++ reflection or any other reflection API, the engine could become so convoluted that I would no longer be able to maintain it properly. I preferred to have a working build that could be used by me or others for learning and start a new project from scratch using what I learnt while building this engine.