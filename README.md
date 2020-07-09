# Easy Fonts
https://pagecdn.com/lib/easyfonts


## Why Easy Fonts
You can use Easy Fonts for several purposes:
1. For self hosting Google Fonts.
2. Define custom cache control if you are not happy with CDN hosted fonts library.


## Using Easy Fonts

```HTML
<link href="https://pagecdn.io/lib/easyfonts/fonts.css" rel="stylesheet" />

<!-- Or load specific font files
    <link href="https://pagecdn.io/lib/easyfonts/open-sans.css" rel="stylesheet" />
    <link href="https://pagecdn.io/lib/easyfonts/roboto.css" rel="stylesheet" /> -->
...
<div class="font-roboto">
    <div class="font-open-sans w600i">
        Stuff here appears in Open Sans, bold and italic
    </div>
    <div class="w600">
        Stuff here appears in Roboto, bold
    </div>
    <div>
        Stuff here appears in Roboto and uses inherited weight and style
    </div>
</div>

:)
```

If you are using `fonts.css`, browsers will download just the font files that you actually use on your website and will not waste 
user's bandwidth. The `fonts.css` file itself is just **25 KB** when loaded from PageCDN. PageCDN uses Brotli:11 compression to very 
tightly compress the file to lower its size.

### Importing a Font

The [`dist`](dist) directory contains CSS files for each individual font family that you can link to from your HTML. 
You can download the library to play with individual font families or link to CSS files directly from CDN. Below is the link to 
`open sans` font family. For other font families, [here is a handy search tool](https://pagecdn.com/lib/easyfonts).

```HTML
<link href="https://pagecdn.io/lib/easyfonts/open-sans.css" rel="stylesheet" />
```

### Importing all Fonts

To quickly test different fonts, Easy Fonts makes it easy to import all font families at once. For this, you need to use 
[`dist/fonts.css`](dist/fonts.css) file or use the below CDN link.

```HTML
<link href="https://pagecdn.io/lib/easyfonts/fonts.css" rel="stylesheet" />
```

### Using with Google Fonts

It is possible to use Easy Fonts and Google Fonts together. Here is how to do it.

```HTML
<link href="https://fonts.googleapis.com/css2?family=Open+Sans:ital@0;1&display=swap" rel="stylesheet"> 
<link href="https://pagecdn.io/lib/easyfonts/classes.css" rel="stylesheet" />
```

### Importing Fonts Dynamically

Easy Fonts provides font information in JSON format for individual font families. This helps you build font selection interfaces for 
themes and website builders. The JSON is located in [`dist/info`](dist/info) directory. You can load information for individual fonts 
or use an all-inclusive JSON file for the entire fonts collection.

#### Load information of all Fonts
```
https://pagecdn.io/lib/easyfonts/info/fonts.json
```

#### Load information of single font family
```
https://pagecdn.io/lib/easyfonts/info/open-sans.json
```

## License

The TTF font files inside [`dist/fonts`](dist/fonts) are unmodified copies of TTF files in [Google Fonts](https://github.com/google/fonts/) GitHub repo 
where you can read licensing information. Individual font families have their own license files in [`dist/license`](dist/license). Relevant 
license files are linked from every CSS file too to help you easily view the license information.

The CSS and JSON files in this repository are dynamicaly generated from font files only and are covered under MIT license. If you 
are aware of a license issue with any font family listed in this repo, please [open an issue](https://github.com/pagecdn/easyfonts/issues/new) to request its removal.
