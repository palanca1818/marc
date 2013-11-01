[back to help index](Help)

If you have problem with icons on your website, please check in different browsers / operating systems first. Then look into checklist.

1. __No iconst at all__
  - Probably, you have wrong fonts paths in CSS. Open browser dev tool and look at networking tab.
2. __No icons in Firefox__
  - if your font and html page are placed on different domains, server must respond with proper CORS headers. Read [[How to setup server to serve fonts]] article. If you can't change server configuration - use CSS file, where fonts are embedded directly. It's already included in generated archive.
3. __No icons (or some icons) on sppecific browsers/platforms__
  - If you used 3-bytes char codes (like 0x1F459), try to change them to 2-bytes from PUA area (0xE000-0xFFFE).
  - If that doesn't help, create a ticket in issue tracker, with detailed info:
    - device name
    - operating system and version
    - browser name and version
    - link to example page
  - Prior to create such ticket, make sure, that fonts are ok in another sutuations.

If your problem is not listed here - contact us:

- Questions: [Google group](https://groups.google.com/group/fontello/)
- Bug reports: [Issue tracker](https://github.com/fontello/fontello/issues)

Please, create new issues in tracker only when you are sure, that it's really fontello's problem. For general questions use google group.