[back to help index](Help)

We don't refuse adding new opensource fonts. The only serious requirement is unobtrusive license, that don't force users to place links on their websites, write posts, tweets, pay money, limit to non commercial use and so on. Also, we don't accept shrinked collections, used for to promote payed full sets.

Please, understand, that we are developpers, and we can't do programming and adding fonts in the same time. We need your help with prepairing font info. If you just wish to inform us about something new - place link to new fonts on the main wiki page to pending list. But if you wish font to be published quickly - read instructions below.

> We always welcome volunteer help! Anytime you can take something from pending list on [main wiki page](https://github.com/fontello/fontello/wiki) and prepare font for embedding to fontello.

_Note for authors_. Howether we don't allow right now to download separate images in vector format, we gently ask to provide separate images license for the future.

Recommended licenses are:

- [SIL](http://scripts.sil.org/OFL) for the font
- [CC BY](http://creativecommons.org/licenses/by/3.0/) or [CC BY-SA](http://creativecommons.org/licenses/by-sa/3.0/) for the images


## Requirements

- Acceptable opensource license
- Icons should be good in small size
- 40+ icons
- Nice look

Last 2 requirements will be removed, when process of adding fonts will be completely automated. Yes, we have some plans.

If you wish to distribute your artwork under specific license, that is not included into recommended list, contact us first to receive a confirmation. Or consider license change.


## How to prepare font for fontello

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
