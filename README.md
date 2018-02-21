# nobadwords.js
nobadwords is a package which replaces bad language with grawlix or custom patterns

## Install

You can install this package with the following command

```
npm install ./nobadwords
```

## Usage

You can use nobadwords.js to prevent the use of bad language on your site, app or other project by censoring the words by adding symbols. There are three flavours to choose from: ``nobadwords()``, ``nobadwords.inner()`` and ``nobadwords.grawlix()``.

#### Replace vowels with asterisks or with a custom character

```js
var nobadwords = require("nobadwords")

nobadwords("bad word") // => b*d w*rd
nobadwords("bad word", "&") // => b&d w&rd
nobadwords("bad word", "#") // => b#d w#rd
nobadwords("bad word", "?") // => b?d w?rd
```  

#### Replace all inner characters into asterisks or a custom character
```js
var nobadwords = require("nobadwords")

nobadwords.inner("bad word") // => b******d
nobadwords.inner("bad word", "&") // => b&&&&&&d
nobadwords.inner("bad word", "#") // => b######d
nobadwords.inner("bad word", "?") // => b??????d
```

#### Replace all character with grawlix

```js
var nobadwords = require("nobadwords")

nobadwords.grawlix("bad word") // => @#$%!&?@
```

## License

This project falls under the [MIT license](license.md).
