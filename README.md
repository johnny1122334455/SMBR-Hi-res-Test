# SMBR-Hi-res-Test
Testing out adding higher res sprites to SMBR

Original project located at https://github.com/JHDev2006/Super-Mario-Bros.-Remastered-Public/wiki

This is an attempt to get higher res sprites working in the game. I've made some changes to the source code to allow handling of larger resolution images. It should be possible to create higher reslution objects for several sprites including characters, enemies, and some blocks. So far, any block or background object that is part of a tile set is not working, and additionally I was having trouble getting the goomba character to work with a higher resolution sprite sheet.

There may also be some characters that don't look right. This is because every character that does not use a 32x32 tile has to be adjusteed in the source code with this method. I adjusted all of them that I could find, but there could be more still. I only played through SMB1 to test that nothing looked off; lost levels, ANN, or custom levels may expose some more characters that need touch ups. I'll try and work on these as I find them.

To make a hi-res resource, create a new resource pack as you normally would. Use an image editor to resize any of the .png images and edit them as desired. Make sure to update the .json for the affected characters, multiplying the frame properties and rect properties to account for your new resolution. The game should be able to handle any resoluition multiplier, I've texted with 4x and 5x resolution.
