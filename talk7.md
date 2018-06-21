# Art with webgl

Max @maxbittker

- Webgl is : Programming the GPU
- don't program alone. Use a bundler
- bundlers work by following the module trail and making a graph. Then it concats and bundles them all together. 
- modules, code reuise, collaboration we all use these, causing a JS renaissance. 
- CPU is a processing unit
- GPU has 2000 or so. It's running many more instructions on parallel. But it's got a core restriction in that it's a lot less flexible. 
- GPUs deal with lots of small tasks, like handling pixel colors. You couldn't handle this much work on a CPU, that's what GPU exists for.
- A shader is a function that takes in coordinates, and outputs something like the color to display for that pixel. 
- GPUs can't run javascript. BUT
- GLSL Graphics Library Shading Language. Like C, but compiled to run on CPU. 
- When GLSL has to figure out which color something should be, it's more interesting. Shaders can split the pixel into two triangles. 
- This makes things easier, is you use more math and if statements. 
- Shadertoy.com is a site where people share shaders they wrote.
- lots of math, lots of loops. All in one file. 
- because numbers are passed around as pixel colors. Changing things around has really interesting visuals. 
- lots of low level helper functions. The tops of files are filled with helper functions people picked up along the way. 

## Perlin Noise
- algorithm for smooth randomness. Simulated natural shapes. 
- it takes a 2 dimensional space, x and y coordinates, and passes out a color. 
- complicated math about it might not be interesting to you, but you don't need to understand it to use it
- glslify is like browserify (a module system) for GLSL. 
- now you're able to import files/functions and start using them. 