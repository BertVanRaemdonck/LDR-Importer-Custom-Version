# LDR Importer - Custom Version#

[![Build Status](https://travis-ci.org/le717/LDR-Importer.svg?branch=master)](https://travis-ci.org/le717/LDR-Importer)

A [Blender 3D](http://www.blender.org) Importer script for the [LDraw Parts Library](http://www.ldraw.org).

> LDraw&trade; is an open standard for LEGO CAD programs that allow the user to create virtual LEGO models and scenes. You can use it to document models
you have physically built, create building instructions just like LEGO, render 3D photo realistic images of your virtual models and even make animations.
The possibilities are endless. Unlike real LEGO bricks where you are limited by the number of parts and colors, in LDraw nothing is impossible.

# Purpose #

The purpose of the **LDR Importer** is to import LDraw and LDraw compatible parts and models into Blender as they should be (including proper mesh and materials). However, options to improve the import, such as cleaning up said mesh and other features, are available at the user's disposal. Other options, such as photo-realism, are left to the user to perform.

______________________________________________

This is a copy of the [LDR Importer](https://github.com/le717/LDR-Importer) project here on GitHub. I edited some files, however, to add some extra features. They
* Fixed colors through a gamma node
* Slope textures on selected slope bricks (you can always edit the dictionary)
* Fixed a bug that made all materials basic
* Fixed the gap feature to produce uniform gaps
* More realistic Pearl Metal materials
* Bevels on bricks (This requires an extra script compared to the original: see note below)
* Optional LEGO logo on the studs (this requires the "logo3.dat" file in your LDraw parts library)

# Important Note #

In order to get the program to work, you'll need the "bevel_shader.osl" file included in this project. I configured the program to look for the "bevel_shade.oso" file in the same directory as the script however. This is due to the fact that the .osl file has to be compiled everytime by Blender, and since the script is in my C folder, it would ask for permission all the time. The problem is that this .oso file is different on every computer. So to set this up correctly, please follow the following steps:
* Open Blender, giving it administrator rights.
* Open a new scene in Blender, select a random object with a material and open the node editor for the material.
* Add in a script node, select 'External' and set the path to the bevel_shader.osl file, which should be located in the same folder as your "import_ldraw" file. Then, compile the script (the 'refresh' arrows)
* Now check that folder. It should have the "bevel_shader.oso" file in it now. Now you can begin to use my version of the LDR Importer.
