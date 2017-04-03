# api documentation for  [color (v1.0.3)](https://github.com/qix-/color#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-color.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-color) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-color.svg)](https://travis-ci.org/npmdoc/node-npmdoc-color)
#### Color conversion and manipulation with CSS string support

[![NPM](https://nodei.co/npm/color.png?downloads=true)](https://www.npmjs.com/package/color)

[![apidoc](https://npmdoc.github.io/node-npmdoc-color/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-color_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-color/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-color/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-color/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "authors": [
        "Josh Junon <i.am.qix@gmail.com>",
        "Heather Arthur <fayearthur@gmail.com>",
        "Maxime Thirouin"
    ],
    "bugs": {
        "url": "https://github.com/qix-/color/issues"
    },
    "dependencies": {
        "color-convert": "^1.8.2",
        "color-string": "^1.4.0"
    },
    "description": "Color conversion and manipulation with CSS string support",
    "devDependencies": {
        "mocha": "^2.2.5",
        "xo": "^0.12.1"
    },
    "directories": {},
    "dist": {
        "shasum": "e48e832d85f14ef694fb468811c2d5cfe729b55d",
        "tarball": "https://registry.npmjs.org/color/-/color-1.0.3.tgz"
    },
    "files": [
        "CHANGELOG.md",
        "LICENSE",
        "index.js"
    ],
    "gitHead": "4234b4044a2bb206986af8d61c7b7cc829707ceb",
    "homepage": "https://github.com/qix-/color#readme",
    "keywords": [
        "color",
        "colour",
        "css"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "harth",
            "email": "fayearthur@gmail.com"
        },
        {
            "name": "moox",
            "email": "m@moox.io"
        },
        {
            "name": "qix",
            "email": "i.am.qix@gmail.com"
        }
    ],
    "name": "color",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/qix-/color.git"
    },
    "scripts": {
        "pretest": "xo",
        "test": "mocha"
    },
    "version": "1.0.3",
    "xo": {
        "rules": {
            "no-cond-assign": 0,
            "new-cap": 0
        }
    }
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module color](#apidoc.module.color)
1.  [function <span class="apidocSignatureSpan">color.</span>ansi16 (color)](#apidoc.element.color.ansi16)
1.  [function <span class="apidocSignatureSpan">color.</span>ansi256 (color)](#apidoc.element.color.ansi256)
1.  [function <span class="apidocSignatureSpan">color.</span>apple (color)](#apidoc.element.color.apple)
1.  [function <span class="apidocSignatureSpan">color.</span>cmyk (color)](#apidoc.element.color.cmyk)
1.  [function <span class="apidocSignatureSpan">color.</span>hcg (color)](#apidoc.element.color.hcg)
1.  [function <span class="apidocSignatureSpan">color.</span>hsl (color)](#apidoc.element.color.hsl)
1.  [function <span class="apidocSignatureSpan">color.</span>hsv (color)](#apidoc.element.color.hsv)
1.  [function <span class="apidocSignatureSpan">color.</span>hwb (color)](#apidoc.element.color.hwb)
1.  [function <span class="apidocSignatureSpan">color.</span>lab (color)](#apidoc.element.color.lab)
1.  [function <span class="apidocSignatureSpan">color.</span>lch (color)](#apidoc.element.color.lch)
1.  [function <span class="apidocSignatureSpan">color.</span>rgb (color)](#apidoc.element.color.rgb)
1.  [function <span class="apidocSignatureSpan">color.</span>xyz (color)](#apidoc.element.color.xyz)



# <a name="apidoc.module.color"></a>[module color](#apidoc.module.color)

#### <a name="apidoc.element.color.ansi16"></a>[function <span class="apidocSignatureSpan">color.</span>ansi16 (color)](#apidoc.element.color.ansi16)
- description and source-code
```javascript
ansi16 = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.color.ansi256"></a>[function <span class="apidocSignatureSpan">color.</span>ansi256 (color)](#apidoc.element.color.ansi256)
- description and source-code
```javascript
ansi256 = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
...

'''js
var color = Color('#7743CE').alpha(0.5).lighten(0.5);
console.log(color.hsl().string());  // 'hsla(262, 59%, 81%, 0.5)'

console.log(color.cmyk().round().array());  // [ 16, 25, 0, 8, 0.5 ]

console.log(color.ansi256().object());  // { ansi256: 183, alpha: 0.5 }
'''

## Install
'''console
$ npm install color
'''
...
```

#### <a name="apidoc.element.color.apple"></a>[function <span class="apidocSignatureSpan">color.</span>apple (color)](#apidoc.element.color.apple)
- description and source-code
```javascript
apple = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.color.cmyk"></a>[function <span class="apidocSignatureSpan">color.</span>cmyk (color)](#apidoc.element.color.cmyk)
- description and source-code
```javascript
cmyk = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
...

> JavaScript library for immutable color conversion and manipulation with support for CSS color strings.

'''js
var color = Color('#7743CE').alpha(0.5).lighten(0.5);
console.log(color.hsl().string());  // 'hsla(262, 59%, 81%, 0.5)'

console.log(color.cmyk().round().array());  // [ 16, 25, 0, 8, 0.5 ]

console.log(color.ansi256().object());  // { ansi256: 183, alpha: 0.5 }
'''

## Install
'''console
$ npm install color
...
```

#### <a name="apidoc.element.color.hcg"></a>[function <span class="apidocSignatureSpan">color.</span>hcg (color)](#apidoc.element.color.hcg)
- description and source-code
```javascript
hcg = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.color.hsl"></a>[function <span class="apidocSignatureSpan">color.</span>hsl (color)](#apidoc.element.color.hsl)
- description and source-code
```javascript
hsl = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
...

# color [![Build Status](https://travis-ci.org/Qix-/color.svg?branch=master)](https://travis-ci.org/Qix-/color)

> JavaScript library for immutable color conversion and manipulation with support for CSS color strings.

'''js
var color = Color('#7743CE').alpha(0.5).lighten(0.5);
console.log(color.hsl().string());  // 'hsla(262, 59%, 81%, 0.5)'

console.log(color.cmyk().round().array());  // [ 16, 25, 0, 8, 0.5 ]

console.log(color.ansi256().object());  // { ansi256: 183, alpha: 0.5 }
'''

## Install
...
```

#### <a name="apidoc.element.color.hsv"></a>[function <span class="apidocSignatureSpan">color.</span>hsv (color)](#apidoc.element.color.hsv)
- description and source-code
```javascript
hsv = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.color.hwb"></a>[function <span class="apidocSignatureSpan">color.</span>hwb (color)](#apidoc.element.color.hwb)
- description and source-code
```javascript
hwb = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
...
	desaturate: function (ratio) {
		var hsl = this.hsl();
		hsl.color[1] -= hsl.color[1] * ratio;
		return hsl;
	},

	whiten: function (ratio) {
		var hwb = this.hwb();
		hwb.color[1] += hwb.color[1] * ratio;
		return hwb;
	},

	blacken: function (ratio) {
		var hwb = this.hwb();
		hwb.color[2] += hwb.color[2] * ratio;
...
```

#### <a name="apidoc.element.color.lab"></a>[function <span class="apidocSignatureSpan">color.</span>lab (color)](#apidoc.element.color.lab)
- description and source-code
```javascript
lab = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.color.lch"></a>[function <span class="apidocSignatureSpan">color.</span>lch (color)](#apidoc.element.color.lch)
- description and source-code
```javascript
lch = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.color.rgb"></a>[function <span class="apidocSignatureSpan">color.</span>rgb (color)](#apidoc.element.color.rgb)
- description and source-code
```javascript
rgb = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
...
var Color = require('color');
'''

### Constructors
'''js
var color = Color('rgb(255, 255, 255)')
var color = Color({r: 255, g: 255, b: 255})
var color = Color.rgb(255, 255, 255)
var color = Color.rgb([255, 255, 255])
'''

Set the values for individual channels with 'alpha', 'red', 'green', 'blue', 'hue', 'saturation' (hsl), 'saturationv' (hsv), 'lightness
', 'whiteness', 'blackness', 'cyan', 'magenta', 'yellow', 'black'

### Getters
'''js
...
```

#### <a name="apidoc.element.color.xyz"></a>[function <span class="apidocSignatureSpan">color.</span>xyz (color)](#apidoc.element.color.xyz)
- description and source-code
```javascript
xyz = function (color) {
		if (typeof color === 'number') {
			color = zeroArray(_slice.call(arguments), channels);
		}
		return new Color(color, model);
	}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
