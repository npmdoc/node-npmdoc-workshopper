# api documentation for  [workshopper (v2.7.0)](https://github.com/rvagg/workshopper)  [![npm package](https://img.shields.io/npm/v/npmdoc-workshopper.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-workshopper) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-workshopper.svg)](https://travis-ci.org/npmdoc/node-npmdoc-workshopper)
#### A terminal workshop runner framework

[![NPM](https://nodei.co/npm/workshopper.png?downloads=true)](https://www.npmjs.com/package/workshopper)

[![apidoc](https://npmdoc.github.io/node-npmdoc-workshopper/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-workshopper_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-workshopper/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-workshopper/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-workshopper/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Rod Vagg",
        "email": "rod@vagg.org",
        "url": "https://github.com/rvagg"
    },
    "bugs": {
        "url": "https://github.com/rvagg/workshopper/issues"
    },
    "dependencies": {
        "chalk": "~0.4.0",
        "colors-tmpl": "~0.1.0",
        "i18n-core": "^1.3.2",
        "map-async": "~0.1.1",
        "mkdirp": "~0.3.5",
        "msee": "~0.1.1",
        "optimist": "~0.6.1",
        "terminal-menu": "^2.1.1",
        "visualwidth": "~0.0.1",
        "xtend": "~3.0.0"
    },
    "description": "A terminal workshop runner framework",
    "devDependencies": {
        "workshopper-exercise": "^1.1.0"
    },
    "directories": {
        "example": "examples"
    },
    "dist": {
        "shasum": "36798703f08071f504ccf9743990663e7b42f639",
        "tarball": "https://registry.npmjs.org/workshopper/-/workshopper-2.7.0.tgz"
    },
    "gitHead": "21f7b948071954b595946aae07192da40578b1cd",
    "homepage": "https://github.com/rvagg/workshopper",
    "license": "MIT",
    "main": "./workshopper.js",
    "maintainers": [
        {
            "name": "rvagg",
            "email": "rod@vagg.org"
        },
        {
            "name": "maxogden",
            "email": "max@maxogden.com"
        },
        {
            "name": "julianduque",
            "email": "julianduquej@gmail.com"
        },
        {
            "name": "leichtgewicht",
            "email": "mh@leichtgewicht.at"
        }
    ],
    "name": "workshopper",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/rvagg/workshopper.git"
    },
    "scripts": {
        "test": "echo \"Error: no test specified\" && exit 1"
    },
    "version": "2.7.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module workshopper](#apidoc.module.workshopper)
1.  [function <span class="apidocSignatureSpan">workshopper.</span>super_ ()](#apidoc.element.workshopper.super_)
1.  object <span class="apidocSignatureSpan">workshopper.</span>i18n
1.  object <span class="apidocSignatureSpan">workshopper.</span>print_text
1.  object <span class="apidocSignatureSpan">workshopper.</span>util

#### [module workshopper.i18n](#apidoc.module.workshopper.i18n)
1.  [function <span class="apidocSignatureSpan">workshopper.i18n.</span>chooseLang (globalDataDir, appDataDir, lang, defaultLang, availableLangs)](#apidoc.element.workshopper.i18n.chooseLang)
1.  [function <span class="apidocSignatureSpan">workshopper.i18n.</span>init (options, exercises, lang)](#apidoc.element.workshopper.i18n.init)

#### [module workshopper.print_text](#apidoc.module.workshopper.print_text)
1.  [function <span class="apidocSignatureSpan">workshopper.print_text.</span>file (appName, appDir, file, callback)](#apidoc.element.workshopper.print_text.file)
1.  [function <span class="apidocSignatureSpan">workshopper.print_text.</span>localisedFile (appName, appDir, file, lang, callback)](#apidoc.element.workshopper.print_text.localisedFile)
1.  [function <span class="apidocSignatureSpan">workshopper.print_text.</span>localisedFirstFile (appName, appDir, files, lang, callback)](#apidoc.element.workshopper.print_text.localisedFirstFile)
1.  [function <span class="apidocSignatureSpan">workshopper.print_text.</span>text (appName, appDir, filetype, contents)](#apidoc.element.workshopper.print_text.text)

#### [module workshopper.util](#apidoc.module.workshopper.util)
1.  [function <span class="apidocSignatureSpan">workshopper.util.</span>applyTextMarker (text, marker, size)](#apidoc.element.workshopper.util.applyTextMarker)
1.  [function <span class="apidocSignatureSpan">workshopper.util.</span>assertDir ()](#apidoc.element.workshopper.util.assertDir)
1.  [function <span class="apidocSignatureSpan">workshopper.util.</span>assertFile ()](#apidoc.element.workshopper.util.assertFile)
1.  [function <span class="apidocSignatureSpan">workshopper.util.</span>dirFromName (exerciseDir, name)](#apidoc.element.workshopper.util.dirFromName)
1.  [function <span class="apidocSignatureSpan">workshopper.util.</span>idFromName (id)](#apidoc.element.workshopper.util.idFromName)
1.  [function <span class="apidocSignatureSpan">workshopper.util.</span>repeat (ch, sz)](#apidoc.element.workshopper.util.repeat)
1.  [function <span class="apidocSignatureSpan">workshopper.util.</span>userDir ()](#apidoc.element.workshopper.util.userDir)



# <a name="apidoc.module.workshopper"></a>[module workshopper](#apidoc.module.workshopper)

#### <a name="apidoc.element.workshopper.super_"></a>[function <span class="apidocSignatureSpan">workshopper.</span>super_ ()](#apidoc.element.workshopper.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.workshopper.i18n"></a>[module workshopper.i18n](#apidoc.module.workshopper.i18n)

#### <a name="apidoc.element.workshopper.i18n.chooseLang"></a>[function <span class="apidocSignatureSpan">workshopper.i18n.</span>chooseLang (globalDataDir, appDataDir, lang, defaultLang, availableLangs)](#apidoc.element.workshopper.i18n.chooseLang)
- description and source-code
```javascript
function chooseLang(globalDataDir, appDataDir, lang, defaultLang, availableLangs) {
  var globalPath = path.resolve(globalDataDir, 'lang.json')
    , appPath = path.resolve(appDataDir, 'lang.json')
    , data
  try {
    // Lets see if we find some stored language in the app's config
    data = require(appPath)
  } catch (e) {
    // Without a file an error will occur here, but thats okay
  }
  if (!data) {
    // Lets see if some other workshopper stored language settings
    try {
      data = require(globalPath)
    } catch (e) {
      data = {}
      // Without a file an error will occur here, but thats okay
    }
  }

  if (!!lang && typeof lang != 'string')
    throw new TypeError('Please supply a language. Available languages are: ' + availableLangs.join(', '))

  if (lang)
    lang = lang.replace(/_/g, '-').toLowerCase()

  if (availableLangs.indexOf(defaultLang) === -1)
    throw new TypeError('The default language "' + defaultLang + ' is not one of the available languages?! Available languages are
: ' + availableLangs.join(', '))

  if (lang && availableLangs.indexOf(lang) === -1)
    throw new TypeError('The language "' + lang + '" is not available.\nAvailable languages are ' + availableLangs.join(', ') + '.\n\nNote: the language is not case-sensitive ("en", "EN", "eN", "En" will become "en") and you can use "_" instead of "-" for seperators.')

  if (availableLangs.indexOf(data.selected) === -1)
    // The stored data is not available so lets use one of the other languages
    data.selected = lang || defaultLang
  else
    data.selected = lang || data.selected || defaultLang

  try {
    fs.writeFileSync(globalPath, JSON.stringify(data))
    fs.writeFileSync(appPath, JSON.stringify(data))
  } catch(e) {
    // It is not good if an error occurs but it shouldn't really matter
  }
  return data.selected
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.workshopper.i18n.init"></a>[function <span class="apidocSignatureSpan">workshopper.i18n.</span>init (options, exercises, lang)](#apidoc.element.workshopper.i18n.init)
- description and source-code
```javascript
init = function (options, exercises, lang) {
  var translator = i18n(
        i18nChain(
            i18nFs(path.resolve(options.appDir, './i18n'))
          , i18nFs(path.resolve(__dirname, './i18n'))
          , i18nObject(createDefaultLookup(options, exercises))
        )
      )
    , result = translator.lang(lang, true)
  translator.fallback = function (key) {
    if (!key)
      return '(???)'

    return '?' + key + '?'
  }
  result.languages = options.languages || ['en']
  result.change = function (globalDataDir, appDataDir, lang, defaultLang, availableLangs) {
    result.changeLang(lang)
    chooseLang(globalDataDir, appDataDir, lang, defaultLang, availableLangs)
  }
  return result
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.workshopper.print_text"></a>[module workshopper.print_text](#apidoc.module.workshopper.print_text)

#### <a name="apidoc.element.workshopper.print_text.file"></a>[function <span class="apidocSignatureSpan">workshopper.print_text.</span>file (appName, appDir, file, callback)](#apidoc.element.workshopper.print_text.file)
- description and source-code
```javascript
function printFile(appName, appDir, file, callback) {
  fs.readFile(file, 'utf8', function (err, contents) {
    if (err)
      throw err

    printText(appName, appDir, path.extname(file).replace(/^\./, ''), contents)
    callback && callback();
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.workshopper.print_text.localisedFile"></a>[function <span class="apidocSignatureSpan">workshopper.print_text.</span>localisedFile (appName, appDir, file, lang, callback)](#apidoc.element.workshopper.print_text.localisedFile)
- description and source-code
```javascript
function printLocalisedFile(appName, appDir, file, lang, callback) {
  file = getExistingFile(file, lang)

  if (file) {
    printFile(appName, appDir, file, callback)
    return true
  }

  if (callback)
    process.nextTick(callback)

  return false
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.workshopper.print_text.localisedFirstFile"></a>[function <span class="apidocSignatureSpan">workshopper.print_text.</span>localisedFirstFile (appName, appDir, files, lang, callback)](#apidoc.element.workshopper.print_text.localisedFirstFile)
- description and source-code
```javascript
function printLocalisedFirstFile(appName, appDir, files, lang, callback) {
  var consumed = false
  files.filter(function (file) {
    // Since the files that will be printed are subject to user manipulation
    // a null can happen here, checking for it just in case.
    return file !== undefined && file !== null
  }).forEach(function (file) {
    if (consumed)
      return
    if (file = getExistingFile(file, lang)) {
      consumed = true
      printFile(appName, appDir, file, callback)
    }
  })
  if (!consumed && callback)
    process.nextTick(callback)
  return consumed
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.workshopper.print_text.text"></a>[function <span class="apidocSignatureSpan">workshopper.print_text.</span>text (appName, appDir, filetype, contents)](#apidoc.element.workshopper.print_text.text)
- description and source-code
```javascript
function printText(appName, appDir, filetype, contents) {
  var variables = {
      appname : appName
    , rootdir : appDir
  }

  contents = colorsTmpl(contents)

  contents = contents.replace(/\{([^}]+)\}/gi, function (match, k) {
    return variables[k] || ('{' + k + '}')
  })

  // proper path resolution
  contents = contents.replace(/\{rootdir:([^}]+)\}/gi, function (match, subpath) {
    return 'file://' + path.join(appDir, subpath)
  })

  if (filetype == 'md') {
    // convert Markdown to ANSI
    contents = msee.parse(contents, mseeOptions)
  }

  console.log(contents)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.workshopper.util"></a>[module workshopper.util](#apidoc.module.workshopper.util)

#### <a name="apidoc.element.workshopper.util.applyTextMarker"></a>[function <span class="apidocSignatureSpan">workshopper.util.</span>applyTextMarker (text, marker, size)](#apidoc.element.workshopper.util.applyTextMarker)
- description and source-code
```javascript
function applyTextMarker(text, marker, size) {
  var availableSpace = size - vw.width(marker, true)

  text = vw.truncate(text, availableSpace, '...', true)

  return text + repeat(' ', availableSpace - vw.width(text, true)) + marker
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.workshopper.util.assertDir"></a>[function <span class="apidocSignatureSpan">workshopper.util.</span>assertDir ()](#apidoc.element.workshopper.util.assertDir)
- description and source-code
```javascript
assertDir = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.workshopper.util.assertFile"></a>[function <span class="apidocSignatureSpan">workshopper.util.</span>assertFile ()](#apidoc.element.workshopper.util.assertFile)
- description and source-code
```javascript
assertFile = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.workshopper.util.dirFromName"></a>[function <span class="apidocSignatureSpan">workshopper.util.</span>dirFromName (exerciseDir, name)](#apidoc.element.workshopper.util.dirFromName)
- description and source-code
```javascript
function dirFromName(exerciseDir, name) {
  return path.join(exerciseDir, idFromName(name))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.workshopper.util.idFromName"></a>[function <span class="apidocSignatureSpan">workshopper.util.</span>idFromName (id)](#apidoc.element.workshopper.util.idFromName)
- description and source-code
```javascript
function idFromName(id) {
  return id.toLowerCase()
    .replace(/\s/g, '_')
    .replace(/[^\w]/gi, '')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.workshopper.util.repeat"></a>[function <span class="apidocSignatureSpan">workshopper.util.</span>repeat (ch, sz)](#apidoc.element.workshopper.util.repeat)
- description and source-code
```javascript
function repeat(ch, sz) {
  return new Array(sz + 1).join(ch)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.workshopper.util.userDir"></a>[function <span class="apidocSignatureSpan">workshopper.util.</span>userDir ()](#apidoc.element.workshopper.util.userDir)
- description and source-code
```javascript
function userDir() {
  var folders = [process.env.HOME || process.env.USERPROFILE].concat(Array.prototype.slice.apply(arguments))
  var dir = path.join.apply(path, folders)
  mkdirp.sync(dir)
  return dir
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
