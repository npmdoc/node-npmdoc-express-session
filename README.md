# api documentation for  [express-session (v1.15.1)](https://github.com/expressjs/session#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-express-session.svg)](https://travis-ci.org/npmdoc/node-npmdoc-express-session)
#### Simple session middleware for Express

[![NPM](https://nodei.co/npm/express-session.png?downloads=true)](https://www.npmjs.com/package/express-session)

[![apidoc](https://npmdoc.github.io/node-npmdoc-express-session/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-express-session_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-express-session/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-express-session/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "TJ Holowaychuk",
        "email": "tj@vision-media.ca",
        "url": "http://tjholowaychuk.com"
    },
    "bugs": {
        "url": "https://github.com/expressjs/session/issues"
    },
    "contributors": [
        {
            "name": "Douglas Christopher Wilson",
            "email": "doug@somethingdoug.com"
        },
        {
            "name": "Joe Wagner",
            "email": "njwjs722@gmail.com"
        }
    ],
    "dependencies": {
        "cookie": "0.3.1",
        "cookie-signature": "1.0.6",
        "crc": "3.4.4",
        "debug": "2.6.1",
        "depd": "~1.1.0",
        "on-headers": "~1.0.1",
        "parseurl": "~1.3.1",
        "uid-safe": "~2.1.3",
        "utils-merge": "1.0.0"
    },
    "description": "Simple session middleware for Express",
    "devDependencies": {
        "after": "0.8.2",
        "cookie-parser": "1.4.3",
        "express": "4.14.0",
        "istanbul": "0.4.5",
        "mocha": "2.5.3",
        "supertest": "1.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "9abba15971beea7ad98da5a4d25ed92ba4a2984e",
        "tarball": "https://registry.npmjs.org/express-session/-/express-session-1.15.1.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "files": [
        "session/",
        "HISTORY.md",
        "LICENSE",
        "index.js"
    ],
    "gitHead": "8e56128d8ba014ab586521247977b0d4e67340f9",
    "homepage": "https://github.com/expressjs/session#readme",
    "license": "MIT",
    "maintainers": [
        {
            "name": "defunctzombie",
            "email": "shtylman@gmail.com"
        },
        {
            "name": "dougwilson",
            "email": "doug@somethingdoug.com"
        },
        {
            "name": "mscdex",
            "email": "mscdex@mscdex.net"
        }
    ],
    "name": "express-session",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/expressjs/session.git"
    },
    "scripts": {
        "test": "mocha --bail --reporter spec test/",
        "test-cov": "istanbul cover node_modules/mocha/bin/_mocha -- --reporter dot test/",
        "test-travis": "istanbul cover node_modules/mocha/bin/_mocha --report lcovonly -- --reporter spec test/"
    },
    "version": "1.15.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module express-session](#apidoc.module.express-session)
1.  [function <span class="apidocSignatureSpan">express-session.</span>Cookie (options)](#apidoc.element.express-session.Cookie)
1.  [function <span class="apidocSignatureSpan">express-session.</span>MemoryStore ()](#apidoc.element.express-session.MemoryStore)
1.  [function <span class="apidocSignatureSpan">express-session.</span>Session (req, data)](#apidoc.element.express-session.Session)
1.  [function <span class="apidocSignatureSpan">express-session.</span>Store ()](#apidoc.element.express-session.Store)
1.  object <span class="apidocSignatureSpan">express-session.</span>Cookie.prototype
1.  object <span class="apidocSignatureSpan">express-session.</span>MemoryStore.prototype
1.  object <span class="apidocSignatureSpan">express-session.</span>Store.prototype

#### [module express-session.Cookie](#apidoc.module.express-session.Cookie)
1.  [function <span class="apidocSignatureSpan">express-session.</span>Cookie (options)](#apidoc.element.express-session.Cookie.Cookie)

#### [module express-session.Cookie.prototype](#apidoc.module.express-session.Cookie.prototype)
1.  [function <span class="apidocSignatureSpan">express-session.Cookie.prototype.</span>serialize (name, val)](#apidoc.element.express-session.Cookie.prototype.serialize)
1.  [function <span class="apidocSignatureSpan">express-session.Cookie.prototype.</span>toJSON ()](#apidoc.element.express-session.Cookie.prototype.toJSON)
1.  object <span class="apidocSignatureSpan">express-session.Cookie.prototype.</span>data

#### [module express-session.MemoryStore](#apidoc.module.express-session.MemoryStore)
1.  [function <span class="apidocSignatureSpan">express-session.</span>MemoryStore ()](#apidoc.element.express-session.MemoryStore.MemoryStore)
1.  [function <span class="apidocSignatureSpan">express-session.MemoryStore.</span>super_ ()](#apidoc.element.express-session.MemoryStore.super_)

#### [module express-session.MemoryStore.prototype](#apidoc.module.express-session.MemoryStore.prototype)
1.  [function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>all (callback)](#apidoc.element.express-session.MemoryStore.prototype.all)
1.  [function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>clear (callback)](#apidoc.element.express-session.MemoryStore.prototype.clear)
1.  [function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>destroy (sessionId, callback)](#apidoc.element.express-session.MemoryStore.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>get (sessionId, callback)](#apidoc.element.express-session.MemoryStore.prototype.get)
1.  [function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>length (callback)](#apidoc.element.express-session.MemoryStore.prototype.length)
1.  [function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>set (sessionId, session, callback)](#apidoc.element.express-session.MemoryStore.prototype.set)
1.  [function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>touch (sessionId, session, callback)](#apidoc.element.express-session.MemoryStore.prototype.touch)

#### [module express-session.Store](#apidoc.module.express-session.Store)
1.  [function <span class="apidocSignatureSpan">express-session.</span>Store ()](#apidoc.element.express-session.Store.Store)
1.  [function <span class="apidocSignatureSpan">express-session.Store.</span>super_ ()](#apidoc.element.express-session.Store.super_)

#### [module express-session.Store.prototype](#apidoc.module.express-session.Store.prototype)
1.  [function <span class="apidocSignatureSpan">express-session.Store.prototype.</span>createSession (req, sess)](#apidoc.element.express-session.Store.prototype.createSession)
1.  [function <span class="apidocSignatureSpan">express-session.Store.prototype.</span>load (sid, fn)](#apidoc.element.express-session.Store.prototype.load)
1.  [function <span class="apidocSignatureSpan">express-session.Store.prototype.</span>regenerate (req, fn)](#apidoc.element.express-session.Store.prototype.regenerate)



# <a name="apidoc.module.express-session"></a>[module express-session](#apidoc.module.express-session)

#### <a name="apidoc.element.express-session.Cookie"></a>[function <span class="apidocSignatureSpan">express-session.</span>Cookie (options)](#apidoc.element.express-session.Cookie)
- description and source-code
```javascript
function Cookie(options) {
  this.path = '/';
  this.maxAge = null;
  this.httpOnly = true;
  if (options) merge(this, options);
  this.originalMaxAge = undefined == this.originalMaxAge
    ? this.maxAge
    : this.originalMaxAge;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-session.MemoryStore"></a>[function <span class="apidocSignatureSpan">express-session.</span>MemoryStore ()](#apidoc.element.express-session.MemoryStore)
- description and source-code
```javascript
function MemoryStore() {
  Store.call(this)
  this.sessions = Object.create(null)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-session.Session"></a>[function <span class="apidocSignatureSpan">express-session.</span>Session (req, data)](#apidoc.element.express-session.Session)
- description and source-code
```javascript
function Session(req, data) {
  Object.defineProperty(this, 'req', { value: req });
  Object.defineProperty(this, 'id', { value: req.sessionID });

  if (typeof data === 'object' && data !== null) {
    // merge data into this, ignoring prototype properties
    for (var prop in data) {
      if (!(prop in this)) {
        this[prop] = data[prop]
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-session.Store"></a>[function <span class="apidocSignatureSpan">express-session.</span>Store ()](#apidoc.element.express-session.Store)
- description and source-code
```javascript
function Store() {
  EventEmitter.call(this)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.express-session.Cookie"></a>[module express-session.Cookie](#apidoc.module.express-session.Cookie)

#### <a name="apidoc.element.express-session.Cookie.Cookie"></a>[function <span class="apidocSignatureSpan">express-session.</span>Cookie (options)](#apidoc.element.express-session.Cookie.Cookie)
- description and source-code
```javascript
function Cookie(options) {
  this.path = '/';
  this.maxAge = null;
  this.httpOnly = true;
  if (options) merge(this, options);
  this.originalMaxAge = undefined == this.originalMaxAge
    ? this.maxAge
    : this.originalMaxAge;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.express-session.Cookie.prototype"></a>[module express-session.Cookie.prototype](#apidoc.module.express-session.Cookie.prototype)

#### <a name="apidoc.element.express-session.Cookie.prototype.serialize"></a>[function <span class="apidocSignatureSpan">express-session.Cookie.prototype.</span>serialize (name, val)](#apidoc.element.express-session.Cookie.prototype.serialize)
- description and source-code
```javascript
serialize = function (name, val){
  return cookie.serialize(name, val, this.data);
}
```
- example usage
```shell
...
 * Set cookie on response.
 *
 * @private
 */

function setcookie(res, name, val, secret, options) {
var signed = 's:' + signature.sign(val, secret);
var data = cookie.serialize(name, signed, options);

debug('set-cookie %s', data);

var prev = res.getHeader('set-cookie') || [];
var header = Array.isArray(prev) ? prev.concat(data) : [prev, data];

res.setHeader('set-cookie', header)
...
```

#### <a name="apidoc.element.express-session.Cookie.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">express-session.Cookie.prototype.</span>toJSON ()](#apidoc.element.express-session.Cookie.prototype.toJSON)
- description and source-code
```javascript
toJSON = function (){
  return this.data;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.express-session.MemoryStore"></a>[module express-session.MemoryStore](#apidoc.module.express-session.MemoryStore)

#### <a name="apidoc.element.express-session.MemoryStore.MemoryStore"></a>[function <span class="apidocSignatureSpan">express-session.</span>MemoryStore ()](#apidoc.element.express-session.MemoryStore.MemoryStore)
- description and source-code
```javascript
function MemoryStore() {
  Store.call(this)
  this.sessions = Object.create(null)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-session.MemoryStore.super_"></a>[function <span class="apidocSignatureSpan">express-session.MemoryStore.</span>super_ ()](#apidoc.element.express-session.MemoryStore.super_)
- description and source-code
```javascript
function Store() {
  EventEmitter.call(this)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.express-session.MemoryStore.prototype"></a>[module express-session.MemoryStore.prototype](#apidoc.module.express-session.MemoryStore.prototype)

#### <a name="apidoc.element.express-session.MemoryStore.prototype.all"></a>[function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>all (callback)](#apidoc.element.express-session.MemoryStore.prototype.all)
- description and source-code
```javascript
function all(callback) {
  var sessionIds = Object.keys(this.sessions)
  var sessions = Object.create(null)

  for (var i = 0; i < sessionIds.length; i++) {
    var sessionId = sessionIds[i]
    var session = getSession.call(this, sessionId)

    if (session) {
      sessions[sessionId] = session;
    }
  }

  callback && defer(callback, null, sessions)
}
```
- example usage
```shell
...
  * Recommended methods are ones that this module will call on the store if
    available.
  * Optional methods are ones this module does not call at all, but helps
    present uniform stores to users.

For an example implementation view the [connect-redis](http://github.com/visionmedia/connect-redis) repo.

### store.all(callback)

**Optional**

This optional method is used to get all sessions in the store as an array. The
'callback' should be called as 'callback(error, sessions)'.

### store.destroy(sid, callback)
...
```

#### <a name="apidoc.element.express-session.MemoryStore.prototype.clear"></a>[function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>clear (callback)](#apidoc.element.express-session.MemoryStore.prototype.clear)
- description and source-code
```javascript
function clear(callback) {
  this.sessions = Object.create(null)
  callback && defer(callback)
}
```
- example usage
```shell
...

**Required**

This required method is used to destroy/delete a session from the store given
a session ID ('sid'). The 'callback' should be called as 'callback(error)' once
the session is destroyed.

### store.clear(callback)

**Optional**

This optional method is used to delete all sessions from the store. The
'callback' should be called as 'callback(error)' once the store is cleared.

### store.length(callback)
...
```

#### <a name="apidoc.element.express-session.MemoryStore.prototype.destroy"></a>[function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>destroy (sessionId, callback)](#apidoc.element.express-session.MemoryStore.prototype.destroy)
- description and source-code
```javascript
function destroy(sessionId, callback) {
  delete this.sessions[sessionId]
  callback && defer(callback)
}
```
- example usage
```shell
...

'''js
req.session.regenerate(function(err) {
// will have a new session here
})
'''

#### Session.destroy(callback)

Destroys the session and will unset the 'req.session' property.
Once complete, the 'callback' will be invoked.

'''js
req.session.destroy(function(err) {
// cannot access session here
...
```

#### <a name="apidoc.element.express-session.MemoryStore.prototype.get"></a>[function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>get (sessionId, callback)](#apidoc.element.express-session.MemoryStore.prototype.get)
- description and source-code
```javascript
function get(sessionId, callback) {
  defer(callback, null, getSession.call(this, sessionId))
}
```
- example usage
```shell
...
'''js
var app = express()
var sess = {
  secret: 'keyboard cat',
  cookie: {}
}

if (app.get('env') === 'production') {
  app.set('trust proxy', 1) // trust first proxy
  sess.cookie.secure = true // serve secure cookies
}

app.use(session(sess))
'''
...
```

#### <a name="apidoc.element.express-session.MemoryStore.prototype.length"></a>[function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>length (callback)](#apidoc.element.express-session.MemoryStore.prototype.length)
- description and source-code
```javascript
function length(callback) {
  this.all(function (err, sessions) {
    if (err) return callback(err)
    callback(null, Object.keys(sessions).length)
  })
}
```
- example usage
```shell
...
### store.clear(callback)

**Optional**

This optional method is used to delete all sessions from the store. The
'callback' should be called as 'callback(error)' once the store is cleared.

### store.length(callback)

**Optional**

This optional method is used to get the count of all sessions in the store.
The 'callback' should be called as 'callback(error, len)'.

### store.get(sid, callback)
...
```

#### <a name="apidoc.element.express-session.MemoryStore.prototype.set"></a>[function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>set (sessionId, session, callback)](#apidoc.element.express-session.MemoryStore.prototype.set)
- description and source-code
```javascript
function set(sessionId, session, callback) {
  this.sessions[sessionId] = JSON.stringify(session)
  callback && defer(callback)
}
```
- example usage
```shell
...
an https-enabled website, i.e., HTTPS is necessary for secure cookies. If 'secure'
is set, and you access your site over HTTP, the cookie will not be set. If you
have your node.js behind a proxy and are using 'secure: true', you need to set
"trust proxy" in express:

'''js
var app = express()
app.set('trust proxy', 1) // trust first proxy
app.use(session({
  secret: 'keyboard cat',
  resave: false,
  saveUninitialized: true,
  cookie: { secure: true }
}))
'''
...
```

#### <a name="apidoc.element.express-session.MemoryStore.prototype.touch"></a>[function <span class="apidocSignatureSpan">express-session.MemoryStore.prototype.</span>touch (sessionId, session, callback)](#apidoc.element.express-session.MemoryStore.prototype.touch)
- description and source-code
```javascript
function touch(sessionId, session, callback) {
  var currentSession = getSession.call(this, sessionId)

  if (currentSession) {
    // update expiration
    currentSession.cookie = session.cookie
    this.sessions[sessionId] = JSON.stringify(currentSession)
  }

  callback && defer(callback)
}
```
- example usage
```shell
...

'''js
req.session.save(function(err) {
  // session saved
})
'''

#### Session.touch()

Updates the '.maxAge' property. Typically this is
not necessary to call, as the session middleware does this for you.

### req.session.id

Each session has a unique ID associated with it. This property will
...
```



# <a name="apidoc.module.express-session.Store"></a>[module express-session.Store](#apidoc.module.express-session.Store)

#### <a name="apidoc.element.express-session.Store.Store"></a>[function <span class="apidocSignatureSpan">express-session.</span>Store ()](#apidoc.element.express-session.Store.Store)
- description and source-code
```javascript
function Store() {
  EventEmitter.call(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-session.Store.super_"></a>[function <span class="apidocSignatureSpan">express-session.Store.</span>super_ ()](#apidoc.element.express-session.Store.super_)
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



# <a name="apidoc.module.express-session.Store.prototype"></a>[module express-session.Store.prototype](#apidoc.module.express-session.Store.prototype)

#### <a name="apidoc.element.express-session.Store.prototype.createSession"></a>[function <span class="apidocSignatureSpan">express-session.Store.prototype.</span>createSession (req, sess)](#apidoc.element.express-session.Store.prototype.createSession)
- description and source-code
```javascript
createSession = function (req, sess){
  var expires = sess.cookie.expires
    , orig = sess.cookie.originalMaxAge;
  sess.cookie = new Cookie(sess.cookie);
  if ('string' == typeof expires) sess.cookie.expires = new Date(expires);
  sess.cookie.originalMaxAge = orig;
  req.session = new Session(req, sess);
  return req.session;
}
```
- example usage
```shell
...
      // no session
      } else if (!sess) {
debug('no session found');
generate();
      // populate req.session
      } else {
debug('session found');
store.createSession(req, sess);
originalId = req.sessionID;
originalHash = hash(sess);

if (!resaveSession) {
  savedHash = originalHash
}
...
```

#### <a name="apidoc.element.express-session.Store.prototype.load"></a>[function <span class="apidocSignatureSpan">express-session.Store.prototype.</span>load (sid, fn)](#apidoc.element.express-session.Store.prototype.load)
- description and source-code
```javascript
load = function (sid, fn){
  var self = this;
  this.get(sid, function(err, sess){
    if (err) return fn(err);
    if (!sess) return fn();
    var req = { sessionID: sid, sessionStore: self };
    fn(null, self.createSession(req, sess))
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.express-session.Store.prototype.regenerate"></a>[function <span class="apidocSignatureSpan">express-session.Store.prototype.</span>regenerate (req, fn)](#apidoc.element.express-session.Store.prototype.regenerate)
- description and source-code
```javascript
regenerate = function (req, fn){
  var self = this;
  this.destroy(req.sessionID, function(err){
    self.generate(req);
    fn(err);
  });
}
```
- example usage
```shell
...
  } else {
    sess.views = 1
    res.end('welcome to the session demo. refresh!')
  }
})
'''

#### Session.regenerate(callback)

To regenerate the session simply invoke the method. Once complete,
a new SID and 'Session' instance will be initialized at 'req.session'
and the 'callback' will be invoked.

'''js
req.session.regenerate(function(err) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
