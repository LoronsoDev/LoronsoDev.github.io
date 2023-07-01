---
title: "Alien Agent"
tags: ["Personal project", "VR"]
date: 99 #Use as "importance" to show on recent
languages: ["C#"]
engines: ["Unity"]
#showSummary: true
draft: false

---

{{< youtube 6PzJBLhjcZA >}}

<span></span>

{{< alert >}}
This game is made for Pico 4 VR headsets using the OpenXR standard
{{< /alert >}}

<span></span>

## What is Alien Agent?
Alien Agent is a short game set in an alternate universe future, where you're in the boots of a soldier, in a future where the army is made up of ordinary people controlling robots fighting in distant conflicts.

## My role in Alien Agent
The whole experience has been designed & developed by me, using bought art assets from Sinty Studios. However, some highlights are:

- Created a flow for iterating faster with Pico 4 headsets, as they were quite new at the moment and development tools were rough.

- Designed the levels, minigames and the whole experience.

- Implemented diegetic menus and interfaces.

- Implemented virtual hands that reproduce the player's hand movements by retrieving the Pico button states and animating the ingame hands accordingly.

- Added physics support so players can interact with their environment without the need of explicitly grabbing the items.

- Supported wearables, like hats or bracelets.

- Created custom shaders to better differentiate certain parts of the experience.

- Implemented double handed weapons and their behaviour.

- Modified render pipeline so certain things could be supported, this was specially useful for 3D tutorials like arrows indicating the next steps. This modifications allowed for the custom shaders to be rendered through any object, so the user could see their next step at any moment just by looking around.

- Animated certain parts of the experience to achieve better feedback for the end user and increase immersion.