---
title: Space Wars
image: /assets/images/spacewarscropped.png
description: C# based multiplayer game capable of handling 60+ players at the same time. Developed while pair programming with MVC design. Required use of event-driven programming, C# delegates, and UI design/development. 
company: Another Company
date: 2021-05-26
layout: post
---


**C# based multiplayer game capable of handling 60+ players at the same time. Developed while pair programming with MVC design. Required use of event-driven programming, C# delegates, and UI design/development.**

Space Wars was an awesome group project between myself and my good friend, Andrew Thompson, for CS 3500 (Software Practice I). This is where I was first introduced to C# -- let alone concepts like delegates and model-view-controller architecture. I was surprised to see how even a simple game like this can be used to simulate phyics with Newton's second law (force = mass * acceleration). The ships and even their projectiles had mass, momentum, and friction. Even the suns in this game had gravitational pull on the physics objects. The networking portion was its own beast as well. We had to create a client and server separately, with the server handling inputs sent from the client and updating the game model, propogating it out to the players to prevent client-side tampering. 

<img src="/assets/images/space-wars-img.png">