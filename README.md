# api documentation for  [spotify-web-api-node (v2.3.6)](https://github.com/thelinmichael/spotify-web-api-node)  [![npm package](https://img.shields.io/npm/v/npmdoc-spotify-web-api-node.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-spotify-web-api-node) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-spotify-web-api-node.svg)](https://travis-ci.org/npmdoc/node-npmdoc-spotify-web-api-node)
#### A Node.js wrapper for Spotify's Web API

[![NPM](https://nodei.co/npm/spotify-web-api-node.png?downloads=true)](https://www.npmjs.com/package/spotify-web-api-node)

[![apidoc](https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-spotify-web-api-node_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-spotify-web-api-node/build/apidoc.html)

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
            "name": "thelinmichael",
            "email": "thelinmichael@gmail.com"
        },
        {
            "name": "jmperez",
            "email": "jmperez1985@gmail.com"
        }
    ],
    "name": "spotify-web-api-node",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module spotify-web-api-node](#apidoc.module.spotify-web-api-node)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.</span>_addMethods (methods)](#apidoc.element.spotify-web-api-node._addMethods)
1.  object <span class="apidocSignatureSpan">spotify-web-api-node.</span>authentication_request
1.  object <span class="apidocSignatureSpan">spotify-web-api-node.</span>base_request
1.  object <span class="apidocSignatureSpan">spotify-web-api-node.</span>http_manager
1.  object <span class="apidocSignatureSpan">spotify-web-api-node.</span>server_methods
1.  object <span class="apidocSignatureSpan">spotify-web-api-node.</span>webapi_request

#### [module spotify-web-api-node.authentication_request](#apidoc.module.spotify-web-api-node.authentication_request)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.authentication_request.</span>builder ()](#apidoc.element.spotify-web-api-node.authentication_request.builder)

#### [module spotify-web-api-node.base_request](#apidoc.module.spotify-web-api-node.base_request)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.base_request.</span>builder ()](#apidoc.element.spotify-web-api-node.base_request.builder)

#### [module spotify-web-api-node.http_manager](#apidoc.module.spotify-web-api-node.http_manager)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.http_manager.</span>_makeRequest (method, options, uri, callback)](#apidoc.element.spotify-web-api-node.http_manager._makeRequest)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.http_manager.</span>del (request, callback)](#apidoc.element.spotify-web-api-node.http_manager.del)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.http_manager.</span>get (request, callback)](#apidoc.element.spotify-web-api-node.http_manager.get)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.http_manager.</span>post (request, callback)](#apidoc.element.spotify-web-api-node.http_manager.post)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.http_manager.</span>put (request, callback)](#apidoc.element.spotify-web-api-node.http_manager.put)

#### [module spotify-web-api-node.server_methods](#apidoc.module.spotify-web-api-node.server_methods)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.server_methods.</span>authorizationCodeGrant (code, callback)](#apidoc.element.spotify-web-api-node.server_methods.authorizationCodeGrant)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.server_methods.</span>clientCredentialsGrant (options, callback)](#apidoc.element.spotify-web-api-node.server_methods.clientCredentialsGrant)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.server_methods.</span>refreshAccessToken (callback)](#apidoc.element.spotify-web-api-node.server_methods.refreshAccessToken)

#### [module spotify-web-api-node.webapi_request](#apidoc.module.spotify-web-api-node.webapi_request)
1.  [function <span class="apidocSignatureSpan">spotify-web-api-node.webapi_request.</span>builder ()](#apidoc.element.spotify-web-api-node.webapi_request.builder)



# <a name="apidoc.module.spotify-web-api-node"></a>[module spotify-web-api-node](#apidoc.module.spotify-web-api-node)

#### <a name="apidoc.element.spotify-web-api-node._addMethods"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.</span>_addMethods (methods)](#apidoc.element.spotify-web-api-node._addMethods)
- description and source-code
```javascript
_addMethods = function (methods) {
  for (var i in methods) {
    if (methods.hasOwnProperty(i)) {
      this.prototype[i] = methods[i];
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spotify-web-api-node.authentication_request"></a>[module spotify-web-api-node.authentication_request](#apidoc.module.spotify-web-api-node.authentication_request)

#### <a name="apidoc.element.spotify-web-api-node.authentication_request.builder"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.authentication_request.</span>builder ()](#apidoc.element.spotify-web-api-node.authentication_request.builder)
- description and source-code
```javascript
builder = function () {
  return Request.builder()
      .withHost(DEFAULT_HOST)
      .withPort(DEFAULT_PORT)
      .withScheme(DEFAULT_SCHEME);
}
```
- example usage
```shell
...
var Request = require('./base-request');

var DEFAULT_HOST = 'accounts.spotify.com',
    DEFAULT_PORT = 443,
    DEFAULT_SCHEME = 'https';

module.exports.builder = function() {
  return Request.builder()
      .withHost(DEFAULT_HOST)
      .withPort(DEFAULT_PORT)
      .withScheme(DEFAULT_SCHEME);
};
...
```



# <a name="apidoc.module.spotify-web-api-node.base_request"></a>[module spotify-web-api-node.base_request](#apidoc.module.spotify-web-api-node.base_request)

#### <a name="apidoc.element.spotify-web-api-node.base_request.builder"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.base_request.</span>builder ()](#apidoc.element.spotify-web-api-node.base_request.builder)
- description and source-code
```javascript
builder = function () {
  return new Builder();
}
```
- example usage
```shell
...
var Request = require('./base-request');

var DEFAULT_HOST = 'accounts.spotify.com',
    DEFAULT_PORT = 443,
    DEFAULT_SCHEME = 'https';

module.exports.builder = function() {
  return Request.builder()
      .withHost(DEFAULT_HOST)
      .withPort(DEFAULT_PORT)
      .withScheme(DEFAULT_SCHEME);
};
...
```



# <a name="apidoc.module.spotify-web-api-node.http_manager"></a>[module spotify-web-api-node.http_manager](#apidoc.module.spotify-web-api-node.http_manager)

#### <a name="apidoc.element.spotify-web-api-node.http_manager._makeRequest"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.http_manager.</span>_makeRequest (method, options, uri, callback)](#apidoc.element.spotify-web-api-node.http_manager._makeRequest)
- description and source-code
```javascript
_makeRequest = function (method, options, uri, callback) {
  var req = method(uri);

  if (options.query) {
    req.query(options.query);
  }

  if (options.data && (!options.headers || options.headers['Content-Type'] !== 'application/json')) {
    req.type('form');
    req.send(options.data);
  } else if (options.data) {
    req.send(options.data);
  }

  if (options.headers) {
    req.set(options.headers);
  }

  req.end(function (err, response) {
    if (err) {
      var errorObject = _getErrorObject('Request error', {
        error: err
      });
      return callback(errorObject);
    }

    return callback(null, {
      body: response.body,
      headers: response.headers,
      statusCode: response.statusCode
    });
  });
}
```
- example usage
```shell
...
* @param {BaseRequest} The request.
* @param {Function} The callback function.
*/
HttpManager.get = function(request, callback) {
 var options = _getParametersFromRequest(request);
 var method = superagent.get;

 HttpManager._makeRequest(method, options, request.getURI(), callback);
};

/**
* Make a HTTP POST request.
* @param {BaseRequest} The request.
* @param {Function} The callback function.
*/
...
```

#### <a name="apidoc.element.spotify-web-api-node.http_manager.del"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.http_manager.</span>del (request, callback)](#apidoc.element.spotify-web-api-node.http_manager.del)
- description and source-code
```javascript
del = function (request, callback) {

  var options = _getParametersFromRequest(request);
  var method = superagent.del;

  HttpManager._makeRequest(method, options, request.getURI(), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spotify-web-api-node.http_manager.get"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.http_manager.</span>get (request, callback)](#apidoc.element.spotify-web-api-node.http_manager.get)
- description and source-code
```javascript
get = function (request, callback) {
  var options = _getParametersFromRequest(request);
  var method = superagent.get;

  HttpManager._makeRequest(method, options, request.getURI(), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spotify-web-api-node.http_manager.post"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.http_manager.</span>post (request, callback)](#apidoc.element.spotify-web-api-node.http_manager.post)
- description and source-code
```javascript
post = function (request, callback) {

  var options = _getParametersFromRequest(request);
  var method = superagent.post;

  HttpManager._makeRequest(method, options, request.getURI(), callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spotify-web-api-node.http_manager.put"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.http_manager.</span>put (request, callback)](#apidoc.element.spotify-web-api-node.http_manager.put)
- description and source-code
```javascript
put = function (request, callback) {

  var options = _getParametersFromRequest(request);
  var method = superagent.put;

  HttpManager._makeRequest(method, options, request.getURI(), callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spotify-web-api-node.server_methods"></a>[module spotify-web-api-node.server_methods](#apidoc.module.spotify-web-api-node.server_methods)

#### <a name="apidoc.element.spotify-web-api-node.server_methods.authorizationCodeGrant"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.server_methods.</span>authorizationCodeGrant (code, callback)](#apidoc.element.spotify-web-api-node.server_methods.authorizationCodeGrant)
- description and source-code
```javascript
authorizationCodeGrant = function (code, callback) {
  var request = AuthenticationRequest.builder()
    .withPath('/api/token')
    .withBodyParameters({
      'grant_type' : 'authorization_code',
      'redirect_uri' : this.getRedirectURI(),
      'code' : code,
      'client_id' : this.getClientId(),
      'client_secret' : this.getClientSecret()
    })
    .build();

  var promise = this._performRequest(HttpManager.post, request);

  if (callback) {
    promise.then(function(data) {
      callback(null, data);
    }, function(err) {
      callback(err);
    });
  } else {
    return promise;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spotify-web-api-node.server_methods.clientCredentialsGrant"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.server_methods.</span>clientCredentialsGrant (options, callback)](#apidoc.element.spotify-web-api-node.server_methods.clientCredentialsGrant)
- description and source-code
```javascript
clientCredentialsGrant = function (options, callback) {
  var request = AuthenticationRequest.builder()
    .withPath('/api/token')
    .withBodyParameters({
      'grant_type' : 'client_credentials'
    })
    .withHeaders({
      Authorization : ('Basic ' + new Buffer(this.getClientId() + ':' + this.getClientSecret()).toString('base64'))
    })
    .build();

  this._addBodyParameters(request, options);

  var promise =  this._performRequest(HttpManager.post, request);

  if (callback) {
    promise.then(function(data) {
      callback(null, data);
    }, function(err) {
      callback(err);
    });
  } else {
    return promise;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.spotify-web-api-node.server_methods.refreshAccessToken"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.server_methods.</span>refreshAccessToken (callback)](#apidoc.element.spotify-web-api-node.server_methods.refreshAccessToken)
- description and source-code
```javascript
refreshAccessToken = function (callback) {
  var request = AuthenticationRequest.builder()
    .withPath('/api/token')
    .withBodyParameters({
      'grant_type' : 'refresh_token',
      'refresh_token' : this.getRefreshToken()
    })
    .withHeaders({
      Authorization : ('Basic ' + new Buffer(this.getClientId() + ':' + this.getClientSecret()).toString('base64'))
    })
    .build();

  var promise = this._performRequest(HttpManager.post, request);

  if (callback) {
    promise.then(function(data) {
      callback(null, data);
    }, function(err) {
      callback(err);
    });
  } else {
    return promise;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.spotify-web-api-node.webapi_request"></a>[module spotify-web-api-node.webapi_request](#apidoc.module.spotify-web-api-node.webapi_request)

#### <a name="apidoc.element.spotify-web-api-node.webapi_request.builder"></a>[function <span class="apidocSignatureSpan">spotify-web-api-node.webapi_request.</span>builder ()](#apidoc.element.spotify-web-api-node.webapi_request.builder)
- description and source-code
```javascript
builder = function () {
  return Request.builder()
      .withHost(DEFAULT_HOST)
      .withPort(DEFAULT_PORT)
      .withScheme(DEFAULT_SCHEME);
}
```
- example usage
```shell
...
var Request = require('./base-request');

var DEFAULT_HOST = 'accounts.spotify.com',
    DEFAULT_PORT = 443,
    DEFAULT_SCHEME = 'https';

module.exports.builder = function() {
  return Request.builder()
      .withHost(DEFAULT_HOST)
      .withPort(DEFAULT_PORT)
      .withScheme(DEFAULT_SCHEME);
};
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
