[back to help index](Help)

If you need something special, that not exists in embedded collections, you can import custom images into fontello. We currently support 2 vector formats:

1. SVG fonts.
2. SVG images.

Usually, other vector formats can be converted to SVG.


## Importing font

If your font is in TTF / OTF / WOFF format, use [FontForge](http://fontforge.org) or something like this to convert font to SVG format. In FontForge do the following:

1. Open your font via `File > Open` menu.
2. Then, in `File > Create fonts...` menu select `SVG` format and save file.
3. Drag and drop SVG file to fontello page.


## Importing SVG images

You should understand that font formats do not support all of the features that the SVG format provides. Though we try to automate the import process, sometimes it's necessary to make adjustments to artwork in order to achieve the desired result.

Here are our recommendations:

1. Remove all fills and colors. You can probably leave black fills. In fonts, fill is defined by contour direction.  Make sure that you don't have any complex rules like `evenodd` fills.
2. Remove all FAT line attributes. This is not supported by Fontello. In fonts, fat lines are drown by 2 nested contours.
3. Join all contours to a single outline. This is the last and the most important step. Usually editors automatically set the correct contour direction depending on nesting and black fills.

## Online solution

You can use this website : https://jakearchibald.github.io/svgomg/


__Troubleshooting.__

If you see, that contour is missed after import, or have inversed fill:

1. Check that SVG contours were joined prior to import.
2. Try to reverse direction of missed contours.

### Preparing images in Inkscape

You may need to do some additional simplification of your drawing, such converting objects and strokes to paths (see the Path menu), in addition to the below. You can check the svg file output in a text editor - if it has worked correctly, you should see a single `<path>` element and an empty `<defs>` element.

1. Select all
2. Object -> Ungroup
3. Path -> Union
4. Path -> Combine paths
5. File -> Vacuum Defs
6. Save as -> Plain SVG

### Preparing images in Adobe illustrator

Make sure that you have merged your vectors together into a compound path.  This is done by selecting all the paths in your glyph and using "Object > Compound Path > Make".  If you've already grouped them into a binary group you'll need to expand it first.

Once you have a single compound path you'll do a "File > Save As", select SVG from the drop-down, and hit save.  You'll want to use the default "SVG 1.1" file format.

(Note: there are some issues with preserving the entire artboard - the "Save As" appears to trim the artboard to the shortest dimension.  Haven't found an effective way to remedy this so we're working around it in CSS.)

(Note2: Illustrator seem to have some problems with the artboard size and Save As... SVG. The solution : create a new perfect square document about 500px, copy and past your artwork, save in SVG. And now, each time you open an SVG file, **the artboard keep the latest artboard dimension.** You could center correctly your artwork in this artboard, and save again )

One trick that may work is to include a rectangle of size 1000x1000 in the Illustrator document, locked with no fill or stroke colour. This will be exported in the SVG, enforcing a minimum size. However, as it's a `rect` rather than a `path`, Fontello will ignore it with a warning message, "Skipped tags and attributes: rect".

## Drawing image from scratch

1. We recommend to set height to 1000px and crop width to visible part. Though, fontello automatically rescale image from any size, we don't recommend use very small dimensions, because that can affect precision.
2. Usually, image should be aligned  text baseline, or text middle line. By default, fontello set baseline to 15% from bottom (you can change this). So, if you need to allign you icon by baseline - set it's bottom to 15% from paper bottom. And if you wish to align it by middle line - just center it visually on paper.
3. If you wish to show image in small size, try to draw it "pixel perfect". Here is [wonderful article](https://github.com/blog/1135-the-making-of-octicons) about.