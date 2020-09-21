                                          Console-Graphics
                                          a.k.a Hello World
                                          =================

**If you are having trouble building this, you can just download a build at                                           <https://www.dropbox.com/sh/pjt2f0hs50iag4j/AAAvBZhCsbmRVUQFwSr5NA9ua?dl=0>**
[![Run on Repl.it](https://repl.it/badge/github/interl0per/Console-Graphics)](https://repl.it/github/interl0per/Console-Graphics)

A full blown 3D graphics engine that runs in the windows command prompt. 
3D objects are rendered in real-time as monochromatic ASCII art.

Right now, you can only load one .obj file at a time. 

## Before running

Set the command prompt's font size to 6 pt. Lucida Console works well.

## Features

 - 3D Wireframe/solid rendering. Solid rendering done with rasterizer. Z buffer for solid rendering, but it's messed up a little.

 - Load meshes from .obj files. Sample .obj is included.

 - Mesh transformations - rotations around x/y/z axis done.

 - Texture mapping. I used barycentric interpolation to do this. Multiple materials/mesh.

 - Lighting: Simple flat shading.

 - User input runs on another thread.

## User Input

After the model has loaded, press Return (the model will start to flicker)

 - Use `WASD` translate meshes
 - Use `R,T,Y` to rotate them
 - Press `Space` to change the rendering mode

## Bugs

 - Problems with using multiple materials per mesh
 - zBuffer isn't quite right
