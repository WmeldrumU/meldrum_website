---
title: WebGL Raytracer
image: /assets/images/RayTracer.png
description: Software-based raytracing program that can run on any web browser. User can interact with camera, lighting, and scene objects as well as toggle between rasterization, raytracing, or hybrid rendering.
date: 2021-05-31
layout: post
---


**Software-based raytracing program that can run on any web browser. User can interact with camera, lighting, and scene objects as well as toggle between rasterization, raytracing, or hybrid rendering.** 

Project for CS 4600 (Intro to Computer Graphics). Not only was this a lesson in ray tracing, but deffered rendering as well. As some of you may know, OpenGL does not support ray tracing. Because of this, you have to "hack" the graphics pipeline by drawing a quad or tri over the camera viewport and implementing ray tracing through the fragment shader. 

A cool feature of this project was that it still had rasterization capability -- and could even combine the two (rays for reflection, rasterization for the rest). Of course, this project supports full ray-based rendering as well.

Line-sphere intersections are the bread and butter of this project. One way of doing so is by substituting the equation of a ray into the implicit function/equation of a sphere. After lot of algebra, we end up with a qudratic equation and solve for our missing term which tells us if/where intersections take place! I highly recommending checking out either of these for more on ray-sphere intersections:

- [Scratchapixel ray-sphere intersections](https://www.scratchapixel.com/lessons/3d-basic-rendering/minimal-ray-tracer-rendering-simple-shapes/ray-sphere-intersection)

- [Wikipedia ray-sphere intersection](https://en.wikipedia.org/wiki/Line%E2%80%93sphere_intersection)


