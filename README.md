# api documentation for  [request-promise (v4.2.0)](https://github.com/request/request-promise#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-request-promise.svg)](https://travis-ci.org/npmdoc/node-npmdoc-request-promise)
#### The simplified HTTP request client 'request' with Promise support. Powered by Bluebird.

[![NPM](https://nodei.co/npm/request-promise.png?downloads=true)](https://www.npmjs.com/package/request-promise)

[![apidoc](https://npmdoc.github.io/node-npmdoc-request-promise/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-request_promise_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-request-promise/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-request-promise/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Nicolai Kamenzky",
        "url": "https://github.com/analog-nico"
    },
    "bugs": {
        "url": "https://github.com/request/request-promise/issues"
    },
    "dependencies": {
        "bluebird": "^3.5.0",
        "request-promise-core": "1.1.1",
        "stealthy-require": "^1.0.0"
    },
    "description": "The simplified HTTP request client 'request' with Promise support. Powered by Bluebird.",
    "devDependencies": {
        "body-parser": "~1.15.2",
        "chai": "~3.5.0",
        "chalk": "~1.1.3",
        "gulp": "~3.9.1",
        "gulp-coveralls": "~0.1.4",
        "gulp-eslint": "~2.1.0",
        "gulp-istanbul": "~1.0.0",
        "gulp-mocha": "~2.2.0",
        "lodash": "~4.13.1",
        "publish-please": "~2.1.4",
        "request": "^2.34.0",
        "rimraf": "~2.5.3",
        "run-sequence": "~1.2.2"
    },
    "directories": {},
    "dist": {
        "shasum": "684f77748d6b4617bee6a4ef4469906e6d074720",
        "tarball": "https://registry.npmjs.org/request-promise/-/request-promise-4.2.0.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "b5e06f5657b14d2640acd1aa2c778d330a3afc12",
    "homepage": "https://github.com/request/request-promise#readme",
    "keywords": [
        "xhr",
        "http",
        "https",
        "promise",
        "request",
        "then",
        "thenable",
        "bluebird"
    ],
    "license": "ISC",
    "main": "./lib/rp.js",
    "maintainers": [
        {
            "name": "analog-nico",
            "email": "nicolai.kamenzky@testrails.org"
        },
        {
            "name": "mikeal",
            "email": "mikeal.rogers@gmail.com"
        },
        {
            "name": "nylen",
            "email": "jnylen@gmail.com"
        },
        {
            "name": "request",
            "email": "request@outofindex.com"
        },
        {
            "name": "simov",
            "email": "simeonvelichkov@gmail.com"
        },
        {
            "name": "tyabonil",
            "email": "ty.abonil@gmail.com"
        }
    ],
    "name": "request-promise",
    "optionalDependencies": {},
    "peerDependencies": {
        "request": "^2.34"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/request/request-promise.git"
    },
    "scripts": {
        "prepublish": "publish-please guard",
        "publish-please": "publish-please",
        "test": "gulp ci",
        "test-publish": "gulp ci-no-cov"
    },
    "version": "4.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module request-promise](#apidoc.module.request-promise)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>Request (options)](#apidoc.element.request-promise.Request)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>bindCLS ()](#apidoc.element.request-promise.bindCLS)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>cookie (str)](#apidoc.element.request-promise.cookie)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>defaults (options, requester)](#apidoc.element.request-promise.defaults)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>del (uri, options, callback)](#apidoc.element.request-promise.del)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>delete (uri, options, callback)](#apidoc.element.request-promise.delete)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>forever (agentOptions, optionsArg)](#apidoc.element.request-promise.forever)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>get (uri, options, callback)](#apidoc.element.request-promise.get)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>head (uri, options, callback)](#apidoc.element.request-promise.head)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>initParams (uri, options, callback)](#apidoc.element.request-promise.initParams)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>jar (store)](#apidoc.element.request-promise.jar)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>patch (uri, options, callback)](#apidoc.element.request-promise.patch)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>post (uri, options, callback)](#apidoc.element.request-promise.post)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>put (uri, options, callback)](#apidoc.element.request-promise.put)
1.  object <span class="apidocSignatureSpan">request-promise.</span>Request.prototype

#### [module request-promise.Request](#apidoc.module.request-promise.Request)
1.  [function <span class="apidocSignatureSpan">request-promise.</span>Request (options)](#apidoc.element.request-promise.Request.Request)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.</span>super_ ()](#apidoc.element.request-promise.Request.super_)
1.  object <span class="apidocSignatureSpan">request-promise.Request.</span>defaultProxyHeaderExclusiveList
1.  object <span class="apidocSignatureSpan">request-promise.Request.</span>defaultProxyHeaderWhiteList

#### [module request-promise.Request.prototype](#apidoc.module.request-promise.Request.prototype)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>abort ()](#apidoc.element.request-promise.Request.prototype.abort)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>auth (user, pass, sendImmediately, bearer)](#apidoc.element.request-promise.Request.prototype.auth)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>aws (opts, now)](#apidoc.element.request-promise.Request.prototype.aws)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>cancel ()](#apidoc.element.request-promise.Request.prototype.cancel)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>catch ()](#apidoc.element.request-promise.Request.prototype.catch)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>debug ()](#apidoc.element.request-promise.Request.prototype.debug)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>destroy ()](#apidoc.element.request-promise.Request.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>enableUnixSocket ()](#apidoc.element.request-promise.Request.prototype.enableUnixSocket)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>end (chunk)](#apidoc.element.request-promise.Request.prototype.end)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>finally ()](#apidoc.element.request-promise.Request.prototype.finally)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>form (form)](#apidoc.element.request-promise.Request.prototype.form)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>getHeader (name, headers)](#apidoc.element.request-promise.Request.prototype.getHeader)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>getNewAgent ()](#apidoc.element.request-promise.Request.prototype.getNewAgent)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>hawk (opts)](#apidoc.element.request-promise.Request.prototype.hawk)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>httpSignature (opts)](#apidoc.element.request-promise.Request.prototype.httpSignature)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>init (requestOptions)](#apidoc.element.request-promise.Request.prototype.init)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>jar (jar)](#apidoc.element.request-promise.Request.prototype.jar)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>json (val)](#apidoc.element.request-promise.Request.prototype.json)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>multipart (multipart)](#apidoc.element.request-promise.Request.prototype.multipart)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>oauth (_oauth)](#apidoc.element.request-promise.Request.prototype.oauth)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>onRequestError (error)](#apidoc.element.request-promise.Request.prototype.onRequestError)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>onRequestResponse (response)](#apidoc.element.request-promise.Request.prototype.onRequestResponse)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>pause ()](#apidoc.element.request-promise.Request.prototype.pause)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>pipe (dest, opts)](#apidoc.element.request-promise.Request.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>pipeDest (dest)](#apidoc.element.request-promise.Request.prototype.pipeDest)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>promise ()](#apidoc.element.request-promise.Request.prototype.promise)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>qs (q, clobber)](#apidoc.element.request-promise.Request.prototype.qs)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>readResponseBody (response)](#apidoc.element.request-promise.Request.prototype.readResponseBody)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>resume ()](#apidoc.element.request-promise.Request.prototype.resume)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>start ()](#apidoc.element.request-promise.Request.prototype.start)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>then ()](#apidoc.element.request-promise.Request.prototype.then)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>toJSON ()](#apidoc.element.request-promise.Request.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>write ()](#apidoc.element.request-promise.Request.prototype.write)



# <a name="apidoc.module.request-promise"></a>[module request-promise](#apidoc.module.request-promise)

#### <a name="apidoc.element.request-promise.Request"></a>[function <span class="apidocSignatureSpan">request-promise.</span>Request (options)](#apidoc.element.request-promise.Request)
- description and source-code
```javascript
function Request(options) {
  // if given the method property in options, set property explicitMethod to true

  // extend the Request instance with any non-reserved properties
  // remove any reserved functions from the options object
  // set Request instance to be readable and writable
  // call init

  var self = this

  // start with HAR, then override with additional options
  if (options.har) {
    self._har = new Har(self)
    options = self._har.options(options)
  }

  stream.Stream.call(self)
  var reserved = Object.keys(Request.prototype)
  var nonReserved = filterForNonReserved(reserved, options)

  extend(self, nonReserved)
  options = filterOutReservedFunctions(reserved, options)

  self.readable = true
  self.writable = true
  if (options.method) {
    self.explicitMethod = true
  }
  self._qs = new Querystring(self)
  self._auth = new Auth(self)
  self._oauth = new OAuth(self)
  self._multipart = new Multipart(self)
  self._redirect = new Redirect(self)
  self._tunnel = new Tunnel(self)
  self.init(options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.bindCLS"></a>[function <span class="apidocSignatureSpan">request-promise.</span>bindCLS ()](#apidoc.element.request-promise.bindCLS)
- description and source-code
```javascript
function RP$bindCLS() {
    throw new Error('CLS support was dropped. To get it back read: https://github.com/request/request-promise/wiki/Getting-Back-
Support-for-Continuation-Local-Storage');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.cookie"></a>[function <span class="apidocSignatureSpan">request-promise.</span>cookie (str)](#apidoc.element.request-promise.cookie)
- description and source-code
```javascript
cookie = function (str) {
  return cookies.parse(str)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.defaults"></a>[function <span class="apidocSignatureSpan">request-promise.</span>defaults (options, requester)](#apidoc.element.request-promise.defaults)
- description and source-code
```javascript
defaults = function (options, requester) {
  var self = this

  options = options || {}

  if (typeof options === 'function') {
    requester = options
    options = {}
  }

  var defaults      = wrapRequestMethod(self, options, requester)

  var verbs = ['get', 'head', 'post', 'put', 'patch', 'del', 'delete']
  verbs.forEach(function(verb) {
    defaults[verb]  = wrapRequestMethod(self[verb], options, requester, verb)
  })

  defaults.cookie   = wrapRequestMethod(self.cookie, options, requester)
  defaults.jar      = self.jar
  defaults.defaults = self.defaults
  return defaults
}
```
- example usage
```shell
...
rp(options)
    .then(function (autoParsedBody) {
        // :)
    });


// You can go one step further and set the transform as the default:
var rpap = rp.defaults({ transform: autoParse });

rpap('http://google.com')
    .then(function (autoParsedBody) {
        // :)
    });

rpap('http://echojs.com')
...
```

#### <a name="apidoc.element.request-promise.del"></a>[function <span class="apidocSignatureSpan">request-promise.</span>del (uri, options, callback)](#apidoc.element.request-promise.del)
- description and source-code
```javascript
del = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...
Consider Request-Promise being:

- A Request object
	- With an [identical API](https://github.com/request/request): 'require('request-promise') == require('request')' so to say
	- However, **STREAMING THE RESPONSE** (e.g. '.pipe(...)') is **DISCOURAGED** because Request-Promise would grow the memory footprint
 for large requests unnecessarily high. Use the original Request library for that. You can use both libraries in the same project
.
- Plus some methods on a request call object:
	- 'rp(...).then(...)' or e.g. 'rp.post(...).then(...)' which turn 'rp(...)' and 'rp.post(...)' into promises
	- 'rp(...).catch(...)' or e.g. 'rp.del(...).catch(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).finally(...)' or e.g. 'rp.put(...).finally(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).cancel()' or e.g. 'rp.get(...).cancel()' which cancels the request
	- 'rp(...).promise()' or e.g. 'rp.head(...).promise()' which returns the underlying promise so you can access the full [Bluebird
 API](https://github.com/petkaantonov/bluebird/blob/master/API.md)
- Plus some additional options:
	- 'simple = true' which is a boolean to set whether status codes other than 2xx should also reject the promise
	- 'resolveWithFullResponse = false' which is a boolean to set whether the promise should be resolved with the full response or
just the response body
	- 'transform' which takes a function to transform the response into a custom value with which the promise is resolved
...
```

#### <a name="apidoc.element.request-promise.delete"></a>[function <span class="apidocSignatureSpan">request-promise.</span>delete (uri, options, callback)](#apidoc.element.request-promise.delete)
- description and source-code
```javascript
delete = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.forever"></a>[function <span class="apidocSignatureSpan">request-promise.</span>forever (agentOptions, optionsArg)](#apidoc.element.request-promise.forever)
- description and source-code
```javascript
forever = function (agentOptions, optionsArg) {
  var options = {}
  if (optionsArg) {
    extend(options, optionsArg)
  }
  if (agentOptions) {
    options.agentOptions = agentOptions
  }

  options.forever = true
  return request.defaults(options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.get"></a>[function <span class="apidocSignatureSpan">request-promise.</span>get (uri, options, callback)](#apidoc.element.request-promise.get)
- description and source-code
```javascript
get = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...
- A Request object
	- With an [identical API](https://github.com/request/request): 'require('request-promise') == require('request')' so to say
	- However, **STREAMING THE RESPONSE** (e.g. '.pipe(...)') is **DISCOURAGED** because Request-Promise would grow the memory footprint
 for large requests unnecessarily high. Use the original Request library for that. You can use both libraries in the same project
.
- Plus some methods on a request call object:
	- 'rp(...).then(...)' or e.g. 'rp.post(...).then(...)' which turn 'rp(...)' and 'rp.post(...)' into promises
	- 'rp(...).catch(...)' or e.g. 'rp.del(...).catch(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).finally(...)' or e.g. 'rp.put(...).finally(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).cancel()' or e.g. 'rp.get(...).cancel()' which cancels the request
	- 'rp(...).promise()' or e.g. 'rp.head(...).promise()' which returns the underlying promise so you can access the full [Bluebird
 API](https://github.com/petkaantonov/bluebird/blob/master/API.md)
- Plus some additional options:
	- 'simple = true' which is a boolean to set whether status codes other than 2xx should also reject the promise
	- 'resolveWithFullResponse = false' which is a boolean to set whether the promise should be resolved with the full response or
just the response body
	- 'transform' which takes a function to transform the response into a custom value with which the promise is resolved
	- 'transform2xxOnly = false' which is a boolean to set whether the transform function is applied to all responses or only to those
 with a 2xx status code
...
```

#### <a name="apidoc.element.request-promise.head"></a>[function <span class="apidocSignatureSpan">request-promise.</span>head (uri, options, callback)](#apidoc.element.request-promise.head)
- description and source-code
```javascript
head = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...
	- With an [identical API](https://github.com/request/request): 'require('request-promise') == require('request')' so to say
	- However, **STREAMING THE RESPONSE** (e.g. '.pipe(...)') is **DISCOURAGED** because Request-Promise would grow the memory footprint
 for large requests unnecessarily high. Use the original Request library for that. You can use both libraries in the same project
.
- Plus some methods on a request call object:
	- 'rp(...).then(...)' or e.g. 'rp.post(...).then(...)' which turn 'rp(...)' and 'rp.post(...)' into promises
	- 'rp(...).catch(...)' or e.g. 'rp.del(...).catch(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).finally(...)' or e.g. 'rp.put(...).finally(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).cancel()' or e.g. 'rp.get(...).cancel()' which cancels the request
	- 'rp(...).promise()' or e.g. 'rp.head(...).promise()' which returns the underlying promise so you can access the full [Bluebird
 API](https://github.com/petkaantonov/bluebird/blob/master/API.md)
- Plus some additional options:
	- 'simple = true' which is a boolean to set whether status codes other than 2xx should also reject the promise
	- 'resolveWithFullResponse = false' which is a boolean to set whether the promise should be resolved with the full response or
just the response body
	- 'transform' which takes a function to transform the response into a custom value with which the promise is resolved
	- 'transform2xxOnly = false' which is a boolean to set whether the transform function is applied to all responses or only to those
 with a 2xx status code

The objects returned by request calls like 'rp(...)' or e.g. 'rp.post(...)' are regular Promises/A+ compliant promises and can be
 assimilated by any compatible promise library.
...
```

#### <a name="apidoc.element.request-promise.initParams"></a>[function <span class="apidocSignatureSpan">request-promise.</span>initParams (uri, options, callback)](#apidoc.element.request-promise.initParams)
- description and source-code
```javascript
function initParams(uri, options, callback) {
  if (typeof options === 'function') {
    callback = options
  }

  var params = {}
  if (typeof options === 'object') {
    extend(params, options, {uri: uri})
  } else if (typeof uri === 'string') {
    extend(params, {uri: uri})
  } else {
    extend(params, uri)
  }

  params.callback = callback || params.callback
  return params
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.jar"></a>[function <span class="apidocSignatureSpan">request-promise.</span>jar (store)](#apidoc.element.request-promise.jar)
- description and source-code
```javascript
jar = function (store) {
  return cookies.jar(store)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.patch"></a>[function <span class="apidocSignatureSpan">request-promise.</span>patch (uri, options, callback)](#apidoc.element.request-promise.patch)
- description and source-code
```javascript
patch = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.post"></a>[function <span class="apidocSignatureSpan">request-promise.</span>post (uri, options, callback)](#apidoc.element.request-promise.post)
- description and source-code
```javascript
post = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...

Consider Request-Promise being:

- A Request object
	- With an [identical API](https://github.com/request/request): 'require('request-promise') == require('request')' so to say
	- However, **STREAMING THE RESPONSE** (e.g. '.pipe(...)') is **DISCOURAGED** because Request-Promise would grow the memory footprint
 for large requests unnecessarily high. Use the original Request library for that. You can use both libraries in the same project
.
- Plus some methods on a request call object:
	- 'rp(...).then(...)' or e.g. 'rp.post(...).then(...)' which turn 'rp(...)' and 'rp.post(...)' into promises
	- 'rp(...).catch(...)' or e.g. 'rp.del(...).catch(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).finally(...)' or e.g. 'rp.put(...).finally(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).cancel()' or e.g. 'rp.get(...).cancel()' which cancels the request
	- 'rp(...).promise()' or e.g. 'rp.head(...).promise()' which returns the underlying promise so you can access the full [Bluebird
 API](https://github.com/petkaantonov/bluebird/blob/master/API.md)
- Plus some additional options:
	- 'simple = true' which is a boolean to set whether status codes other than 2xx should also reject the promise
	- 'resolveWithFullResponse = false' which is a boolean to set whether the promise should be resolved with the full response or
just the response body
...
```

#### <a name="apidoc.element.request-promise.put"></a>[function <span class="apidocSignatureSpan">request-promise.</span>put (uri, options, callback)](#apidoc.element.request-promise.put)
- description and source-code
```javascript
put = function (uri, options, callback) {
  var params = initParams(uri, options, callback)
  params.method = method
  return request(params, params.callback)
}
```
- example usage
```shell
...

- A Request object
	- With an [identical API](https://github.com/request/request): 'require('request-promise') == require('request')' so to say
	- However, **STREAMING THE RESPONSE** (e.g. '.pipe(...)') is **DISCOURAGED** because Request-Promise would grow the memory footprint
 for large requests unnecessarily high. Use the original Request library for that. You can use both libraries in the same project
.
- Plus some methods on a request call object:
	- 'rp(...).then(...)' or e.g. 'rp.post(...).then(...)' which turn 'rp(...)' and 'rp.post(...)' into promises
	- 'rp(...).catch(...)' or e.g. 'rp.del(...).catch(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).finally(...)' or e.g. 'rp.put(...).finally(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).cancel()' or e.g. 'rp.get(...).cancel()' which cancels the request
	- 'rp(...).promise()' or e.g. 'rp.head(...).promise()' which returns the underlying promise so you can access the full [Bluebird
 API](https://github.com/petkaantonov/bluebird/blob/master/API.md)
- Plus some additional options:
	- 'simple = true' which is a boolean to set whether status codes other than 2xx should also reject the promise
	- 'resolveWithFullResponse = false' which is a boolean to set whether the promise should be resolved with the full response or
just the response body
	- 'transform' which takes a function to transform the response into a custom value with which the promise is resolved
	- 'transform2xxOnly = false' which is a boolean to set whether the transform function is applied to all responses or only to those
 with a 2xx status code
...
```



# <a name="apidoc.module.request-promise.Request"></a>[module request-promise.Request](#apidoc.module.request-promise.Request)

#### <a name="apidoc.element.request-promise.Request.Request"></a>[function <span class="apidocSignatureSpan">request-promise.</span>Request (options)](#apidoc.element.request-promise.Request.Request)
- description and source-code
```javascript
function Request(options) {
  // if given the method property in options, set property explicitMethod to true

  // extend the Request instance with any non-reserved properties
  // remove any reserved functions from the options object
  // set Request instance to be readable and writable
  // call init

  var self = this

  // start with HAR, then override with additional options
  if (options.har) {
    self._har = new Har(self)
    options = self._har.options(options)
  }

  stream.Stream.call(self)
  var reserved = Object.keys(Request.prototype)
  var nonReserved = filterForNonReserved(reserved, options)

  extend(self, nonReserved)
  options = filterOutReservedFunctions(reserved, options)

  self.readable = true
  self.writable = true
  if (options.method) {
    self.explicitMethod = true
  }
  self._qs = new Querystring(self)
  self._auth = new Auth(self)
  self._oauth = new OAuth(self)
  self._multipart = new Multipart(self)
  self._redirect = new Redirect(self)
  self._tunnel = new Tunnel(self)
  self.init(options)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.super_"></a>[function <span class="apidocSignatureSpan">request-promise.Request.</span>super_ ()](#apidoc.element.request-promise.Request.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.request-promise.Request.prototype"></a>[module request-promise.Request.prototype](#apidoc.module.request-promise.Request.prototype)

#### <a name="apidoc.element.request-promise.Request.prototype.abort"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>abort ()](#apidoc.element.request-promise.Request.prototype.abort)
- description and source-code
```javascript
abort = function () {
  var self = this
  self._aborted = true

  if (self.req) {
    self.req.abort()
  }
  else if (self.response) {
    self.response.destroy()
  }

  self.emit('abort')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.auth"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>auth (user, pass, sendImmediately, bearer)](#apidoc.element.request-promise.Request.prototype.auth)
- description and source-code
```javascript
auth = function (user, pass, sendImmediately, bearer) {
  var self = this

  self._auth.onRequest(user, pass, sendImmediately, bearer)

  return self
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.aws"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>aws (opts, now)](#apidoc.element.request-promise.Request.prototype.aws)
- description and source-code
```javascript
aws = function (opts, now) {
  var self = this

  if (!now) {
    self._aws = opts
    return self
  }

  if (opts.sign_version == 4 || opts.sign_version == '4') {
    // use aws4
    var options = {
      host: self.uri.host,
      path: self.uri.path,
      method: self.method,
      headers: {
        'content-type': self.getHeader('content-type') || ''
      },
      body: self.body
    }
    var signRes = aws4.sign(options, {
      accessKeyId: opts.key,
      secretAccessKey: opts.secret,
      sessionToken: opts.session
    })
    self.setHeader('authorization', signRes.headers.Authorization)
    self.setHeader('x-amz-date', signRes.headers['X-Amz-Date'])
    if (signRes.headers['X-Amz-Security-Token']) {
      self.setHeader('x-amz-security-token', signRes.headers['X-Amz-Security-Token'])
    }
  }
  else {
    // default: use aws-sign2
    var date = new Date()
    self.setHeader('date', date.toUTCString())
    var auth =
      { key: opts.key
      , secret: opts.secret
      , verb: self.method.toUpperCase()
      , date: date
      , contentType: self.getHeader('content-type') || ''
      , md5: self.getHeader('content-md5') || ''
      , amazonHeaders: aws2.canonicalizeHeaders(self.headers)
      }
    var path = self.uri.path
    if (opts.bucket && path) {
      auth.resource = '/' + opts.bucket + path
    } else if (opts.bucket && !path) {
      auth.resource = '/' + opts.bucket
    } else if (!opts.bucket && path) {
      auth.resource = path
    } else if (!opts.bucket && !path) {
      auth.resource = '/'
    }
    auth.resource = aws2.canonicalizeResource(auth.resource)
    self.setHeader('authorization', aws2.authorization(auth))
  }

  return self
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.cancel"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>cancel ()](#apidoc.element.request-promise.Request.prototype.cancel)
- description and source-code
```javascript
function RP$exposed() {
    var self = bindTo || this;
    return self[promisePropertyKey][methodToExpose].apply(self[promisePropertyKey], arguments);
}
```
- example usage
```shell
...
- A Request object
	- With an [identical API](https://github.com/request/request): 'require('request-promise') == require('request')' so to say
	- However, **STREAMING THE RESPONSE** (e.g. '.pipe(...)') is **DISCOURAGED** because Request-Promise would grow the memory footprint
 for large requests unnecessarily high. Use the original Request library for that. You can use both libraries in the same project
.
- Plus some methods on a request call object:
	- 'rp(...).then(...)' or e.g. 'rp.post(...).then(...)' which turn 'rp(...)' and 'rp.post(...)' into promises
	- 'rp(...).catch(...)' or e.g. 'rp.del(...).catch(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).finally(...)' or e.g. 'rp.put(...).finally(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).cancel()' or e.g. 'rp.get(...).cancel()' which cancels the request
	- 'rp(...).promise()' or e.g. 'rp.head(...).promise()' which returns the underlying promise so you can access the full [Bluebird
 API](https://github.com/petkaantonov/bluebird/blob/master/API.md)
- Plus some additional options:
	- 'simple = true' which is a boolean to set whether status codes other than 2xx should also reject the promise
	- 'resolveWithFullResponse = false' which is a boolean to set whether the promise should be resolved with the full response or
just the response body
	- 'transform' which takes a function to transform the response into a custom value with which the promise is resolved
	- 'transform2xxOnly = false' which is a boolean to set whether the transform function is applied to all responses or only to those
 with a 2xx status code
...
```

#### <a name="apidoc.element.request-promise.Request.prototype.catch"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>catch ()](#apidoc.element.request-promise.Request.prototype.catch)
- description and source-code
```javascript
function RP$exposed() {
    var self = bindTo || this;
    return self[promisePropertyKey][methodToExpose].apply(self[promisePropertyKey], arguments);
}
```
- example usage
```shell
...
### Crawl a webpage

''' js
rp('http://www.google.com')
    .then(function (htmlString) {
        // Process html...
    })
    .catch(function (err) {
        // Crawling failed...
    });
'''

### Crawl a webpage better

''' js
...
```

#### <a name="apidoc.element.request-promise.Request.prototype.debug"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>debug ()](#apidoc.element.request-promise.Request.prototype.debug)
- description and source-code
```javascript
function debug() {
  if (Request.debug) {
    console.error('REQUEST %s', util.format.apply(util, arguments))
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.destroy"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>destroy ()](#apidoc.element.request-promise.Request.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  var self = this
  if (!self._ended) {
    self.end()
  } else if (self.response) {
    self.response.destroy()
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.enableUnixSocket"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>enableUnixSocket ()](#apidoc.element.request-promise.Request.prototype.enableUnixSocket)
- description and source-code
```javascript
enableUnixSocket = function () {
  // Get the socket & request paths from the URL
  var unixParts = this.uri.path.split(':')
    , host = unixParts[0]
    , path = unixParts[1]
  // Apply unix properties to request
  this.socketPath = host
  this.uri.pathname = path
  this.uri.path = path
  this.uri.host = host
  this.uri.hostname = host
  this.uri.isUnix = true
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.end"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>end (chunk)](#apidoc.element.request-promise.Request.prototype.end)
- description and source-code
```javascript
end = function (chunk) {
  var self = this
  if (self._aborted) {return}

  if (chunk) {
    self.write(chunk)
  }
  if (!self._started) {
    self.start()
  }
  if (self.req) {
    self.req.end()
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.finally"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>finally ()](#apidoc.element.request-promise.Request.prototype.finally)
- description and source-code
```javascript
function RP$exposed() {
    var self = bindTo || this;
    return self[promisePropertyKey][methodToExpose].apply(self[promisePropertyKey], arguments);
}
```
- example usage
```shell
...

- A Request object
	- With an [identical API](https://github.com/request/request): 'require('request-promise') == require('request')' so to say
	- However, **STREAMING THE RESPONSE** (e.g. '.pipe(...)') is **DISCOURAGED** because Request-Promise would grow the memory footprint
 for large requests unnecessarily high. Use the original Request library for that. You can use both libraries in the same project
.
- Plus some methods on a request call object:
	- 'rp(...).then(...)' or e.g. 'rp.post(...).then(...)' which turn 'rp(...)' and 'rp.post(...)' into promises
	- 'rp(...).catch(...)' or e.g. 'rp.del(...).catch(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).finally(...)' or e.g. 'rp.put(...).finally(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).cancel()' or e.g. 'rp.get(...).cancel()' which cancels the request
	- 'rp(...).promise()' or e.g. 'rp.head(...).promise()' which returns the underlying promise so you can access the full [Bluebird
 API](https://github.com/petkaantonov/bluebird/blob/master/API.md)
- Plus some additional options:
	- 'simple = true' which is a boolean to set whether status codes other than 2xx should also reject the promise
	- 'resolveWithFullResponse = false' which is a boolean to set whether the promise should be resolved with the full response or
just the response body
	- 'transform' which takes a function to transform the response into a custom value with which the promise is resolved
	- 'transform2xxOnly = false' which is a boolean to set whether the transform function is applied to all responses or only to those
 with a 2xx status code
...
```

#### <a name="apidoc.element.request-promise.Request.prototype.form"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>form (form)](#apidoc.element.request-promise.Request.prototype.form)
- description and source-code
```javascript
form = function (form) {
  var self = this
  if (form) {
    if (!/^application\/x-www-form-urlencoded\b/.test(self.getHeader('content-type'))) {
      self.setHeader('content-type', 'application/x-www-form-urlencoded')
    }
    self.body = (typeof form === 'string')
      ? self._qs.rfc3986(form.toString('utf8'))
      : self._qs.stringify(form).toString('utf8')
    return self
  }
  // create form-data object
  self._form = new FormData()
  self._form.on('error', function(err) {
    err.message = 'form-data: ' + err.message
    self.emit('error', err)
    self.abort()
  })
  return self._form
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.getHeader"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>getHeader (name, headers)](#apidoc.element.request-promise.Request.prototype.getHeader)
- description and source-code
```javascript
getHeader = function (name, headers) {
  var self = this
  var result, re, match
  if (!headers) {
    headers = self.headers
  }
  Object.keys(headers).forEach(function (key) {
    if (key.length !== name.length) {
      return
    }
    re = new RegExp(name, 'i')
    match = key.match(re)
    if (match) {
      result = headers[key]
    }
  })
  return result
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.getNewAgent"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>getNewAgent ()](#apidoc.element.request-promise.Request.prototype.getNewAgent)
- description and source-code
```javascript
getNewAgent = function () {
  var self = this
  var Agent = self.agentClass
  var options = {}
  if (self.agentOptions) {
    for (var i in self.agentOptions) {
      options[i] = self.agentOptions[i]
    }
  }
  if (self.ca) {
    options.ca = self.ca
  }
  if (self.ciphers) {
    options.ciphers = self.ciphers
  }
  if (self.secureProtocol) {
    options.secureProtocol = self.secureProtocol
  }
  if (self.secureOptions) {
    options.secureOptions = self.secureOptions
  }
  if (typeof self.rejectUnauthorized !== 'undefined') {
    options.rejectUnauthorized = self.rejectUnauthorized
  }

  if (self.cert && self.key) {
    options.key = self.key
    options.cert = self.cert
  }

  if (self.pfx) {
    options.pfx = self.pfx
  }

  if (self.passphrase) {
    options.passphrase = self.passphrase
  }

  var poolKey = ''

  // different types of agents are in different pools
  if (Agent !== self.httpModule.Agent) {
    poolKey += Agent.name
  }

  // ca option is only relevant if proxy or destination are https
  var proxy = self.proxy
  if (typeof proxy === 'string') {
    proxy = url.parse(proxy)
  }
  var isHttps = (proxy && proxy.protocol === 'https:') || this.uri.protocol === 'https:'

  if (isHttps) {
    if (options.ca) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.ca
    }

    if (typeof options.rejectUnauthorized !== 'undefined') {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.rejectUnauthorized
    }

    if (options.cert) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.cert.toString('ascii') + options.key.toString('ascii')
    }

    if (options.pfx) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.pfx.toString('ascii')
    }

    if (options.ciphers) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.ciphers
    }

    if (options.secureProtocol) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.secureProtocol
    }

    if (options.secureOptions) {
      if (poolKey) {
        poolKey += ':'
      }
      poolKey += options.secureOptions
    }
  }

  if (self.pool === globalPool && !poolKey && Object.keys(options).length === 0 && self.httpModule.globalAgent) {
    // not doing anything special.  Use the globalAgent
    return self.httpModule.globalAgent
  }

  // we're using a stored agent.  Make sure it's protocol-specific
  poolKey = self.uri.protocol + poolKey

  // generate a new agent for this setting if none yet exists
  if (!self.pool[poolKey]) {
    self.pool[poolKey] = new Agent(options)
    // properly set maxSockets on new agents
    if (self.pool.maxSockets) {
      self.pool[poolKey].maxSockets = self.pool.maxSockets
    }
  }

  return self.pool[poolKey]
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.hawk"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>hawk (opts)](#apidoc.element.request-promise.Request.prototype.hawk)
- description and source-code
```javascript
hawk = function (opts) {
  var self = this
  self.setHeader('Authorization', hawk.client.header(self.uri, self.method, opts).field)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.httpSignature"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>httpSignature (opts)](#apidoc.element.request-promise.Request.prototype.httpSignature)
- description and source-code
```javascript
httpSignature = function (opts) {
  var self = this
  httpSignature.signRequest({
    getHeader: function(header) {
      return self.getHeader(header, self.headers)
    },
    setHeader: function(header, value) {
      self.setHeader(header, value)
    },
    method: self.method,
    path: self.path
  }, opts)
  debug('httpSignature authorization', self.getHeader('authorization'))

  return self
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.init"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>init (requestOptions)](#apidoc.element.request-promise.Request.prototype.init)
- description and source-code
```javascript
function RP$initInterceptor(requestOptions) {

    // Init may be called again - currently in case of redirects
    if (isObjectLike(requestOptions) && !this._callback && !this._rp_promise) {

        plumbing.init.call(this, requestOptions);

    }

    return originalInit.apply(this, arguments);

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.jar"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>jar (jar)](#apidoc.element.request-promise.Request.prototype.jar)
- description and source-code
```javascript
jar = function (jar) {
  var self = this
  var cookies

  if (self._redirect.redirectsFollowed === 0) {
    self.originalCookieHeader = self.getHeader('cookie')
  }

  if (!jar) {
    // disable cookies
    cookies = false
    self._disableCookies = true
  } else {
    var targetCookieJar = (jar && jar.getCookieString) ? jar : globalCookieJar
    var urihref = self.uri.href
    //fetch cookie in the Specified host
    if (targetCookieJar) {
      cookies = targetCookieJar.getCookieString(urihref)
    }
  }

  //if need cookie and cookie is not empty
  if (cookies && cookies.length) {
    if (self.originalCookieHeader) {
      // Don't overwrite existing Cookie header
      self.setHeader('cookie', self.originalCookieHeader + '; ' + cookies)
    } else {
      self.setHeader('cookie', cookies)
    }
  }
  self._jar = jar
  return self
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.json"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>json (val)](#apidoc.element.request-promise.Request.prototype.json)
- description and source-code
```javascript
json = function (val) {
  var self = this

  if (!self.hasHeader('accept')) {
    self.setHeader('accept', 'application/json')
  }

  if (typeof self.jsonReplacer === 'function') {
    self._jsonReplacer = self.jsonReplacer
  }

  self._json = true
  if (typeof val === 'boolean') {
    if (self.body !== undefined) {
      if (!/^application\/x-www-form-urlencoded\b/.test(self.getHeader('content-type'))) {
        self.body = safeStringify(self.body, self._jsonReplacer)
      } else {
        self.body = self._qs.rfc3986(self.body)
      }
      if (!self.hasHeader('content-type')) {
        self.setHeader('content-type', 'application/json')
      }
    }
  } else {
    self.body = safeStringify(val, self._jsonReplacer)
    if (!self.hasHeader('content-type')) {
      self.setHeader('content-type', 'application/json')
    }
  }

  if (typeof self.jsonReviver === 'function') {
    self._jsonReviver = self.jsonReviver
  }

  return self
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.multipart"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>multipart (multipart)](#apidoc.element.request-promise.Request.prototype.multipart)
- description and source-code
```javascript
multipart = function (multipart) {
  var self = this

  self._multipart.onRequest(multipart)

  if (!self._multipart.chunked) {
    self.body = self._multipart.body
  }

  return self
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.oauth"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>oauth (_oauth)](#apidoc.element.request-promise.Request.prototype.oauth)
- description and source-code
```javascript
oauth = function (_oauth) {
  var self = this

  self._oauth.onRequest(_oauth)

  return self
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.onRequestError"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>onRequestError (error)](#apidoc.element.request-promise.Request.prototype.onRequestError)
- description and source-code
```javascript
onRequestError = function (error) {
  var self = this
  if (self._aborted) {
    return
  }
  if (self.req && self.req._reusedSocket && error.code === 'ECONNRESET'
      && self.agent.addRequestNoreuse) {
    self.agent = { addRequest: self.agent.addRequestNoreuse.bind(self.agent) }
    self.start()
    self.req.end()
    return
  }
  if (self.timeout && self.timeoutTimer) {
    clearTimeout(self.timeoutTimer)
    self.timeoutTimer = null
  }
  self.emit('error', error)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.onRequestResponse"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>onRequestResponse (response)](#apidoc.element.request-promise.Request.prototype.onRequestResponse)
- description and source-code
```javascript
onRequestResponse = function (response) {
  var self = this

  if (self.timing) {
    self.timings.response = now() - self.startTimeNow
  }

  debug('onRequestResponse', self.uri.href, response.statusCode, response.headers)
  response.on('end', function() {
    if (self.timing) {
      self.timings.end = now() - self.startTimeNow
      response.timingStart = self.startTime

      // fill in the blanks for any periods that didn't trigger, such as
      // no lookup or connect due to keep alive
      if (!self.timings.socket) {
        self.timings.socket = 0
      }
      if (!self.timings.lookup) {
        self.timings.lookup = self.timings.socket
      }
      if (!self.timings.connect) {
        self.timings.connect = self.timings.lookup
      }
      if (!self.timings.response) {
        self.timings.response = self.timings.connect
      }

      debug('elapsed time', self.timings.end)

      // elapsedTime includes all redirects
      self.elapsedTime += Math.round(self.timings.end)

      // NOTE: elapsedTime is deprecated in favor of .timings
      response.elapsedTime = self.elapsedTime

      // timings is just for the final fetch
      response.timings = self.timings

      // pre-calculate phase timings as well
      response.timingPhases = {
        wait: self.timings.socket,
        dns: self.timings.lookup - self.timings.socket,
        tcp: self.timings.connect - self.timings.lookup,
        firstByte: self.timings.response - self.timings.connect,
        download: self.timings.end - self.timings.response,
        total: self.timings.end
      }
    }
    debug('response end', self.uri.href, response.statusCode, response.headers)
  })

  if (self._aborted) {
    debug('aborted', self.uri.href)
    response.resume()
    return
  }

  self.response = response
  response.request = self
  response.toJSON = responseToJSON

  // XXX This is different on 0.10, because SSL is strict by default
  if (self.httpModule === https &&
      self.strictSSL && (!response.hasOwnProperty('socket') ||
      !response.socket.authorized)) {
    debug('strict ssl error', self.uri.href)
    var sslErr = response.hasOwnProperty('socket') ? response.socket.authorizationError : self.uri.href + ' does not support SSL
'
    self.emit('error', new Error('SSL Error: ' + sslErr))
    return
  }

  // Save the original host before any redirect (if it changes, we need to
  // remove any authorization headers).  Also remember the case of the header
  // name because lots of broken servers expect Host instead of host and we
  // want the caller to be able to specify this.
  self.originalHost = self.getHeader('host')
  if (!self.originalHostHeaderName) {
    self.originalHostHeaderName = self.hasHeader('host')
  }
  if (self.setHost) {
    self.removeHeader('host')
  }
  if (self.timeout && self.timeoutTimer) {
    clearTimeout(self.timeoutTimer)
    self.timeoutTimer = null
  }

  var targetCookieJar = (self._jar && self._jar.setCookie) ? self._jar : globalCookieJar
  var addCookie = function (cookie) {
    //set the cookie if it's domain in the href's domain.
    try {
      targetCookieJar.setCookie(cookie, self.uri.href, {ignoreError: true})
    } catch (e) {
      self.emit('error', e)
    }
  }

  response.caseless = caseless(response.headers)

  if (response.caseless.has('set-cookie') && (!self._disableCookies)) {
    var headerName = response.caseless.has('set-cookie')
    if (Array.isArray(response.headers[headerName])) {
      response.headers[headerName].forEach(addCookie)
    } else {
      addCookie(response.headers[headerName])
    }
  }

  if (self._redirect.onResponse(response)) {
    return // Ignore the rest of the response
  } else {
    // Be a good stream and emit end when the response is finished.
    // Hack to emit end on close because of a core bug that never fires end
    response.on('close', function () {
      if (!self._ended) {
        self.response.emit('end')
      }
    })

    response.once('end', function () {
      self._ended = true
    })

    var noBody = function (code) {
      return (
        self.method === 'HEAD' ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.pause"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>pause ()](#apidoc.element.request-promise.Request.prototype.pause)
- description and source-code
```javascript
pause = function () {
  var self = this
  if (!self.responseContent) {
    self._paused = true
  } else {
    self.responseContent.pause.apply(self.responseContent, arguments)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.pipe"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>pipe (dest, opts)](#apidoc.element.request-promise.Request.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest, opts) {
  var self = this

  if (self.response) {
    if (self._destdata) {
      self.emit('error', new Error('You cannot pipe after data has been emitted from the response.'))
    } else if (self._ended) {
      self.emit('error', new Error('You cannot pipe after the response has been ended.'))
    } else {
      stream.Stream.prototype.pipe.call(self, dest, opts)
      self.pipeDest(dest)
      return dest
    }
  } else {
    self.dests.push(dest)
    stream.Stream.prototype.pipe.call(self, dest, opts)
    return dest
  }
}
```
- example usage
```shell
...

## API in Detail

Consider Request-Promise being:

- A Request object
	- With an [identical API](https://github.com/request/request): 'require('request-promise') == require('request')' so to say
	- However, **STREAMING THE RESPONSE** (e.g. '.pipe(...)') is **DISCOURAGED** because Request-Promise would grow the memory footprint
 for large requests unnecessarily high. Use the original Request library for that. You can use both libraries in the same project
.
- Plus some methods on a request call object:
	- 'rp(...).then(...)' or e.g. 'rp.post(...).then(...)' which turn 'rp(...)' and 'rp.post(...)' into promises
	- 'rp(...).catch(...)' or e.g. 'rp.del(...).catch(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).finally(...)' or e.g. 'rp.put(...).finally(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).cancel()' or e.g. 'rp.get(...).cancel()' which cancels the request
	- 'rp(...).promise()' or e.g. 'rp.head(...).promise()' which returns the underlying promise so you can access the full [Bluebird
 API](https://github.com/petkaantonov/bluebird/blob/master/API.md)
- Plus some additional options:
...
```

#### <a name="apidoc.element.request-promise.Request.prototype.pipeDest"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>pipeDest (dest)](#apidoc.element.request-promise.Request.prototype.pipeDest)
- description and source-code
```javascript
pipeDest = function (dest) {
  var self = this
  var response = self.response
  // Called after the response is received
  if (dest.headers && !dest.headersSent) {
    if (response.caseless.has('content-type')) {
      var ctname = response.caseless.has('content-type')
      if (dest.setHeader) {
        dest.setHeader(ctname, response.headers[ctname])
      }
      else {
        dest.headers[ctname] = response.headers[ctname]
      }
    }

    if (response.caseless.has('content-length')) {
      var clname = response.caseless.has('content-length')
      if (dest.setHeader) {
        dest.setHeader(clname, response.headers[clname])
      } else {
        dest.headers[clname] = response.headers[clname]
      }
    }
  }
  if (dest.setHeader && !dest.headersSent) {
    for (var i in response.headers) {
      // If the response content is being decoded, the Content-Encoding header
      // of the response doesn't represent the piped content, so don't pass it.
      if (!self.gzip || i !== 'content-encoding') {
        dest.setHeader(i, response.headers[i])
      }
    }
    dest.statusCode = response.statusCode
  }
  if (self.pipefilter) {
    self.pipefilter(response, dest)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.promise"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>promise ()](#apidoc.element.request-promise.Request.prototype.promise)
- description and source-code
```javascript
function RP$promise() {
    var self = bindTo || this;
    return self[promisePropertyKey];
}
```
- example usage
```shell
...
	- With an [identical API](https://github.com/request/request): 'require('request-promise') == require('request')' so to say
	- However, **STREAMING THE RESPONSE** (e.g. '.pipe(...)') is **DISCOURAGED** because Request-Promise would grow the memory footprint
 for large requests unnecessarily high. Use the original Request library for that. You can use both libraries in the same project
.
- Plus some methods on a request call object:
	- 'rp(...).then(...)' or e.g. 'rp.post(...).then(...)' which turn 'rp(...)' and 'rp.post(...)' into promises
	- 'rp(...).catch(...)' or e.g. 'rp.del(...).catch(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).finally(...)' or e.g. 'rp.put(...).finally(...)' which is the same method as provided by Bluebird promises
	- 'rp(...).cancel()' or e.g. 'rp.get(...).cancel()' which cancels the request
	- 'rp(...).promise()' or e.g. 'rp.head(...).promise()' which returns the underlying promise so you can access the full [Bluebird
 API](https://github.com/petkaantonov/bluebird/blob/master/API.md)
- Plus some additional options:
	- 'simple = true' which is a boolean to set whether status codes other than 2xx should also reject the promise
	- 'resolveWithFullResponse = false' which is a boolean to set whether the promise should be resolved with the full response or
just the response body
	- 'transform' which takes a function to transform the response into a custom value with which the promise is resolved
	- 'transform2xxOnly = false' which is a boolean to set whether the transform function is applied to all responses or only to those
 with a 2xx status code

The objects returned by request calls like 'rp(...)' or e.g. 'rp.post(...)' are regular Promises/A+ compliant promises and can be
 assimilated by any compatible promise library.
...
```

#### <a name="apidoc.element.request-promise.Request.prototype.qs"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>qs (q, clobber)](#apidoc.element.request-promise.Request.prototype.qs)
- description and source-code
```javascript
qs = function (q, clobber) {
  var self = this
  var base
  if (!clobber && self.uri.query) {
    base = self._qs.parse(self.uri.query)
  } else {
    base = {}
  }

  for (var i in q) {
    base[i] = q[i]
  }

  var qs = self._qs.stringify(base)

  if (qs === '') {
    return self
  }

  self.uri = url.parse(self.uri.href.split('?')[0] + '?' + qs)
  self.url = self.uri
  self.path = self.uri.path

  if (self.uri.host === 'unix') {
    self.enableUnixSocket()
  }

  return self
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.readResponseBody"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>readResponseBody (response)](#apidoc.element.request-promise.Request.prototype.readResponseBody)
- description and source-code
```javascript
readResponseBody = function (response) {
  var self = this
  debug('reading response\'s body')
  var buffers = []
    , bufferLength = 0
    , strings = []

  self.on('data', function (chunk) {
    if (!Buffer.isBuffer(chunk)) {
      strings.push(chunk)
    } else if (chunk.length) {
      bufferLength += chunk.length
      buffers.push(chunk)
    }
  })
  self.on('end', function () {
    debug('end event', self.uri.href)
    if (self._aborted) {
      debug('aborted', self.uri.href)
      // 'buffer' is defined in the parent scope and used in a closure it exists for the life of the request.
      // This can lead to leaky behavior if the user retains a reference to the request object.
      buffers = []
      bufferLength = 0
      return
    }

    if (bufferLength) {
      debug('has body', self.uri.href, bufferLength)
      response.body = Buffer.concat(buffers, bufferLength)
      if (self.encoding !== null) {
        response.body = response.body.toString(self.encoding)
      }
      // 'buffer' is defined in the parent scope and used in a closure it exists for the life of the Request.
      // This can lead to leaky behavior if the user retains a reference to the request object.
      buffers = []
      bufferLength = 0
    } else if (strings.length) {
      // The UTF8 BOM [0xEF,0xBB,0xBF] is converted to [0xFE,0xFF] in the JS UTC16/UCS2 representation.
      // Strip this value out when the encoding is set to 'utf8', as upstream consumers won't expect it and it breaks JSON.parse
().
      if (self.encoding === 'utf8' && strings[0].length > 0 && strings[0][0] === '\uFEFF') {
        strings[0] = strings[0].substring(1)
      }
      response.body = strings.join('')
    }

    if (self._json) {
      try {
        response.body = JSON.parse(response.body, self._jsonReviver)
      } catch (e) {
        debug('invalid JSON received', self.uri.href)
      }
    }
    debug('emitting complete', self.uri.href)
    if (typeof response.body === 'undefined' && !self._json) {
      response.body = self.encoding === null ? Buffer.alloc(0) : ''
    }
    self.emit('complete', response, response.body)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.resume"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>resume ()](#apidoc.element.request-promise.Request.prototype.resume)
- description and source-code
```javascript
resume = function () {
  var self = this
  if (!self.responseContent) {
    self._paused = false
  } else {
    self.responseContent.resume.apply(self.responseContent, arguments)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.start"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>start ()](#apidoc.element.request-promise.Request.prototype.start)
- description and source-code
```javascript
start = function () {
  // start() is called once we are ready to send the outgoing HTTP request.
  // this is usually called on the first write(), end() or on nextTick()
  var self = this

  if (self.timing) {
    // All timings will be relative to this request's startTime.  In order to do this,
    // we need to capture the wall-clock start time (via Date), immediately followed
    // by the high-resolution timer (via now()).  While these two won't be set
    // at the _exact_ same time, they should be close enough to be able to calculate
    // high-resolution, monotonically non-decreasing timestamps relative to startTime.
    var startTime = new Date().getTime()
    var startTimeNow = now()
  }

  if (self._aborted) {
    return
  }

  self._started = true
  self.method = self.method || 'GET'
  self.href = self.uri.href

  if (self.src && self.src.stat && self.src.stat.size && !self.hasHeader('content-length')) {
    self.setHeader('content-length', self.src.stat.size)
  }
  if (self._aws) {
    self.aws(self._aws, true)
  }

  // We have a method named auth, which is completely different from the http.request
  // auth option.  If we don't remove it, we're gonna have a bad time.
  var reqOptions = copy(self)
  delete reqOptions.auth

  debug('make request', self.uri.href)

  // node v6.8.0 now supports a 'timeout' value in 'http.request()', but we
  // should delete it for now since we handle timeouts manually for better
  // consistency with node versions before v6.8.0
  delete reqOptions.timeout

  try {
    self.req = self.httpModule.request(reqOptions)
  } catch (err) {
    self.emit('error', err)
    return
  }

  if (self.timing) {
    self.startTime = startTime
    self.startTimeNow = startTimeNow

    // Timing values will all be relative to startTime (by comparing to startTimeNow
    // so we have an accurate clock)
    self.timings = {}
  }

  var timeout
  if (self.timeout && !self.timeoutTimer) {
    if (self.timeout < 0) {
      timeout = 0
    } else if (typeof self.timeout === 'number' && isFinite(self.timeout)) {
      timeout = self.timeout
    }
  }

  self.req.on('response', self.onRequestResponse.bind(self))
  self.req.on('error', self.onRequestError.bind(self))
  self.req.on('drain', function() {
    self.emit('drain')
  })
  self.req.on('socket', function(socket) {
    // '._connecting' was the old property which was made public in node v6.1.0
    var isConnecting = socket._connecting || socket.connecting
    if (self.timing) {
      self.timings.socket = now() - self.startTimeNow

      if (isConnecting) {
        var onLookupTiming = function() {
          self.timings.lookup = now() - self.startTimeNow
        }

        var onConnectTiming = function() {
          self.timings.connect = now() - self.startTimeNow
        }

        socket.once('lookup', onLookupTiming)
        socket.once('connect', onConnectTiming)

        // clean up timing event listeners if needed on error
        self.req.once('error', function() {
          socket.removeListener('lookup', onLookupTiming)
          socket.removeListener('connect', onConnectTiming)
        })
      }
    }

    var setReqTimeout = function() {
      // This timeout sets the amount of time to wait *between* bytes sent
      // from the server once connected.
      //
      // In particular, it's useful for erroring if the server fails to send
      // data halfway through streaming a response.
      self.req.setTimeout(timeout, function () {
        if (self.req) {
          self.abort()
          var e = new Error('ESOCKETTIMEDOUT')
          e.code = 'ESOCKETTIMEDOUT'
          e.connect = false
          self.emit('error', e)
        }
      })
    }
    if (timeout !== undefined) {
      // Only start the connection timer if we're actually connecting a new
      // socket, otherwise if we're already connected (because this is a
      // keep-alive connection) do not bother. This is important since we won't
      // get a 'connect' event for an already connected socket.
      if (isConnecting) {
        var onReqSockConnect = function() { ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.then"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>then ()](#apidoc.element.request-promise.Request.prototype.then)
- description and source-code
```javascript
function RP$exposed() {
    var self = bindTo || this;
    return self[promisePropertyKey][methodToExpose].apply(self[promisePropertyKey], arguments);
}
```
- example usage
```shell
...
[![Build Status](https://img.shields.io/travis/request/request-promise/master.svg?style=flat-square&maxAge=2592000)](https://travis
-ci.org/request/request-promise)
[![Coverage Status](https://img.shields.io/coveralls/request/request-promise.svg?style=flat-square&maxAge=2592000)](https://coveralls
.io/r/request/request-promise)
[![Dependency Status](https://img.shields.io/david/request/request-promise.svg?style=flat-square&maxAge=2592000)](https://david-
dm.org/request/request-promise)
[![Known Vulnerabilities](https://snyk.io/test/npm/request-promise/badge.svg?style=flat-square&maxAge=2592000)](https://snyk.io/
test/npm/request-promise)

The simplified HTTP request client 'request' with Promise support. Powered by Bluebird.

[Request](https://github.com/request/request) and [Bluebird](https://github.com/petkaantonov/bluebird) are pretty awesome, but I
 found myself using the same design pattern. Request-Promise adds a Bluebird-powered '.then(...)' method to Request call objects
. By default, http response codes other than 2xx will cause the promise to be rejected. This can be overwritten by setting 'options
.simple = false'.

Also check out the new libraries that are **very similar to 'request-promise' v4**:
- ['request-promise-native'](https://github.com/request/request-promise-native) v1 &ndash; Does not depend on Bluebird and uses
native ES6 promises instead.
- ['request-promise-any'](https://github.com/request/request-promise-any) v1 &ndash; Allows you to register any Promise library
supported by ['any-promise'](https://www.npmjs.com/package/any-promise).

---
...
```

#### <a name="apidoc.element.request-promise.Request.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>toJSON ()](#apidoc.element.request-promise.Request.prototype.toJSON)
- description and source-code
```javascript
function requestToJSON() {
  var self = this
  return {
    uri: self.uri,
    method: self.method,
    headers: self.headers
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.request-promise.Request.prototype.write"></a>[function <span class="apidocSignatureSpan">request-promise.Request.prototype.</span>write ()](#apidoc.element.request-promise.Request.prototype.write)
- description and source-code
```javascript
write = function () {
  var self = this
  if (self._aborted) {return}

  if (!self._started) {
    self.start()
  }
  if (self.req) {
    return self.req.write.apply(self.req, arguments)
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
