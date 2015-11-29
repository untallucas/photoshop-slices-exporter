#Photoshop Slices Exporter

Photoshop's **Save for Web** has an arbitrary limit of **8192 pixels**. No image dimension can go above that number of pixels, and when you need to work with a larger file, it's a pain in the ass. 

The workarounds I've found implies to crop and create a new file for every slice I want to export (sometimes I have up to 30 in a single file), or to crop my master file into smaller pieces (nonsense!).

None of these are handy solutions for my workflow, so I decided to do this script that **treats certain layers as slices, cropping and exporting an image for each one**.

#####USAGE
- Create a new **layer group**.
- Inside that layer group, create a **new layer** for each slice you want to export.
- In each one of these layers, **fill the area** that you want to crop and export (any color or content will do the trick).
- Remember to leave visible just the layers you want to export.
- Run the script.

#####THE SCRIPT WILL
- Ask for input (slices layer group name, export file name setup)
- Recognice the layer group where the "slices" are stored.
- Choose one of the layers.
- Make a selection from the layer.
- Crop the document to the layer size.
- Export the resulting image as a transparent background PNG.
- Back History to the start point.
- Go on with the next layer.

This has been **very** helpful in my workflow, hope you can use it too.

Tested only in CS6, on OSX.

Programming scripts it's not my main task, but feedback to improve this one in the future is welcome.
