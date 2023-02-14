# Godot4TerrainShader
Split texture, stochastic sampled, triplanar texture shader for Godot4

![An example screenshot of the terrain shader](https://github.com/acegiak/Godot4TerrainShader/raw/main/screenshots/terrainshader.png)

Based on:
 * [/u/Rotoscope](https://www.reddit.com/user/rotoscope-/)'s [Stochastic Sampling Shader for Unity](https://www.reddit.com/r/Unity3D/comments/dhr5g2/i_made_a_stochastic_texture_sampling_shader/)
 * [John Watson](https://twitter.com/yafd)'s [Split Triplanar Terrain Shader for Godot3](https://github.com/jotson/godot3-triplanar-terrain-demo)


## How To Use:
 * Unzip the folder into your project so that the terrain-shader folder is in your addons folder.
 * Create a Shader Material and use Terrain.gdshader as the shader.
 * Set shader parameters:
    * set wall_tex_scale and top_tex_scale to be larger than zero.
    * set wall_color and top_color to be lighter than black (eg middle grey)
    * assign textures to wall_tex and top_tex
    * adjust blend values (2,0,0,1 are good starting values) (These just have to be played with and adjusted to your taste)

There's also an example material in the example folder

![](https://github.com/acegiak/Godot4TerrainShader/raw/main/screenshots/shader_use_example.gif)