# npmdoc-spotify-web-api-node

#### api documentation for  [spotify-web-api-node (v2.3.6)](https://github.com/thelinmichael/spotify-web-api-node)  [![npm package](https://img.shields.io/npm/v/npmdoc-spotify-web-api-node.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-spotify-web-api-node) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-spotify-web-api-node.svg)](https://travis-ci.org/npmdoc/node-npmdoc-spotify-web-api-node)

#### A Node.js wrapper for Spotify's Web API

[![NPM](https://nodei.co/npm/spotify-web-api-node.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/spotify-web-api-node)

- [https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Michael Thelin"
    },
    "browser": {
        "./src/server.js": "./src/client.js"
    },
    "bugs": {
        "url": "https://github.com/thelinmichael/spotify-web-api-node/issues"
    },
    "config": {
        "blanket": {
            "pattern": "src",
            "data-cover-never": "node_modules"
        }
    },
    "dependencies": {
        "superagent": "^2.0.0"
    },
    "description": "A Node.js wrapper for Spotify's Web API",
    "devDependencies": {
        "blanket": "^1.1.7",
        "coveralls": "^2.11.2",
        "grunt": "^1.0.1",
        "grunt-contrib-jshint": "~0.11.0",
        "grunt-contrib-watch": "~0.6",
        "grunt-simple-mocha": "0.4.x",
        "mocha": "~1.20.1",
        "mocha-lcov-reporter": "0.0.2",
        "mockery": "^1.4.0",
        "should": "~3.0",
        "sinon": "~1.12.2",
        "xunit-file": "0.0.5"
    },
    "directories": {},
    "dist": {
        "shasum": "7c79e4045ec412869e89f6ba6ab816a3d4c322cc",
        "tarball": "https://registry.npmjs.org/spotify-web-api-node/-/spotify-web-api-node-2.3.6.tgz"
    },
    "gitHead": "dad2b832f734b0c23c55237e680cda4d08cc1fe0",
    "homepage": "https://github.com/thelinmichael/spotify-web-api-node",
    "keywords": [
        "spotify",
        "echonest",
        "music",
        "api",
        "wrapper",
        "client",
        "web api"
    ],
    "license": "MIT",
    "main": "./src/server.js",
    "maintainers": [
        {
            "name": "thelinmichael"
        },
        {
            "name": "jmperez"
        }
    ],
    "name": "spotify-web-api-node",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/thelinmichael/spotify-web-api-node.git"
    },
    "scripts": {
        "coveralls": "mocha -r blanket -R mocha-lcov-reporter | ./node_modules/coveralls/bin/coveralls.js",
        "lint": "grunt jshint",
        "test": "npm run lint && ./node_modules/.bin/mocha --bail"
    },
    "version": "2.3.6"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
