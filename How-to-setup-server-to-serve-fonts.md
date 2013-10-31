[back to help index](Help)

In order to display fonts right, browser must receive font files with correct http headers. If server does not set required headers, some browsers can report errors in console or completely fail to display fonts.

Probably, your server is already configured, and you don't need to change anything. If not, you need to care about:

1. Correct `mime-type` headers
2. `CORS` headers - only if you serve fonts files & html pages from different domains

(*) If you can't set CORS headers, you can embed font files directly into CSS. Template already exists in fontello archive.


## Apache

To set right mime-types for font files, add this lines to config:

```
AddType application/vnd.ms-fontobject    .eot
AddType application/x-font-ttf           .ttf
AddType application/font-woff            .woff
```

If you can't edit config, create `.htaccess` file in folder with your project and add lines there.


## nginx

By default nginx has no default mime types for fonts, and wrong mimy type for `.eot` files. Got to folder with configs and find where mime types are defiled. Usually, that's in `mimes.conf` file.

1. Search `.eot` and string with it.
2. Add strings below.

```
application/vnd.ms-fontobject    eot;
application/x-font-ttf           ttf;
application/font-woff            woff;
```
