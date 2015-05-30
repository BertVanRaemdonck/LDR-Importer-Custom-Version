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
* Bevels on bricks (This requires an extra script compared to the original: "bevel_shader.oso", that you need to place in the same directory as the importer script!)
* Optional LEGO logo on the studs (this requires the "logo3.dat" file in your LDraw parts library)
