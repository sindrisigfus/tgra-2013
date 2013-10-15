# Lab assignment 8
This document contains the eight lab assignment in the course T-511-TGRA.
## Texture mapping in OpenGl

Start this exercise with the „Sphere, lights and Game mode example“ project found under *Other material*. Make it display a single cube and a single sphere, close to each other but not at the same spot. Also make the lights and materials white (1.0, 1.0, 1.0, 1.0) to start with. You can also find the textures needed for this assignment under *Other material* named Dice and earth texture. Unpack them into an asset folder within your project.

Texture mapping is simply the act of assigning 2D coordinates within a texture image to the 3D vertices of the polygons in our scene. The texture image can be a regular digital image file - .bmp, .jpg, etc.

	Gdx.gl11.glEnableClientState(GL11.GL_TEXTURE_COORD_ARRAY);










	Gdx.gl11.glDisableClientState(GL11.GL_TEXTURE_COORD_ARRAY);


You have to disable using the texture array because you only loaded 4 (s,t) coordinates into the texture array and thus can only use it when drawing the first 4 vertices in the vertex array.


