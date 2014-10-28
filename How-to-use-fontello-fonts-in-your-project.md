Fontello generates archive with fonts, css files and docs. Here are recommendation, how to use one in your project to show icons.

## Recommended way

1. Copy ALL files with folder structure into your project, without change. That will simplify future font updates.
2. If you need to change `@fontface` params - use `<your_font_name>-codes.css`, and define `@fontface` rule in outer files. That will help to keep fontello folder intact, and will prevent mistakes on upgrade, when you overwrite content with new font version.
  - Also, having your own `@font-face` will allow to use [new notation from twitter bootstrap 3+](http://getbootstrap.com/components/#glyphicons) - every icon can be defined with 2 CSS classes.
3. Don't forget to [[setup proper mime types|How to setup server to serve fonts]] for font file.
4. If you place fonts on separate domain, make sure, that server responds with proper [[CORS headers|How to setup server to serve fonts]].

## Special cases

### Separate domains + no CORS headers

That's a bad situation. Try to avoid it if possible. But if you can't  - embed fonts directly into CSS. See example in `<your_font_name>-codes.css`.

### IE7

TBD

### IE6

TBD

## Troubleshooting

Look at [[problems checklist]]