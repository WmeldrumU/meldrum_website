---
title: Volumetric Lighting
image: /assets/images/Volumetric.png
description: From-scratch renderrer, written in C++ 14 with OpenGL 4.4. The renderrer takes in .obj files and parses the textures, materials, and vertex data, displaying them in a deferred rending-based blinn-phong shading. Rays are then cast from screen space to render crepuscular beams (god rays) which interact with the scene. 
company: Another Company
date: 2022-05-31
layout: post
---


**From-scratch renderrer, written in C++ with OpenGL. The renderrer takes in .obj files and parses the textures, materials, and vertex data, displaying them in a deferred rending-based blinn-phong shading. Rays are then cast from screen space to render crepuscular beams (god rays) which interact with the scene.**


This was a final project for my Interactive Computer Graphics course. We were able to choose the subject of our final project. I started with fluid simulation, only to soon discover that thesis-sized amounts of worked would be required for such a task... though I do plan on getting back to fluid simulation. It's too interesting NOT to try.

*Anyway*, I then decided to focus on volumetrics -- specifically "god rays" and fog -- I wanted to understand how these amorphous objects were rendered. 

Often times, god rays will be rendered only in two dimensional space. The sources of light will be blurred outward and provide an *okay* result. This implementation doesn't give volume to the light, and a lightsource must be on screen for the light beams to be drawn. 

I decided to implement a ray-marching based approach. Rays are cast from the point of view into our scene and then the shader asks "okay, are we in view of the lightsource?" if so, the pixel color is altered and the ray "marches" to the next sampling point. 



<br>
<div class="video-container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/ZVCu2sMbm_I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
<br>