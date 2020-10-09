# Wireframe Shader Graph
A simple Shader Graph implementation of a wireframe effect.

![Wireframe effect in action](https://github.com/ArturoNereu/WireframeShaderGraph/blob/main/Turntable_01.gif)

Based on this tutorial by Catlike Coding: https://catlikecoding.com/unity/tutorials/advanced-rendering/flat-and-wireframe-shading/

It involves two steps:

- Making sure the mesh doesn't share vertices and that each vertex has a color assigned(RGB).
- Executing the shader to see how far we are from the edges of the triangle to either paint a pixel or leave it transparent.

Shader Graph doesn't provide support for Geometry Shaders, we could use a code node as [GameDevBill explains here](https://gamedevbill.com/geometry-shaders-in-urp/) but for simplicity, we didn't.

Note: the shader graph is by no means optimized, it is just intended to show an approach of having a wireframe effect in a game. But you can use it as a starting point and tweak it from there.
