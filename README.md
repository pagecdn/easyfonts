# Easy Fonts
https://pagecdn.com/lib/easyfonts


## Why Easy Fonts
You can use Easy Fonts for several purposes:
1. For self hosting Google Fonts.



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

Easy Fonts provides handy JSON files that contain information about individual fonts. These JSON files help you build font selection 
interfaces for themes builders. These JSON files are located in [`dist/info`](dist/info) directory. You can load JSON files for individual fonts 
or use an all-inclusive JSON file for the entire collection.


#### Load information of all Fonts
```
https://pagecdn.io/lib/easyfonts/info/fonts.json
```

#### Load information of single font family
```
https://pagecdn.io/lib/easyfonts/info/open-sans.json
```




## License

The TTF font files inside [`dist/fonts`](dist/fonts) are unmodified copy of TTF files in [Google Fonts](https://github.com/google/fonts/) GitHub repo 
where you can read licensing information. Individual font families have their own license files in [`dist/license`](dist/license). Relevant 
license files are linked from every CSS file.

The CSS and JSON files in this repository are generated dynamicaly from font files only and are covered under MIT license. If you 
are aware of a license issue with any font family listed in this repo, or if you are an author of a font and want to remove it from 
this project, please [open an issue](issues/new) to request its removal.

 


