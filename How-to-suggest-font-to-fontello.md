[back to help index](Help)

We don't refuse to add new open source fonts. The only serious requirement is an unobtrusive license, that doesn't force users to place links on their websites, write posts, tweet, pay money, limit use to non-commercial projects and so on. Also, we don't accept sample collections, used to promote paid full sets.

Please understand that we are developers; we can't program and add fonts at the same time. We need your help with preparing font info. If you just wish to inform us about something new, place a link to the new font on the [wiki page pending list](https://github.com/fontello/fontello/wiki#more-vector-sources). If you'd like for your font to be included more quickly, read the instructions below.

> We always welcome volunteer help! One way you can help is to choose a font from the pending list on [main wiki page](https://github.com/fontello/fontello/wiki#more-vector-sources) and prepare the font for inclusion in fontello.

_Note for authors_. We currently don't allow the download of separate images in vector format, we gently ask you to use a separate license for your images.

##### Recommended licenses are:

- [SIL](http://scripts.sil.org/OFL) for the font
- [CC BY](http://creativecommons.org/licenses/by/3.0/) or [CC BY-SA](http://creativecommons.org/licenses/by-sa/3.0/) for the images


## Requirements

- Acceptable open source license
- Icons should look good at small sizes
- 40+ icons
- Nice look

Last 2 requirements will be removed in the future, when the process of adding fonts becomes completely automated. Yes, we have some plans.

If you wish to distribute your artwork under a specific license that is not included in the recommended list, contact us first to receive a confirmation. Or consider another license.


## How to prepare a font for use with fontello

The only difference with creating your own font is adding search tags. That's very important. Fontello has a lot of icons, and nobody wants to scroll through the entire site to find one icon. We ask that you add search terms to your glyphs to make this search easier on end users. We've made this process easy for you.

So, the whole process is:

1. Import SVG images / SVG font / into a fontello project.
2. Hover over each glyph, and click the edit pencil. You'll be presented with the default name and list of search tags.
   * names can be edited both on selector and on customizer tables, every name should be unique
   * search tags are just comma-separated keywords. For example: `weather,sun` or `arrow,left`. Just imagine, that you are user, that needs to find appropriate icons. Use terms that you might search for.
3. Set font name in the field to the left of the download button.
4. Go to `Settings > Advanced` menu and fill in development info if required.
5. Select all glyphs and download your font.
6. Upload the zip file to a web host (something like [Google Drive](https://drive.google.com/))
7. Create a [new issue](https://github.com/fontello/fontello/issues/new) and link us to that zip file
   * make sure the file is set to "public" or "shared with users who have the link" so we can access it.