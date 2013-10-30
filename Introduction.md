[back to help index](Help)

## What is Fontello

[Fontello](http://fontello.com) is a tool to quickly pack vector images into webfonts. Consider it like [Twitter Bootstrap](http://getbootstrap.com/), but for images. It builds everything nesessary to include graphics into your web pages. Also, fontello has big built-in collection of opensource artworks.

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

Fontello is sponsored by [RC Design](http://forum.rcdesign.ru/) & [Nodeca](http://nodeca.com/). That's a pet-project. In fact, fontello's funding is enougth to concentrate on interesting developmend & high quality, instead of loosing time with making money.


## Alternate projects & why fontello is better

Since we are sure in fontello's quality, we have no reasons to hide info about alternate projects :)

- [Icomoon](http://icomoon.io)
- [Fontastic](http://fontastic.me/)

Probably, you can find those more convenient for your needs - no problems. That's a question of taste, we are not jelous :) . However, you should understand, that fontello is much more, than just a usual font creation tool:

1. We not only "take" from opensource community (we use fonts by other authors), but we also "give back" our programming experience and our libraries. For example, see [svg2ttf](https://github.com/fontello/svg2ttf) / [ttf2woff](https://github.com/fontello/ttf2woff) / [ttf2eot](https://github.com/fontello/ttf2eot) / [svgpath](https://github.com/fontello/svgpath) . Also, all fontello code is open.
2. Alternate projects only take from opensource, and return nothing. In fact, they use opensource artworks to promote paid services. Yes, licence allows such use, but...
3. Since we provide high-quality service free, competitors can't take money for the same things from you :)
4. We don't need to push you create accounts to store your projects. Since we can suggest more effective and safe options: github + [API](https://github.com/fontello/fontello#developers-api) for your workflow intergation.
5. Fontello has much higher technical level, than competitors - we don't optimize it for making money, we optimize it for best quality. For example, we show icons on preview via fonts, while others use SVG kludges like raphael. So, our preview show exactly what you get in final result.
6. You can participate in development, for glory and for training skills :) . Fontello is opensource.