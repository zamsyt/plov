# plov
Tool for managing image overlays for r/place

`plov` flattens the list of images in layers.txt to a single PNG, and converts the image to the 3:1 overlay format. Returns as overlay.png

layers.txt is a newline separated list of PNGs. Add "x " in the beginning of a line to omit the layer. Example:

```
layer1.png
layer2.png
x omitted.png
layer3.png
```

Sub-commands:

`flatten` - combines the images in layers.txt and returns in 1:1 format as flat.png

`explode <filename.png>` - Converts a 1:1 template image into the 3:1 overlay format

`crop` or `crop <filename.png>` - Crops an image (or the images in layers.txt) to remove empty space on the edges (for easy sharing of templates as images)
