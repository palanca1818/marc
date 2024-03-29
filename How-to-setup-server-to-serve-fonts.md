[back to help index](Help)

In order to display fonts right, browser must receive font files with correct http headers. If server does not set required headers, some browsers can report errors in console or completely fail to display fonts.

Probably, your server is already configured, and you don't need to change anything. If not, you need to care about:

1. Correct mime-type headers
2. [CORS](http://en.wikipedia.org/wiki/Cross-origin_resource_sharing) headers - only if you serve fonts files & html pages from different domains
3. For IE, check that your http headers for the font files do not have no-store or no-cache

(*) If you can't set CORS headers, you can embed font files directly into CSS. Appropriate CSS file already exists in fontello archive.


## Apache

To set right mime-types for font files, add this lines to config:

```
AddType font/ttf                         ttf
AddType font/otf                         otf
AddType font/woff                        woff
AddType font/woff2                       woff2
AddType application/vnd.ms-fontobject    eot
```

If you can't edit config, create `.htaccess` file in folder with your project and add lines there.

For CORS headers add:

```
<FilesMatch ".(eot|ttf|otf|woff|woff2)">
  Header set Access-Control-Allow-Origin "*"
</FilesMatch>
```

## nginx

By default nginx has no default mime types for fonts, and wrong mime type for `.eot` files. Go to folder with configs and find where mime types are defined. Usually, that's in the `mime.types` file.

1. Search `.eot` and string with it.
2. Add strings below.

```
font/ttf                         ttf;
font/otf                         otf;
font/woff                        woff;
font/woff2                       woff2;
application/vnd.ms-fontobject    eot;
```

For CORS headers, add something like this to your vhost config

```
location ~* \.(eot|otf|ttf|woff|woff2)$ {
    add_header Access-Control-Allow-Origin *;
}
```