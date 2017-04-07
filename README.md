# api documentation for  [electron-packager (v8.6.0)](https://github.com/electron-userland/electron-packager)  [![npm package](https://img.shields.io/npm/v/npmdoc-electron-packager.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-electron-packager) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-electron-packager.svg)](https://travis-ci.org/npmdoc/node-npmdoc-electron-packager)
#### Package and distribute your Electron app with OS-specific bundles (.app, .exe etc) via JS or CLI

[![NPM](https://nodei.co/npm/electron-packager.png?downloads=true)](https://www.npmjs.com/package/electron-packager)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-packager/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-electron-packager%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-packager/build/apidoc.html)

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
            "name": "feross",
            "email": "feross@feross.org"
        },
        {
            "name": "jlord",
            "email": "to.jlord@gmail.com"
        },
        {
            "name": "jsdnxx",
            "email": "jason@denizac.org"
        },
        {
            "name": "kfranqueiro",
            "email": "kenneth.franqueiro@gmail.com"
        },
        {
            "name": "malept",
            "email": "nodejs.npm.nospam@lazymalevolence.com"
        },
        {
            "name": "maxogden",
            "email": "max@maxogden.com"
        },
        {
            "name": "sindresorhus",
            "email": "sindresorhus@gmail.com"
        },
        {
            "name": "stefanbuck",
            "email": "web@broud.de"
        },
        {
            "name": "zeke",
            "email": "zeke@sikelianos.com"
        }
    ],
    "name": "electron-packager",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module electron-packager](#apidoc.module.electron-packager)
1.  object <span class="apidocSignatureSpan">electron-packager.</span>common
1.  object <span class="apidocSignatureSpan">electron-packager.</span>ignore
1.  object <span class="apidocSignatureSpan">electron-packager.</span>linux
1.  object <span class="apidocSignatureSpan">electron-packager.</span>mac
1.  object <span class="apidocSignatureSpan">electron-packager.</span>targets
1.  object <span class="apidocSignatureSpan">electron-packager.</span>win32

#### [module electron-packager.common](#apidoc.module.electron-packager.common)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>baseTempDir (opts)](#apidoc.element.electron-packager.common.baseTempDir)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>camelCase (properties, warn)](#apidoc.element.electron-packager.common.camelCase)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>createAsarOpts (opts)](#apidoc.element.electron-packager.common.createAsarOpts)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>createDownloadCombos (opts, selectedPlatforms, selectedArchs, ignoreFunc)](#apidoc.element.electron-packager.common.createDownloadCombos)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>createDownloadOpts (opts, platform, arch)](#apidoc.element.electron-packager.common.createDownloadOpts)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>deprecatedParameter (properties, oldName, newName, newCLIName)](#apidoc.element.electron-packager.common.deprecatedParameter)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>downloadElectronZip (downloadOpts, cb)](#apidoc.element.electron-packager.common.downloadElectronZip)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>generateFinalBasename (opts)](#apidoc.element.electron-packager.common.generateFinalBasename)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>generateFinalPath (opts)](#apidoc.element.electron-packager.common.generateFinalPath)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>info (message, quiet)](#apidoc.element.electron-packager.common.info)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>initializeApp (opts, templatePath, appRelativePath, callback)](#apidoc.element.electron-packager.common.initializeApp)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>isPlatformMac (platform)](#apidoc.element.electron-packager.common.isPlatformMac)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>moveApp (opts, tempPath, callback)](#apidoc.element.electron-packager.common.moveApp)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>normalizeExt (filename, targetExt, cb)](#apidoc.element.electron-packager.common.normalizeExt)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>parseCLIArgs (argv)](#apidoc.element.electron-packager.common.parseCLIArgs)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>rename (basePath, oldName, newName, cb)](#apidoc.element.electron-packager.common.rename)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>sanitizeAppName (name)](#apidoc.element.electron-packager.common.sanitizeAppName)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>subOptionWarning (properties, optionName, parameter, value, quiet)](#apidoc.element.electron-packager.common.subOptionWarning)
1.  [function <span class="apidocSignatureSpan">electron-packager.common.</span>warning (message, quiet)](#apidoc.element.electron-packager.common.warning)
1.  object <span class="apidocSignatureSpan">electron-packager.common.</span>archs
1.  object <span class="apidocSignatureSpan">electron-packager.common.</span>kebabProperties
1.  object <span class="apidocSignatureSpan">electron-packager.common.</span>platforms

#### [module electron-packager.ignore](#apidoc.module.electron-packager.ignore)
1.  [function <span class="apidocSignatureSpan">electron-packager.ignore.</span>generateIgnores (opts)](#apidoc.element.electron-packager.ignore.generateIgnores)
1.  [function <span class="apidocSignatureSpan">electron-packager.ignore.</span>generateOutIgnores (opts)](#apidoc.element.electron-packager.ignore.generateOutIgnores)
1.  [function <span class="apidocSignatureSpan">electron-packager.ignore.</span>userIgnoreFilter (opts)](#apidoc.element.electron-packager.ignore.userIgnoreFilter)

#### [module electron-packager.linux](#apidoc.module.electron-packager.linux)
1.  [function <span class="apidocSignatureSpan">electron-packager.linux.</span>createApp (opts, templatePath, callback)](#apidoc.element.electron-packager.linux.createApp)

#### [module electron-packager.mac](#apidoc.module.electron-packager.mac)
1.  [function <span class="apidocSignatureSpan">electron-packager.mac.</span>createApp (opts, templatePath, callback)](#apidoc.element.electron-packager.mac.createApp)
1.  [function <span class="apidocSignatureSpan">electron-packager.mac.</span>createSignOpts (properties, platform, app, version, quiet)](#apidoc.element.electron-packager.mac.createSignOpts)
1.  [function <span class="apidocSignatureSpan">electron-packager.mac.</span>filterCFBundleIdentifier (identifier)](#apidoc.element.electron-packager.mac.filterCFBundleIdentifier)

#### [module electron-packager.targets](#apidoc.module.electron-packager.targets)
1.  [function <span class="apidocSignatureSpan">electron-packager.targets.</span>validateListFromOptions (opts, supported, name)](#apidoc.element.electron-packager.targets.validateListFromOptions)
1.  object <span class="apidocSignatureSpan">electron-packager.targets.</span>supportedArchs
1.  object <span class="apidocSignatureSpan">electron-packager.targets.</span>supportedPlatforms

#### [module electron-packager.win32](#apidoc.module.electron-packager.win32)
1.  [function <span class="apidocSignatureSpan">electron-packager.win32.</span>createApp (opts, templatePath, callback)](#apidoc.element.electron-packager.win32.createApp)
1.  [function <span class="apidocSignatureSpan">electron-packager.win32.</span>generateRceditOptionsSansIcon (opts)](#apidoc.element.electron-packager.win32.generateRceditOptionsSansIcon)
1.  [function <span class="apidocSignatureSpan">electron-packager.win32.</span>updateWineMissingException (err)](#apidoc.element.electron-packager.win32.updateWineMissingException)



# <a name="apidoc.module.electron-packager"></a>[module electron-packager](#apidoc.module.electron-packager)



# <a name="apidoc.module.electron-packager.common"></a>[module electron-packager.common](#apidoc.module.electron-packager.common)

#### <a name="apidoc.element.electron-packager.common.baseTempDir"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>baseTempDir (opts)](#apidoc.element.electron-packager.common.baseTempDir)
- description and source-code
```javascript
function baseTempDir(opts) {
  return path.join(opts.tmpdir || os.tmpdir(), 'electron-packager')
}
```
- example usage
```shell
...
function debugHostInfo () {
debug('Electron Packager ${metadata.version}')
debug('Node ${process.version}')
debug('Host Operating system: ${process.platform} (${process.arch})')
}

function createSeries (opts, archs, platforms) {
const tempBase = common.baseTempDir(opts)

function testSymlink (cb) {
  var testPath = path.join(tempBase, 'symlink-test')
  var testFile = path.join(testPath, 'test')
  var testLink = path.join(testPath, 'testlink')
  series([
    function (cb) {
...
```

#### <a name="apidoc.element.electron-packager.common.camelCase"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>camelCase (properties, warn)](#apidoc.element.electron-packager.common.camelCase)
- description and source-code
```javascript
function camelCase(properties, warn) {
  Object.keys(module.exports.kebabProperties).forEach(function (key) {
    var value = module.exports.kebabProperties[key]
    if (properties.hasOwnProperty(key)) {
      if (warn) {
        warning('The ${key} parameter is deprecated when used from JS, use ${value} instead. It will be removed in the next major
 version.')
      }
      if (!properties.hasOwnProperty(value)) {
        properties[value] = properties[key]
      }
      delete properties[key]
    }
  })
}
```
- example usage
```shell
...
  if (!Array.isArray(platforms)) return cb(platforms)

  debug('Target Platforms: ${platforms.join(', ')}')
  debug('Target Architectures: ${archs.join(', ')}')

  common.deprecatedParameter(opts, 'version', 'electronVersion', 'electron-version')

  common.camelCase(opts, true)

  getMetadataFromPackageJSON(opts, path.resolve(process.cwd(), opts.dir) || process.cwd(), function (err) {
if (err) return cb(err)

if (/ Helper$/.test(opts.name)) {
  return cb(new Error('Application names cannot end in " Helper" due to limitations on macOS'))
}
...
```

#### <a name="apidoc.element.electron-packager.common.createAsarOpts"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>createAsarOpts (opts)](#apidoc.element.electron-packager.common.createAsarOpts)
- description and source-code
```javascript
function createAsarOpts(opts) {
  let asarOptions
  if (opts.asar === true) {
    asarOptions = {}
  } else if (typeof opts.asar === 'object') {
    asarOptions = opts.asar
  } else if (opts.asar === false || opts.asar === undefined) {
    return false
  } else {
    warning('asar parameter set to an invalid value (${opts.asar}), ignoring and disabling asar')
    return false
  }

  return asarOptions
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-packager.common.createDownloadCombos"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>createDownloadCombos (opts, selectedPlatforms, selectedArchs, ignoreFunc)](#apidoc.element.electron-packager.common.createDownloadCombos)
- description and source-code
```javascript
function createDownloadCombos(opts, selectedPlatforms, selectedArchs, ignoreFunc) {
  let combinations = []
  for (let arch of selectedArchs) {
    for (let platform of selectedPlatforms) {
      // Electron does not have 32-bit releases for Mac OS X, so skip that combination
      if (isPlatformMac(platform) && arch === 'ia32') continue
      // Electron only has armv7l releases for Linux
      if (arch === 'armv7l' && platform !== 'linux') continue
      if (typeof ignoreFunc === 'function' && ignoreFunc(platform, arch)) continue
      combinations.push(createDownloadOpts(opts, platform, arch))
    }
  }

  return combinations
}
```
- example usage
```shell
...
  var tasks = []
  var useTempDir = opts.tmpdir !== false
  if (useTempDir) {
tasks.push(function (cb) {
  fs.remove(tempBase, cb)
})
  }
  return tasks.concat(common.createDownloadCombos(opts, platforms, archs).map(combination => {
var arch = combination.arch
var platform = combination.platform
var version = combination.version

return (callback) => {
  common.downloadElectronZip(combination, (err, zipPath) => {
    if (err) return callback(err)
...
```

#### <a name="apidoc.element.electron-packager.common.createDownloadOpts"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>createDownloadOpts (opts, platform, arch)](#apidoc.element.electron-packager.common.createDownloadOpts)
- description and source-code
```javascript
function createDownloadOpts(opts, platform, arch) {
  let downloadOpts = Object.assign({}, opts.download)

  subOptionWarning(downloadOpts, 'download', 'platform', platform, opts.quiet)
  subOptionWarning(downloadOpts, 'download', 'arch', arch, opts.quiet)
  subOptionWarning(downloadOpts, 'download', 'version', opts.electronVersion, opts.quiet)

  return downloadOpts
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-packager.common.deprecatedParameter"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>deprecatedParameter (properties, oldName, newName, newCLIName)](#apidoc.element.electron-packager.common.deprecatedParameter)
- description and source-code
```javascript
function deprecatedParameter(properties, oldName, newName, newCLIName) {
  if (properties.hasOwnProperty(oldName)) {
    warning('The ${oldName} parameter is deprecated, use ${newName} (or --${newCLIName} in the CLI) instead')
    if (!properties.hasOwnProperty(newName)) {
      properties[newName] = properties[oldName]
    }
    delete properties[oldName]
  }
}
```
- example usage
```shell
...
  let platforms = targets.validateListFromOptions(opts, targets.supportedPlatforms, 'platform')
  if (!Array.isArray(archs)) return cb(archs)
  if (!Array.isArray(platforms)) return cb(platforms)

  debug('Target Platforms: ${platforms.join(', ')}')
  debug('Target Architectures: ${archs.join(', ')}')

  common.deprecatedParameter(opts, 'version', 'electronVersion', 'electron-version')

  common.camelCase(opts, true)

  getMetadataFromPackageJSON(opts, path.resolve(process.cwd(), opts.dir) || process.cwd(), function (err) {
if (err) return cb(err)

if (/ Helper$/.test(opts.name)) {
...
```

#### <a name="apidoc.element.electron-packager.common.downloadElectronZip"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>downloadElectronZip (downloadOpts, cb)](#apidoc.element.electron-packager.common.downloadElectronZip)
- description and source-code
```javascript
function downloadElectronZip(downloadOpts, cb) {
  // armv7l builds have only been backfilled for Electron >= 1.0.0.
  // See: https://github.com/electron/electron/pull/6986
  if (downloadOpts.arch === 'armv7l' && semver.lt(downloadOpts.version, '1.0.0')) {
    downloadOpts.arch = 'arm'
  }
  debug('Downloading Electron with options ${JSON.stringify(downloadOpts)}')
  download(downloadOpts, cb)
}
```
- example usage
```shell
...
  }
  return tasks.concat(common.createDownloadCombos(opts, platforms, archs).map(combination => {
    var arch = combination.arch
    var platform = combination.platform
    var version = combination.version

    return (callback) => {
      common.downloadElectronZip(combination, (err, zipPath) => {
if (err) return callback(err)

function createApp (comboOpts) {
  var buildParentDir
  if (useTempDir) {
    buildParentDir = tempBase
  } else {
...
```

#### <a name="apidoc.element.electron-packager.common.generateFinalBasename"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>generateFinalBasename (opts)](#apidoc.element.electron-packager.common.generateFinalBasename)
- description and source-code
```javascript
function generateFinalBasename(opts) {
  return '${sanitizeAppName(opts.name)}-${opts.platform}-${opts.arch}'
}
```
- example usage
```shell
...
  for (let platform of common.platforms) {
    for (let arch of common.archs) {
      let basenameOpts = {
        arch: arch,
        name: opts.name,
        platform: platform
      }
      outIgnores.push(path.join(process.cwd(), common.generateFinalBasename(basenameOpts)))
    }
  }
} else {
  outIgnores.push(normalizedOut)
}

debug('Ignored paths based on the out param:', outIgnores)
...
```

#### <a name="apidoc.element.electron-packager.common.generateFinalPath"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>generateFinalPath (opts)](#apidoc.element.electron-packager.common.generateFinalPath)
- description and source-code
```javascript
function generateFinalPath(opts) {
  return path.join(opts.out || process.cwd(), generateFinalBasename(opts))
}
```
- example usage
```shell
...

if (!useTempDir) {
  createApp(comboOpts)
  return
}

function checkOverwrite () {
  var finalPath = common.generateFinalPath(comboOpts)
  fs.exists(finalPath, function (exists) {
    if (exists) {
      if (opts.overwrite) {
        fs.remove(finalPath, function () {
          createApp(comboOpts)
        })
      } else {
...
```

#### <a name="apidoc.element.electron-packager.common.info"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>info (message, quiet)](#apidoc.element.electron-packager.common.info)
- description and source-code
```javascript
function info(message, quiet) {
  if (!quiet) {
    console.error(message)
  }
}
```
- example usage
```shell
...
var buildParentDir
if (useTempDir) {
  buildParentDir = tempBase
} else {
  buildParentDir = opts.out || process.cwd()
}
var buildDir = path.join(buildParentDir, '${platform}-${arch}-template')
common.info('Packaging app for platform ${platform} ${arch} using electron v${version}', opts.quiet)
series([
  function (cb) {
    debug('Creating ${buildDir}')
    fs.mkdirs(buildDir, cb)
  },
  function (cb) {
    debug('Extracting ${zipPath} to ${buildDir}')
...
```

#### <a name="apidoc.element.electron-packager.common.initializeApp"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>initializeApp (opts, templatePath, appRelativePath, callback)](#apidoc.element.electron-packager.common.initializeApp)
- description and source-code
```javascript
function initializeApp(opts, templatePath, appRelativePath, callback) {
  // Performs the following initial operations for an app:
  // * Creates temporary directory
  // * Copies template into temporary directory
  // * Copies user's app into temporary directory
  // * Prunes non-production node_modules (if opts.prune is either truthy or undefined)
  // * Creates an asar (if opts.asar is set)

  var tempPath
  if (opts.tmpdir === false) {
    tempPath = generateFinalPath(opts)
  } else {
    tempPath = path.join(baseTempDir(opts), '${opts.platform}-${opts.arch}', generateFinalBasename(opts))
  }

  debug('Initializing app in ${tempPath} from ${templatePath} template')

  // Path to 'app' directory
  var appPath = path.join(tempPath, appRelativePath)
  var resourcesPath = path.resolve(appPath, '..')

  var operations = [
    function (cb) {
      fs.move(templatePath, tempPath, {clobber: true}, cb)
    },
    function (cb) {
      // 'deref-symlinks' is the default value so we'll use it unless
      // 'derefSymlinks' is defined.
      var shouldDeref = opts['deref-symlinks']
      if (opts.derefSymlinks !== undefined) {
        shouldDeref = opts.derefSymlinks
      }

      fs.copy(opts.dir, appPath, {filter: ignore.userIgnoreFilter(opts), dereference: shouldDeref}, cb)
    },
    function (cb) {
      var afterCopyHooks = (opts.afterCopy || []).map(function (afterCopyFn) {
        return function (cb) {
          afterCopyFn(appPath, opts.electronVersion, opts.platform, opts.arch, cb)
        }
      })
      series(afterCopyHooks, cb)
    },
    function (cb) {
      // Support removing old default_app folder that is now an asar archive
      fs.remove(path.join(resourcesPath, 'default_app'), cb)
    },
    function (cb) {
      fs.remove(path.join(resourcesPath, 'default_app.asar'), cb)
    }
  ]

  // Prune and asar are now performed before platform-specific logic, primarily so that
  // appPath is predictable (e.g. before .app is renamed for mac)
  if (opts.prune || opts.prune === undefined) {
    operations.push(function (cb) {
      debug('Running npm prune --production')
      child.exec('npm prune --production', {cwd: appPath}, cb)
    })
  }

  let asarOptions = createAsarOpts(opts)
  if (asarOptions) {
    operations.push(function (cb) {
      asarApp(appPath, asarOptions, cb)
    })
  }

  series(operations, function (err) {
    if (err) return callback(err)
    // Resolve to path to temporary app folder for platform-specific processes to use
    callback(null, tempPath)
  })
}
```
- example usage
```shell
...
'use strict'

const common = require('./common')
const path = require('path')

module.exports = {
createApp: function createApp (opts, templatePath, callback) {
  common.initializeApp(opts, templatePath, path.join('resources', 'app'), function buildLinuxApp (err, tempPath) {
    if (err) return callback(err)
    common.rename(tempPath, 'electron', common.sanitizeAppName(opts.name), function (err) {
      if (err) return callback(err)
      common.moveApp(opts, tempPath, callback)
    })
  })
}
...
```

#### <a name="apidoc.element.electron-packager.common.isPlatformMac"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>isPlatformMac (platform)](#apidoc.element.electron-packager.common.isPlatformMac)
- description and source-code
```javascript
function isPlatformMac(platform) {
  return platform === 'darwin' || platform === 'mas'
}
```
- example usage
```shell
...
      }
    } else {
      createApp(comboOpts)
    }
  })
}

if (common.isPlatformMac(combination.platform)) {
  testSymlink(function (result) {
    if (result) return checkOverwrite()

    common.info('Cannot create symlinks (on Windows hosts, it requires admin privileges); skipping ${combination.platform} platform
', opts.quiet)
    callback()
  })
} else {
...
```

#### <a name="apidoc.element.electron-packager.common.moveApp"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>moveApp (opts, tempPath, callback)](#apidoc.element.electron-packager.common.moveApp)
- description and source-code
```javascript
function finalizeApp(opts, tempPath, callback) {
  var finalPath = generateFinalPath(opts)

  if (opts.tmpdir === false) {
    callback(null, finalPath)
    return
  }

  debug('Moving ${tempPath} to ${finalPath}')
  fs.move(tempPath, finalPath, function (err) {
    callback(err, finalPath)
  })
}
```
- example usage
```shell
...

module.exports = {
  createApp: function createApp (opts, templatePath, callback) {
    common.initializeApp(opts, templatePath, path.join('resources', 'app'), function buildLinuxApp (err, tempPath) {
      if (err) return callback(err)
      common.rename(tempPath, 'electron', common.sanitizeAppName(opts.name), function (err) {
        if (err) return callback(err)
        common.moveApp(opts, tempPath, callback)
      })
    })
  }
}
...
```

#### <a name="apidoc.element.electron-packager.common.normalizeExt"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>normalizeExt (filename, targetExt, cb)](#apidoc.element.electron-packager.common.normalizeExt)
- description and source-code
```javascript
function normalizeExt(filename, targetExt, cb) {
  // Forces a filename to a given extension and fires the given callback with the normalized filename,
  // if it exists.  Otherwise reports the error from the fs.stat call.
  // (Used for resolving icon filenames, particularly during --all runs.)

  // This error path is used by win32.js if no icon is specified
  if (!filename) return cb(new Error('No filename specified to normalizeExt'))

  var ext = path.extname(filename)
  if (ext !== targetExt) {
    filename = filename.slice(0, filename.length - ext.length) + targetExt
  }

  fs.stat(filename, function (err) {
    cb(err, err ? null : filename)
  })
}
```
- example usage
```shell
...
  }), (err) => {
    callback(err)
  })
}

enqueueCopyingIcon () {
  this.operations.push((cb) => {
    common.normalizeExt(this.opts.icon, '.icns', (err, icon) => {
      if (err) {
        // Ignore error if icon doesn't exist, in case it's only available for other OS
        cb(null)
      } else {
        debug('Copying icon "${icon}" to app's Resources as "${this.appPlist.CFBundleIconFile}"')
        fs.copy(icon, path.join(this.resourcesPath, this.appPlist.CFBundleIconFile), cb)
      }
...
```

#### <a name="apidoc.element.electron-packager.common.parseCLIArgs"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>parseCLIArgs (argv)](#apidoc.element.electron-packager.common.parseCLIArgs)
- description and source-code
```javascript
function parseCLIArgs(argv) {
  var args = minimist(argv, {
    boolean: [
      'all',
      'deref-symlinks',
      'download.strictSSL',
      'overwrite',
      'prune',
      'quiet'
    ],
    default: {
      'deref-symlinks': true,
      'download.strictSSL': true,
      prune: true
    },
    string: [
      'electron-version',
      'out'
    ]
  })

  args.dir = args._[0]
  args.name = args._[1]

  // Transform hyphenated keys into camelCase
  module.exports.camelCase(args, false)

  var protocolSchemes = [].concat(args.protocol || [])
  var protocolNames = [].concat(args.protocolName || [])

  if (protocolSchemes && protocolNames && protocolNames.length === protocolSchemes.length) {
    args.protocols = protocolSchemes.map(function (scheme, i) {
      return {schemes: [scheme], name: protocolNames[i]}
    })
  }

  if (args.out === '') {
    args.out = null
  }

  // Overrides for multi-typed arguments, because minimist doesn't support it

  // asar: 'Object' or 'true'
  if (args.asar === 'true' || args.asar instanceof Array) {
    args.asar = true
  }

  // osx-sign: 'Object' or 'true'
  if (args.osxSign === 'true') {
    args.osxSign = true
  }

  // tmpdir: 'String' or 'false'
  if (args.tmpdir === 'false') {
    args.tmpdir = false
  }

  return args
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-packager.common.rename"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>rename (basePath, oldName, newName, cb)](#apidoc.element.electron-packager.common.rename)
- description and source-code
```javascript
function rename(basePath, oldName, newName, cb) {
  debug('Renaming ${oldName} to ${newName} in ${basePath}')
  fs.rename(path.join(basePath, oldName), path.join(basePath, newName), cb)
}
```
- example usage
```shell
...
    fs.stat(filename, function (err) {
      cb(err, err ? null : filename)
    })
  },

  rename: function rename (basePath, oldName, newName, cb) {
    debug('Renaming ${oldName} to ${newName} in ${basePath}')
    fs.rename(path.join(basePath, oldName), path.join(basePath, newName), cb)
  },
  sanitizeAppName: sanitizeAppName,
  warning: warning
}
...
```

#### <a name="apidoc.element.electron-packager.common.sanitizeAppName"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>sanitizeAppName (name)](#apidoc.element.electron-packager.common.sanitizeAppName)
- description and source-code
```javascript
function sanitizeAppName(name) {
  return sanitize(name, {replacement: '-'})
}
```
- example usage
```shell
...
const common = require('./common')
const path = require('path')

module.exports = {
  createApp: function createApp (opts, templatePath, callback) {
    common.initializeApp(opts, templatePath, path.join('resources', 'app'), function buildLinuxApp (err, tempPath) {
      if (err) return callback(err)
      common.rename(tempPath, 'electron', common.sanitizeAppName(opts.name), function (err) {
        if (err) return callback(err)
        common.moveApp(opts, tempPath, callback)
      })
    })
  }
}
...
```

#### <a name="apidoc.element.electron-packager.common.subOptionWarning"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>subOptionWarning (properties, optionName, parameter, value, quiet)](#apidoc.element.electron-packager.common.subOptionWarning)
- description and source-code
```javascript
function subOptionWarning(properties, optionName, parameter, value, quiet) {
  if (properties.hasOwnProperty(parameter)) {
    warning('${optionName}.${parameter} will be inferred from the main options', quiet)
  }
  properties[parameter] = value
}
```
- example usage
```shell
...
function createSignOpts (properties, platform, app, version, quiet) {
// use default sign opts if osx-sign is true, otherwise clone osx-sign object
let signOpts = properties === true ? {identity: null} : Object.assign({}, properties)

// osx-sign options are handed off to sign module, but
// with a few additions from the main options
// user may think they can pass platform, app, or version, but they will be ignored
common.subOptionWarning(signOpts, 'osx-sign', 'platform', platform, quiet)
common.subOptionWarning(signOpts, 'osx-sign', 'app', app, quiet)
common.subOptionWarning(signOpts, 'osx-sign', 'version', version, quiet)

if (signOpts.binaries) {
  common.warning('osx-sign.binaries is not an allowed sub-option. Not passing to electron-osx-sign.')
  delete signOpts.binaries
}
...
```

#### <a name="apidoc.element.electron-packager.common.warning"></a>[function <span class="apidocSignatureSpan">electron-packager.common.</span>warning (message, quiet)](#apidoc.element.electron-packager.common.warning)
- description and source-code
```javascript
function warning(message, quiet) {
  if (!quiet) {
    console.warn('WARNING: ${message}')
  }
}
```
- example usage
```shell
...
  enqueueAppSigningIfSpecified () {
let osxSignOpt = this.opts.osxSign
let platform = this.opts.platform
let version = this.opts.electronVersion

if ((platform === 'all' || platform === 'mas') &&
    osxSignOpt === undefined) {
  common.warning('signing is required for mas builds. Provide the osx-sign option, ' +
                 'or manually sign the app later.')
}

if (osxSignOpt) {
  this.operations.push((cb) => {
    let signOpts = createSignOpts(osxSignOpt, platform, this.renamedAppPath, version, this.opts.quiet)
    debug('Running electron-osx-sign with the options ${JSON.stringify(signOpts)}')
...
```



# <a name="apidoc.module.electron-packager.ignore"></a>[module electron-packager.ignore](#apidoc.module.electron-packager.ignore)

#### <a name="apidoc.element.electron-packager.ignore.generateIgnores"></a>[function <span class="apidocSignatureSpan">electron-packager.ignore.</span>generateIgnores (opts)](#apidoc.element.electron-packager.ignore.generateIgnores)
- description and source-code
```javascript
function generateIgnores(opts) {
  if (typeof (opts.ignore) !== 'function') {
    // Avoid a circular require that breaks things
    const common = require('./common')

    if (opts.ignore && !Array.isArray(opts.ignore)) opts.ignore = [opts.ignore]
    opts.ignore = (opts.ignore) ? opts.ignore.concat(DEFAULT_IGNORES) : [].concat(DEFAULT_IGNORES)
    if (process.platform === 'linux') {
      opts.ignore.push(common.baseTempDir(opts))
    }

    debug('Ignored path regular expressions:', opts.ignore)
  }
}
```
- example usage
```shell
...
    if (/ Helper$/.test(opts.name)) {
return cb(new Error('Application names cannot end in " Helper" due to limitations on macOS'))
    }

    debug('Application name: ${opts.name}')
    debug('Target Electron version: ${opts.electronVersion}')

    ignore.generateIgnores(opts)

    series(createSeries(opts, archs, platforms), function (err, appPaths) {
if (err) return cb(err)

cb(null, appPaths.filter(function (appPath) {
  // Remove falsy entries (e.g. skipped platforms)
  return appPath
...
```

#### <a name="apidoc.element.electron-packager.ignore.generateOutIgnores"></a>[function <span class="apidocSignatureSpan">electron-packager.ignore.</span>generateOutIgnores (opts)](#apidoc.element.electron-packager.ignore.generateOutIgnores)
- description and source-code
```javascript
function generateOutIgnores(opts) {
  // Avoid a circular require that breaks things
  const common = require('./common')

  let normalizedOut = opts.out ? path.resolve(opts.out) : null
  let outIgnores = []
  if (normalizedOut === null || normalizedOut === process.cwd()) {
    for (let platform of common.platforms) {
      for (let arch of common.archs) {
        let basenameOpts = {
          arch: arch,
          name: opts.name,
          platform: platform
        }
        outIgnores.push(path.join(process.cwd(), common.generateFinalBasename(basenameOpts)))
      }
    }
  } else {
    outIgnores.push(normalizedOut)
  }

  debug('Ignored paths based on the out param:', outIgnores)

  return outIgnores
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-packager.ignore.userIgnoreFilter"></a>[function <span class="apidocSignatureSpan">electron-packager.ignore.</span>userIgnoreFilter (opts)](#apidoc.element.electron-packager.ignore.userIgnoreFilter)
- description and source-code
```javascript
function userIgnoreFilter(opts) {
  var ignore = opts.ignore || []
  var ignoreFunc = null

  if (typeof (ignore) === 'function') {
    ignoreFunc = file => { return !ignore(file) }
  } else {
    if (!Array.isArray(ignore)) ignore = [ignore]

    ignoreFunc = function filterByRegexes (file) {
      for (var i = 0; i < ignore.length; i++) {
        if (file.match(ignore[i])) {
          return false
        }
      }

      return true
    }
  }

  let outIgnores = generateOutIgnores(opts)

  return function filter (file) {
    if (outIgnores.indexOf(file) !== -1) {
      return false
    }

    var name = file.split(path.resolve(opts.dir))[1]

    if (path.sep === '\\') {
      // convert slashes so unix-format ignores work
      name = name.replace(/\\/g, '/')
    }

    return ignoreFunc(name)
  }
}
```
- example usage
```shell
...
  // 'deref-symlinks' is the default value so we'll use it unless
  // 'derefSymlinks' is defined.
  var shouldDeref = opts['deref-symlinks']
  if (opts.derefSymlinks !== undefined) {
    shouldDeref = opts.derefSymlinks
  }

  fs.copy(opts.dir, appPath, {filter: ignore.userIgnoreFilter(opts), dereference: shouldDeref}, cb)
},
function (cb) {
  var afterCopyHooks = (opts.afterCopy || []).map(function (afterCopyFn) {
    return function (cb) {
      afterCopyFn(appPath, opts.electronVersion, opts.platform, opts.arch, cb)
    }
  })
...
```



# <a name="apidoc.module.electron-packager.linux"></a>[module electron-packager.linux](#apidoc.module.electron-packager.linux)

#### <a name="apidoc.element.electron-packager.linux.createApp"></a>[function <span class="apidocSignatureSpan">electron-packager.linux.</span>createApp (opts, templatePath, callback)](#apidoc.element.electron-packager.linux.createApp)
- description and source-code
```javascript
function createApp(opts, templatePath, callback) {
  common.initializeApp(opts, templatePath, path.join('resources', 'app'), function buildLinuxApp (err, tempPath) {
    if (err) return callback(err)
    common.rename(tempPath, 'electron', common.sanitizeAppName(opts.name), function (err) {
      if (err) return callback(err)
      common.moveApp(opts, tempPath, callback)
    })
  })
}
```
- example usage
```shell
...
        var newFunctions = opts.afterExtract.map(function (fn) {
          return fn.bind(this, buildDir, version, platform, arch)
        })
        series(newFunctions, cb)
      }
    }
  ], function () {
    require(targets.supportedPlatforms[platform]).createApp(comboOpts, buildDir, callback)
  })
}

// Create delegated options object with specific platform and arch, for output directory naming
var comboOpts = Object.create(opts)
comboOpts.arch = arch
comboOpts.platform = platform
...
```



# <a name="apidoc.module.electron-packager.mac"></a>[module electron-packager.mac](#apidoc.module.electron-packager.mac)

#### <a name="apidoc.element.electron-packager.mac.createApp"></a>[function <span class="apidocSignatureSpan">electron-packager.mac.</span>createApp (opts, templatePath, callback)](#apidoc.element.electron-packager.mac.createApp)
- description and source-code
```javascript
function createApp(opts, templatePath, callback) {
  let appRelativePath = path.join('Electron.app', 'Contents', 'Resources', 'app')
  common.initializeApp(opts, templatePath, appRelativePath, function buildMacApp (err, stagingPath) {
    if (err) return callback(err)

    let appCreator = new MacApp(opts, stagingPath)
    appCreator.updatePlistFiles()

    if (opts.icon) {
      appCreator.enqueueCopyingIcon()
    }

    if (opts.extraResource) {
      appCreator.enqueueCopyingExtraFiles(opts.extraResource)
    }

    appCreator.enqueueRenamingElectronBinary()
    appCreator.enqueueRenamingAppAndHelpers()
    appCreator.enqueueAppSigningIfSpecified()

    return appCreator.executeOperations(callback)
  })
}
```
- example usage
```shell
...
        var newFunctions = opts.afterExtract.map(function (fn) {
          return fn.bind(this, buildDir, version, platform, arch)
        })
        series(newFunctions, cb)
      }
    }
  ], function () {
    require(targets.supportedPlatforms[platform]).createApp(comboOpts, buildDir, callback)
  })
}

// Create delegated options object with specific platform and arch, for output directory naming
var comboOpts = Object.create(opts)
comboOpts.arch = arch
comboOpts.platform = platform
...
```

#### <a name="apidoc.element.electron-packager.mac.createSignOpts"></a>[function <span class="apidocSignatureSpan">electron-packager.mac.</span>createSignOpts (properties, platform, app, version, quiet)](#apidoc.element.electron-packager.mac.createSignOpts)
- description and source-code
```javascript
function createSignOpts(properties, platform, app, version, quiet) {
  // use default sign opts if osx-sign is true, otherwise clone osx-sign object
  let signOpts = properties === true ? {identity: null} : Object.assign({}, properties)

  // osx-sign options are handed off to sign module, but
  // with a few additions from the main options
  // user may think they can pass platform, app, or version, but they will be ignored
  common.subOptionWarning(signOpts, 'osx-sign', 'platform', platform, quiet)
  common.subOptionWarning(signOpts, 'osx-sign', 'app', app, quiet)
  common.subOptionWarning(signOpts, 'osx-sign', 'version', version, quiet)

  if (signOpts.binaries) {
    common.warning('osx-sign.binaries is not an allowed sub-option. Not passing to electron-osx-sign.')
    delete signOpts.binaries
  }

  // Take argument osx-sign as signing identity:
  // if opts.osxSign is true (bool), fallback to identity=null for
  // autodiscovery. Otherwise, provide signing certificate info.
  if (signOpts.identity === true) {
    signOpts.identity = null
  }

  return signOpts
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-packager.mac.filterCFBundleIdentifier"></a>[function <span class="apidocSignatureSpan">electron-packager.mac.</span>filterCFBundleIdentifier (identifier)](#apidoc.element.electron-packager.mac.filterCFBundleIdentifier)
- description and source-code
```javascript
function filterCFBundleIdentifier(identifier) {
  return identifier.replace(/ /g, '-').replace(/[^a-zA-Z0-9.-]/g, '')
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.electron-packager.targets"></a>[module electron-packager.targets](#apidoc.module.electron-packager.targets)

#### <a name="apidoc.element.electron-packager.targets.validateListFromOptions"></a>[function <span class="apidocSignatureSpan">electron-packager.targets.</span>validateListFromOptions (opts, supported, name)](#apidoc.element.electron-packager.targets.validateListFromOptions)
- description and source-code
```javascript
function validateListFromOptions(opts, supported, name) {
  if (opts.all) return Object.keys(supported)

  let list = opts[name] || process[name]
  if (list === 'all') return Object.keys(supported)

  if (!Array.isArray(list)) {
    if (typeof list === 'string') {
      list = list.split(',')
    } else {
      return unsupportedListOption(name, list, supported)
    }
  }

  for (let value of list) {
    if (!supported[value]) {
      return unsupportedListOption(name, value, supported)
    }
  }

  return list
}
```
- example usage
```shell
...
}))
}

module.exports = function packager (opts, cb) {
debugHostInfo()
if (debug.enabled) debug('Packager Options: ${JSON.stringify(opts)}')

let archs = targets.validateListFromOptions(opts, targets.supportedArchs, 'arch')
let platforms = targets.validateListFromOptions(opts, targets.supportedPlatforms, 'platform')
if (!Array.isArray(archs)) return cb(archs)
if (!Array.isArray(platforms)) return cb(platforms)

debug('Target Platforms: ${platforms.join(', ')}')
debug('Target Architectures: ${archs.join(', ')}')
...
```



# <a name="apidoc.module.electron-packager.win32"></a>[module electron-packager.win32](#apidoc.module.electron-packager.win32)

#### <a name="apidoc.element.electron-packager.win32.createApp"></a>[function <span class="apidocSignatureSpan">electron-packager.win32.</span>createApp (opts, templatePath, callback)](#apidoc.element.electron-packager.win32.createApp)
- description and source-code
```javascript
function createApp(opts, templatePath, callback) {
  common.initializeApp(opts, templatePath, path.join('resources', 'app'), function buildWinApp (err, tempPath) {
    if (err) return callback(err)

    let newExeName = '${common.sanitizeAppName(opts.name)}.exe'
    var operations = [
      function (cb) {
        common.rename(tempPath, 'electron.exe', newExeName, cb)
      }
    ]

    const rcOpts = generateRceditOptionsSansIcon(opts)

    if (opts.icon || opts.win32metadata || opts['version-string'] || opts.appCopyright || opts.appVersion || opts.buildVersion) {
      operations.push(function (cb) {
        common.normalizeExt(opts.icon, '.ico', function (err, icon) {
          // Icon might be omitted or only exist in one OS's format, so skip it if normalizeExt reports an error
          if (!err) {
            rcOpts.icon = icon
          }

          debug('Running rcedit with the options ${JSON.stringify(rcOpts)}')
          require('rcedit')(path.join(tempPath, newExeName), rcOpts, function (err) {
            cb(updateWineMissingException(err))
          })
        })
      })
    }

    series(operations, function (err) {
      if (err) return callback(err)
      common.moveApp(opts, tempPath, callback)
    })
  })
}
```
- example usage
```shell
...
        var newFunctions = opts.afterExtract.map(function (fn) {
          return fn.bind(this, buildDir, version, platform, arch)
        })
        series(newFunctions, cb)
      }
    }
  ], function () {
    require(targets.supportedPlatforms[platform]).createApp(comboOpts, buildDir, callback)
  })
}

// Create delegated options object with specific platform and arch, for output directory naming
var comboOpts = Object.create(opts)
comboOpts.arch = arch
comboOpts.platform = platform
...
```

#### <a name="apidoc.element.electron-packager.win32.generateRceditOptionsSansIcon"></a>[function <span class="apidocSignatureSpan">electron-packager.win32.</span>generateRceditOptionsSansIcon (opts)](#apidoc.element.electron-packager.win32.generateRceditOptionsSansIcon)
- description and source-code
```javascript
function generateRceditOptionsSansIcon(opts) {
  const win32metadata = Object.assign({}, opts['version-string'], opts.win32metadata)

  let rcOpts = {'version-string': win32metadata}

  if (opts.appVersion) {
    rcOpts['product-version'] = rcOpts['file-version'] = opts.appVersion
  }

  if (opts.buildVersion) {
    rcOpts['file-version'] = opts.buildVersion
  }

  if (opts.appCopyright) {
    rcOpts['version-string'].LegalCopyright = opts.appCopyright
  }

  return rcOpts
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.electron-packager.win32.updateWineMissingException"></a>[function <span class="apidocSignatureSpan">electron-packager.win32.</span>updateWineMissingException (err)](#apidoc.element.electron-packager.win32.updateWineMissingException)
- description and source-code
```javascript
function updateWineMissingException(err) {
  if (err && err.code === 'ENOENT' && err.syscall === 'spawn wine') {
    err.message = 'Could not find "wine" on your system.\n\n' +
      'Wine is required to use the app-copyright, app-version, build-version, icon, and \n' +
      'win32metadata parameters for Windows targets.\n\n' +
      'Make sure that the "wine" executable is in your PATH.\n\n' +
      'See https://github.com/electron-userland/electron-packager#building-windows-apps-from-non-windows-platforms for details.'
  }

  return err
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
