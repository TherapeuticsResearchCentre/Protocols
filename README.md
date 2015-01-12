# Protocols
A collection of open protocols we have developed:

1. Pseudocoloring Multispectral Images from the LaVision Multiphoton Microscope

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

1. Open each channel image and color merge as above (Images -> Color -> Merge channels)
  + Ensure the 'Create Composite' is checked
2. Go to 'Images -> Color' and open: Color Channels
3. Go to 'Images -> Adjust' and open: Brightness & Contrast
4. In the 'Channels' dialog box, select 'Color' from the pull down menu
5. Select 'Channel 1', press 'Set', and enter the 'Minimum' and 'Maximum' displayed values as indicated above. Don't check anything else in that dialog. Do the same for the other channels.
6. Now we want to save each channel as it's own pseudocolored image. Select from the menu 'Image -> Type -> 
