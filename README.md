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
Ambient lighting is the general lighting in a scene that all of the shapes are lit by. When the ambient light is set to 0, the sides of the cube not illuminted by any other light are completely black and invisible against the background. When it is set to 1, the entire cube is white and the individual faces aren''t distinguishable. When it is set in between, the cube has brighter faces where lit by both the ambient light and another light and darker faces where it is just ambient light. The higher the number, the brighter all faces.
 
