# connect-fonts-notosans

Noto Sans fontpack for [connect-fonts](https://github.com/shane-tomlinson/connect-fonts).

## Usage

1. Include [connect-fonts](https://github.com/shane-tomlinson/connect-fonts) in a node module.
```js
const font_middleware = require("connect-fonts");
```

2. Include the font packs that you want to serve.
```js
const font_pack  = require("connect-fonts-notosans");
```

3. Add a middleware by calling the `setup` function.
```js
    app.use(font_middleware.setup({
      fonts: [ font_pack ],
      allow_origin: "https://exampledomain.com"
    }));
```

4. Add a link tag to include the font CSS.
```html
<link href="/notosans-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Multiple fonts from the family can be included by using a comma separated list of fonts:
```html
<link href="/notosans-bold,notosans-bolditalic,notosans-italic,notosans-regular/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available fonts:
* notosans-bold
* notosans-bolditalic
* notosans-italic
* notosans-regular

Locale-optimised font sets can be served by specifying the locale in the fonts.css URL.
```html
<link href="/latin/notosans-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available subsets:
* latin

5. Set your CSS up to use the new font by using the "Noto Sans" font-family.
```
    body {
      font-family: 'Noto Sans', 'sans-serif', 'serif';
    }
```

## Font Info
Noto Sans

* Description: Designed by Monotype design team
* Copyright: Copyright 2012 Google Inc. All Rights Reserved.
* Trademark: Noto is a trademark of Google Inc. and may be registered in certain jurisdictions.
* Designer: Monotype Design team
* Designer URL: http://www.monotypeimaging.com/ProductsServices/TypeDesignerShowcase 
* Vendor: Monotype Imaging Inc.
* Vendor URL: http://code.google.com/p/noto/

## Development Info
* Homepage: https://github.com/shane-tomlinson/connect-fonts-notosans
* Repo: https://github.com/shane-tomlinson/connect-fonts-notosans

## Author
* Shane Tomlinson
* shane@shanetomlinson.com
* stomlinson@mozilla.com
* set117@yahoo.com
* https://shanetomlinson.com
* https://github.com/shane-tomlinson
* https://github.com/stomlinson
* @shane_tomlinson


## License

Software: Licenced under version 2.0 of the MPL

  https://www.mozilla.org/MPL/

Fonts: Licensed under version 2.0 of the Apache

  http://www.apache.org/licenses/LICENSE-2.0

