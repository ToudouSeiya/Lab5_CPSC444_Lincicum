# WebGL Lighting Lab

## Overview

This lab introduces the fundamental concepts of lighting in computer graphics using WebGL. Students will explore how lighting calculations affect the appearance of a 3D object by modifying shaders and JavaScript code.

The lab begins with a working rotating cube and guides students through a series of lighting experiments involving:

- Ambient Lighting
- Diffuse Lighting
- Light Direction
- Colored Lighting
- Animated Lighting

Students will gain hands-on experience with shader programming and learn how modern graphics engines simulate light.

---

## Learning Objectives

By the end of this lab, students will be able to:

- Explain the purpose of lighting in 3D graphics.
- Describe the difference between ambient and diffuse lighting.
- Modify GLSL shaders.
- Change light direction using JavaScript uniforms.
- Create colored light sources.
- Animate a light source around a 3D object.
- Understand the role of surface normals in lighting calculations.

---

## Project Structure

```text
WebGLLightingLab/
│
├── lighting.html
├── lighting.js
├── vertexShader.glsl
├── fragmentShader.glsl
│
└── Common/
```

## Reflection Questions
### 1. What is ambient lighting?
Ambient lighting is the general lighting in a scene that all of the shapes are lit by. When the ambient light is set to 0, the sides of the cube not illuminted by any other light are completely black and invisible against the background. When it is set to 1, the entire cube is white and the individual faces aren't distinguishable. When it is set in between, the cube has brighter faces where lit by both the ambient light and another light and darker faces where it is just ambient light. The higher the number, the brighter all faces.
### 2. What is diffuse lighting?
Diffuse lighting is direction-based lighting. The direction of the diffuse light determines which faces will be lit up by it.
### 3. Why do we need normal vectors?
The normal vectors represent the surfaces of the cube and are what get multiplied by the ambient and diffuse light to properly show the light. The normals determine whether the cube is lit on the outside or the inside. 
### 4. What role does the dot product play in lighting calculations?
The dot product is used in addition to the light direction of the diffuse light to change the brightness/color of a face depending on if it is being hit by the diffuse light or not.
### 5. How does changing light direction affect a 3D object?
Depending on the light direction, different faces of the object will be lit or not. When the light shines from the left, the leftmost face will be brightest and the rightmost will be darkest, etc.
### 6. How does changing light color affect realism?
Colors such as white light, blueish and yellowish light are the most realistic, while others look more unrealistic or like they'd be in an unnatural situation like a concert. 
### 7. Which modification produced the most interesting result?
I found the moving light was the most interesting result. The combination of the moving light and the rotating cube created an interesting pattern of faces becoming lit and unlit by the diffuse light. 
### 8. Why do game engines automate lighting calculations?
Lighting calculations use some complex math, and the exact values can make a big difference. Having preset equations/values can make the process faster and easier. 
