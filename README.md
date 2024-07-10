# Dinamic-cube
The dynamic cube I created in the C++ programming language consists of 4 smaller cubes that merge into 1 larger cube and can be separated again. This was developed as an independent project as part of the Computer Graphics course

- Textures for wood, toy box, and brick wall borrowed from exercise materials, while other textures were generated using the tool: https://cpetry.github.io/NormalMap-Online/ from black and white images found online or manually created images.
- The scene consists of 8 cubes of different colors with normal mapping that move away from their initial positions upon pressing a key, hold for a while, and then return.
- The path of each cube is represented by an object from the Path structure, which contains the starting and ending points of each cube and a function that returns a point on the path based on the parameter t within the interval [0, 1].
- Position interpolation uses the cubic_hermite function with parameter t to achieve acceleration and deceleration effects (https://registry.khronos.org/OpenGL-Refpages/gl4/html/smoothstep.xhtml).
- An additional structure Cube combines the texture used for normal mapping, the cube's path, and its color.
- The set_cubes function sets normal map textures, colors, and paths for each cube.
- During execution, the camera and light rotate around the center of the scene in opposite directions.
- Functions, structures, and classes were adapted from exercise materials and modified as needed to function within the task requirements.

Application Controls:
- Pressing the S key initiates the cubes' animation.
- Pressing ESCAPE exits the application.
