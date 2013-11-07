[back to help index](Help)

If you need something special, that not exists in embedded conllections, you can import custom images into fontello. We currently support 2 vertor formats:

1. SVG fonts.
2. SVG images.

Usually, other vector formats can be converted to SVG.


## Importing font

If your font is on TTF / OTF / WOFF format, use [FontForge](http://fontforge.org) or something like this to convert font to SVG format. In FontForge do the following:

1. Open your font via `File > Open` menu.
2. Then, in `File > Create fonts...` menu select `SVG` format and save file.
3. Drag and drop SVG file to fontello page.


## Importing SVG images

You should underatand, that SVG format is more rich, that can be sopported by fonts. Though we try to automate importing process, sometime it's more safe to prepare image in editor for exact result.

Here are our recommendations:

1. Remove all fills and colors. In fonts fill is defined by contour direction. Probablym you can leave black fills. Make sure, you don't have complex rules like `evenodd` fills.
2. Remove all FAT lines attributes. Those are not supported, anyway. In fonts, fat line is drown by 2 nested contours.
3. Join all coutours to single outline. That's the last and the most important step. Usually, editors automatically set right coutours direction, depandint on nesting and black fill.


__Troubleshooting.__

If you see, that coutour is missed after import, or have inversed fill:

1. Check that SVG coutours were joined prior to import.
2. Try to reverse direction of missed contours.

### Preparing images in Inskape

TBD.

### Preparing images in Adobe illustrator

TBD.


## Drawing image from scratch

1. We recommend to set height to 1000px and crop width to visible part. Though, fontello automatically rescale image from any size, we don't recomment use very small dimentions, because that can affect precision.
2. Usually, image should be alligned  text baseline, or text middle line. By default, fontello set baseline to 15% from bottom (you can change this). So, if you need to allign you icon by baseline - set it's bottom to 15% from paper bottom. And if you wish to allign it by middle line - just center it visually on paper.
3. If you wish to shaw image in small size, try to draw it "pixel perfect". Here is [wonderful article](https://github.com/blog/1135-the-making-of-octicons) about.
