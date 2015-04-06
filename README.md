# Unity3d-Sprites-Opaque-Shader
Unity3D doesn't come with a shader for opaque sprites. The Sprites-Default shader always render sprites by calculating transparency, regardless if your sprite is transparent or not. A simple test showed that my opaque sprite shader is 30% faster than the default sprite shader. The test was made with only one sprite. I believe the performance gain is much greater than 30% in cases where you would have several layers of sprites.  

I'm really not good with shaders so I just modified the Sprites-Default shader. Feel free to contribute if you can optimize this further.

To use this, create a material and select the shader named Opaque under Sprites. When using sprites, select the newly created material instead of the default one.

This is only ment for Unity 4.x. Untested on Unity 5.
