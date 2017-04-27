# npmdoc-electron-packager

#### basic api documentation for  [electron-packager (v8.6.0)](https://github.com/electron-userland/electron-packager)  [![npm package](https://img.shields.io/npm/v/npmdoc-electron-packager.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-electron-packager) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-electron-packager.svg)](https://travis-ci.org/npmdoc/node-npmdoc-electron-packager)

#### Package and distribute your Electron app with OS-specific bundles (.app, .exe etc) via JS or CLI

[![NPM](https://nodei.co/npm/electron-packager.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/electron-packager)

- [https://npmdoc.github.io/node-npmdoc-electron-packager/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-electron-packager/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-packager/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-packager/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-electron-packager/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-electron-packager/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "max ogden"
    },
    "bin": {
        "electron-packager": "cli.js"
    },
    "bugs": {
        "url": "https://github.com/electron-userland/electron-packager/issues"
    },
    "dependencies": {
        "asar": "^0.13.0",
        "debug": "^2.2.0",
        "electron-download": "^4.0.0",
        "electron-osx-sign": "^0.4.1",
        "extract-zip": "^1.0.3",
        "fs-extra": "^2.0.0",
        "get-package-info": "^1.0.0",
        "minimist": "^1.1.1",
        "plist": "^2.0.0",
        "rcedit": "^0.8.0",
        "resolve": "^1.1.6",
        "run-series": "^1.1.1",
        "sanitize-filename": "^1.6.0",
        "semver": "^5.3.0"
    },
    "description": "Package and distribute your Electron app with OS-specific bundles (.app, .exe etc) via JS or CLI",
    "devDependencies": {
        "buffer-equal": "^1.0.0",
        "coveralls": "^2.11.6",
        "eslint": "^3.2.0",
        "eslint-config-standard": "^7.0.0",
        "eslint-plugin-promise": "^3.0.0",
        "eslint-plugin-standard": "^2.0.0",
        "eslint-plugin-tape": "^1.1.0",
        "is-admin": "^2.0.0",
        "nyc": "^10.0.0",
        "pkg-up": "^1.0.0",
        "rimraf": "^2.3.2",
        "run-waterfall": "^1.1.1",
        "tape": "^4.0.0"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "23a4233cb573389c0f728b4e87ef74416d9933e9",
        "tarball": "https://registry.npmjs.org/electron-packager/-/electron-packager-8.6.0.tgz"
    },
    "engines": {
        "node": ">= 4.0"
    },
    "eslintConfig": {
        "extends": [
            "plugin:tape/recommended",
            "standard"
        ],
        "parserOptions": {
            "sourceType": "script"
        },
        "plugins": [
            "tape"
        ],
        "rules": {
            "strict": [
                "error"
            ]
        }
    },
    "gitHead": "1c2f3ea4c4f4c724262108e628c37f165ed6f0d9",
    "homepage": "https://github.com/electron-userland/electron-packager",
    "keywords": [],
    "license": "BSD-2-Clause",
    "main": "index.js",
    "maintainers": [
        {
            "name": "feross"
        },
        {
            "name": "jlord"
        },
        {
            "name": "jsdnxx"
        },
        {
            "name": "kfranqueiro"
        },
        {
            "name": "malept"
        },
        {
            "name": "maxogden"
        },
        {
            "name": "sindresorhus"
        },
        {
            "name": "stefanbuck"
        },
        {
            "name": "zeke"
        }
    ],
    "name": "electron-packager",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/electron-userland/electron-packager.git"
    },
    "scripts": {
        "coveralls": "nyc report --reporter=text-lcov | coveralls",
        "lint": "eslint .",
        "pretest": "rimraf test/work",
        "test": "npm run lint && nyc tape test"
    },
    "version": "8.6.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
