[back to help index](Help)

We don't refuse to add new open source fonts. The only serious requirement is an unobtrusive license, that doesn't force users to place links on their websites, write posts, tweet, pay money, limit use to non-commercial projects and so on. Also, we don't accept sample collections, used for to promote paid full sets.

Please, understand that we are developers, and we can't program and add fonts at the same time. We need your help with preparing font info. If you just wish to inform us about something new, place a link to the new font on the wiki page pending list. If you'd like for your font to be included more quickly, read the instructions below.

> We always welcome volunteer help! One way you can help is to take choose a font from the pending list on [main wiki page](https://github.com/fontello/fontello/wiki) and prepare the font for inclusion in fontello.

_Note for authors_. However we don't allow right now to download separate images in vector format, we gently ask to provide separate images license for the future.

Recommended licenses are:

- [SIL](http://scripts.sil.org/OFL) for the font
- [CC BY](http://creativecommons.org/licenses/by/3.0/) or [CC BY-SA](http://creativecommons.org/licenses/by-sa/3.0/) for the images


## Requirements

- Acceptable open source license
- Icons should look good at small sizes
- 40+ icons
- Nice look

Last 2 requirements will be removed in the future, when the process of adding fonts becomes completely automated. Yes, we have some plans.

If you wish to distribute your artwork under a specific license that is not included the the recommended list, contact us first to receive a confirmation. Or consider another license.


## How to prepare a font for fontello

The only difference with creating your own font is adding search tags. That's very important. Fontello has very big icons count, and nobody scroll full set to find icon. Everything is done by search.

So, the whole process is:

1. Import SVG images / SVG font / existing fontello project.
2. For each glyph, edit default name and list of search tags.
   * names can be edited both on selector and on customizer tabls, every name should be unique
   * search tags are just comme-separated keywords. For example: `weather,sun` or `arrow,left`. Just imagine, that you are user, than need to find icons. Add possible words, that you could try.
3. Set font name on the left from download button
4. Go to `Settings > Advanced` menu and fill development info.
5. Select all glyphs and download your font.
6. Create a ticket in issue tracker and give there link, where to download generated archive.