[back to help index](Help)

If you have problem with icons on your website, please check in different browsers / operating systems first.

## Quick check

1. Open demo page from fontello archive and check if it's ok. Then try to understand what is different on your site.
2. Check that files are uploaded right (no problems with encoding and so on)
3. In browser dev tools
  - check that no error message in console
  - on network tab
    - check that fonts are loaded (correct url)
    - check that fonts [[mime types|How to setup server to serve fonts]] are correct
  - on html tab
    - check that @fontface and icon code rules are really applied for element, that should show icon

## Usual cases

1. __No icons at all__
  - You probably have wrong fonts paths in CSS. Open browser dev tool and look at networking tab.
2. __No icons in Firefox__
  - If your font and html page are placed on different domains, server must respond with proper CORS headers. Read [[How to setup server to serve fonts]] article. If you can't change server configuration - use CSS file, where fonts are embedded directly. It's already included in generated archive.
3. __No icons (or some icons) on specific browsers/platforms__
  - If you used 3-bytes char codes (like 0x1F459), try to change them to 2-bytes from PUA area (0xE000-0xF8FF).
  - If that doesn't help, create a ticket in issue tracker, with detailed info:
    - device name
    - operating system and version
    - browser name and version
    - link to example page
  - Prior to creating such a ticket, make sure that fonts are ok in other situations.

## Asking for help

Note that most issues are related to not fontello bug, but to your understanding of css. Fontello is not a commercial service, and any help is provided "when possible". To maximize effectivity, please, provide this info in your request:

- link to live example (almost mandatory)
- gist with your fontello config from archive, or link to the whole archive with fontello font
- screenshot (optional, and that can be not enough without live link)
- OS / Browsers with versions. Note, that we are <s>poor boys without macs</s>crazy boys with ubuntu on macs, and it's comfortable for us, if your problem can be reproduced in chrome/firefox.

Contacts:

- Questions: [Google group](https://groups.google.com/group/fontello/)
- Bug reports: [Issue tracker](https://github.com/fontello/fontello/issues)

Please create new issues in tracker only when you are sure that it's really fontello's problem. For general questions use Google group.