# Protocols
A collection of open protocols we have developed:

1. [Pseudocoloring Multispectral Images from the LaVision Multiphoton Microscope](https://github.com/TherapeuticsResearchCentre/Protocols/blob/master/README.md#pseudocoloring-multispectral-images-from-the-lavision-multiphoton-microscope)

## Pseudocoloring Multispectral Images from the LaVision Multiphoton Microscope

+ The goal is to create pseudocolored images at a consistent brightness and contrast that can be compared between imaged samples
+ Also, we want to create a merged pseudocolored image.

### Dependencies

1. [Fiji](http://fiji.sc/Fiji) - don't worry, it's free and open source and won't cost you anything!

### Brightness and Contract Settings

1. Channel 1 (C3; Red):	300-1500
2. Channel 2 (C1; Green): 0-8000
2. Channel 3 (C0; Blue): 400-1000

### Protocol

1. Open up Fiji and ensure that it's up to date!
2. Open each channel image ('File -> Open' or `Ctrl-O`.
  + Images saved by the LaVision (if exported to a Tif file that is) will have the following extension: `yourfile.ome.tif`
  + If you have images recorded simulatenously across multiple detectors (i.e. a multi-spectral image), each detector will have it's own tif file. The naming structure looks like this: `yourfile_C1.ome.tif`, `yourfile_C2.ome.tif` and so on, where `C#` refers to the number (#) of channels. 
  + You need to open all the channel images!
3. After you've opened all the channel images,  we want to merge them into composite image (composite just means that it's handled as 1 file, but it has the multiple channels in the 1 file). To do this: 
  1. Select from the menu: 'Images -> Color -> Merge channels':
  2. Assign the file names to the colors you desire. In this case, I set `C0` to blue, `C1` to green, and `C3` to red.
  3. Ensure the 'Create Composite' is checked
  4. Press 'Ok'
  5. <img src="http://s25.postimg.org/j5e0rep5b/Merge_Channels.png"/>
4. Go to 'Images -> Color' and open: Color Channels
5. Go to 'Images -> Adjust' and open: Brightness & Contrast
6. In the 'Channels' dialog box, select 'Color' from the pull down menu
7. Select 'Channel 1', press 'Set', and enter the 'Minimum' and 'Maximum' displayed values as indicated above. Don't check anything else in that dialog. Do the same for the other channels.
8. Now we want to save each channel as it's own pseudocolored image. Select from the menu 'Image -> Type -> 
