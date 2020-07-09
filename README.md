# Easy Fonts
https://pagecdn.com/lib/easyfonts


## Why Easy Fonts
You can use Easy Fonts for several purposes:
1. For self hosting Google Fonts.
2. 


## Easy to use CSS Classes

## Using Easy Fonts

Easy Fonts has the following directory structure:

```
/dist/              CSS files
/dist/fonts/        TTF font files
/dist/info/         JSON files containing information for all families
/dist/license/      License files for individual font families
```

All css, json, font and license files are placed in files are 

### Importing a Font

The `dist` directory contains CSS files for each individual font family. You can link to one or more CSS files from your HTML. You can download the library to play with individual font families or link to CSS files directly from CDN. Below is the link to `open sans` font families. Here is a [handy search tool](https://pagecdn.com/lib/easyfonts) for all fonts.

```
<link href="https://pagecdn.io/lib/easyfonts/open-sans.css" rel="stylesheet" />
```

### Importing all Fonts

Easy Fonts makes it easy to import all font families at once and then quickly test different fonts. For this, you need to use `dist/fonts.css` file or use the below CDN link.

```
<link href="https://pagecdn.io/lib/easyfonts/fonts.css" rel="stylesheet" />
```

### Using with Google Fonts

It is possible to use Easy Fonts and Google Fonts together. Here is how to do it.

```
<link href="https://fonts.googleapis.com/css2?family=Open+Sans:ital@0;1&display=swap" rel="stylesheet"> 
<link href="https://pagecdn.io/lib/easyfonts/classes.css" rel="stylesheet" />
```

### Importing Fonts Dynamically

Easy Fonts provides handy JSON files that contain information about individual fonts. These JSON files help you build font selection 
interfaces for themes builders. These JSON files are located in `dist/info` directory. You can load JSON files for individual fonts 
or use an all-inclusive JSON file for the entire collection.

```
//Load information of all Fonts
https://pagecdn.io/lib/easyfonts/info/fonts.json

//Load information of single font family
https://pagecdn.io/lib/easyfonts/info/open-sans.json
```




