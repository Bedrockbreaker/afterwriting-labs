# How to add a new font?

1. Copy font files (ttf/otf) to `afterwriting-labs/js/fonts/source/FolderWithMyFonts`
2. Generate JS file with fonts using:
    ```bash
    cd afterwriting-labs/js/fonts
    node ../../tools/fonts-converter.js \
        -r source/FolderWithMyFonts/MyFont-Regular.ttf \
        -b source/FolderWithMyFonts/MyFont-Bold.ttf \
        -i source/FolderWithMyFonts/MyFont-Italic.ttf \
        -x source/FolderWithMyFonts/MyFont-Bold-Italic.ttf \
        -o my-font.js
    ```
3. Add new font to the config: `afterwriting-labs/js/fonts/fonts-loader.js`

# Sources:

## courier-prime.js

Courier Prime: https://quoteunquoteapps.com/courierprime/downloads/courier-prime.zip

```bash
node ../../tools/fonts-converter.js \
    -r source/Courier-Prime/Courier-Prime.ttf \
    -b source/Courier-Prime/Courier-Prime-Bold.ttf \
    -i source/Courier-Prime/Courier-Prime-Italic.ttf \
    -x source/Courier-Prime/Courier-Prime-Bold-Italic.ttf \
    -o courier-prime.js
```

## courier-prime-cyrillic.js

Courier Prime Cyrillic: http://dimkanovikov.pro/courierprime/courierprime.zip

```bash
node ../../tools/fonts-converter.js \
    -r source/Courier-Prime-Cyrillic/Courier-Prime.ttf \
    -b source/Courier-Prime-Cyrillic/Courier-Prime-Bold.ttf \
    -i source/Courier-Prime-Cyrillic/Courier-Prime-Italic.ttf \
    -x source/Courier-Prime-Cyrillic/Courier-Prime-Bold-Italic.ttf \
    -o courier-prime-cyrillic.js
```

## kosugi.js

Kosugi: https://fonts.google.com/specimen/Kosugi

```bash
node ../../tools/fonts-converter.js \
    -r source/Kosugi/Kosugi-Regular.ttf \
    -o kosugi.js
```

## kosugi-prime.js

A derived font from both Courier Prime and Kosugi.

```bash
node ../../tools/fonts-converter.js \
    -r source/Kosugi-Prime/KosugiPrime.ttf \
    -b source/Kosugi-Prime/KosugiPrime-Bold.ttf \
    -i source/Kosugi-Prime/KosugiPrime-Italic.ttf \
    -x source/Kosugi-Prime/KosugiPrime-Bold-Italic.ttf \
    -o kosugi-prime.js
```