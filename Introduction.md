[back to help index](Help)

## What is Fontello

[Fontello](http://fontello.com) is a tool to quickly pack vector images into webfonts. Consider it like [Twitter Bootstrap](http://getbootstrap.com/), but for images. It builds everything nesessary to include graphics into your web pages. Also, fontello has a big built-in collection of opensource artworks.

If you like stories, here is an [article on CSS Tricks](http://css-tricks.com/fontello-past-future-icon-font-service/) how fontello was created.

## Why iconic fonts are cool

__Advantages__

- Fonts are vectors, so there is no pixelation or blurring on high-resolution screens as there would be if the graphic was raster and needed to scale up.
- The browser support is as good as you need it to be
- Once the system is in place, using them is very convenient.
  - Arguably easier than spriting images.
  - They can be controlled with CSS, like the size, color, shadow, etc.

__Limitations__

- The icons will be single-color. There are some fancy (hacky) techniques for multi-color however, and modern trends and HIGs (human interface guidelines) suggest single colors anyway.

Look at [nice demo](http://css-tricks.com/examples/IconFont/) what you can do with iconic fonts.


## Why fontello is opensource and free

Fontello is a pet-project, sponsored by [RC Design](http://forum.rcdesign.ru/) & [Nodeca](http://nodeca.com/). We do it just because we love programming and doing something interesting.

Please, note, that fontello is non-commercial project. It is intentional choice to have more time for development. We prefer to spend time for reaching highest quality, instead of making money. That's the main reason, when we select priorities for new features.

For example, sometime people ask why fontello does not provide user accounts to store projects on our server. Here's our thoughts:

- Keeping critical user data is a big responsibility. To keep quality of service high, that requires investment and that means running Fontello like a business. Since Fontello is positioned as non-commercial project, we don't want to push it toward being a business.
- Users don’t need accounts, they need good importing and exporting. This can be achieved in better way:
  - Every generated font pack already has config file which can be loaded back into Fontello to continue work. Just drag it (or the whole archive) onto the Fontello site. Or use the API, for [your workwlow integration](https://github.com/fontello/fontello/wiki/How-to-save-and-load-projects). Easy!
  - Use GitHub to store your projects and control changes. That’s much more safe and protects you from mistakes.

Of cause, we are always ready to improve fontello with something awesome. Feel free to share your ideas in our [tracker](https://github.com/fontello/fontello/issues). We consider any ideas, even mad ones :)


## Alternate projects & why fontello is better

Since we are sure in fontello's quality, we have no reasons to hide info about alternate projects :)

- [Icomoon](http://icomoon.io)
- [Fontastic](http://fontastic.me/)
- [Pictos](http://pictos.cc/server/)

Probably, you can find those more convenient for your needs - no problems. That's a question of taste, we are not jelous :) . However, you should understand, that fontello is much more, than just a usual font creation tool:

1. We not only "take" from opensource community (we use fonts by other authors), but we also "give back" our programming experience and our libraries. For example, see [svg2ttf](https://github.com/fontello/svg2ttf) / [ttf2woff](https://github.com/fontello/ttf2woff) / [ttf2eot](https://github.com/fontello/ttf2eot) / [svgpath](https://github.com/fontello/svgpath) . Also, all fontello code is open.
2. Very often alternate commercial projects just use artworks of opensourse developpers to promote their paid services, and return nothing back to community. May be, that's ok for iconic fonts creation, but too few in general for moving progress forward. Yes, many opensourse licences allows such use, but...
3. Since we provide high-quality service free, commercial "competitors" can't take money from you for the same things :)
4. We don't need to push you create accounts to store your projects. Since we can suggest more effective and safe options: github + [API](https://github.com/fontello/fontello#developers-api) for your [workflow intergation](https://github.com/fontello/fontello/wiki/How-to-save-and-load-projects).
5. Fontello has much higher technical level, than competitors - we don't optimize it for making money, we optimize it for best quality. For example, we show icons on preview via fonts, while others use SVG kludges like raphael. So, our preview show exactly what you get in final result.
6. You can participate in development, for fun, for glory and for training skills :) . Fontello is opensource.