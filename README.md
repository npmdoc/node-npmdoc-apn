# api documentation for  [apn (v2.1.4)](https://github.com/node-apn/node-apn#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-apn.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-apn) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-apn.svg)](https://travis-ci.org/npmdoc/node-npmdoc-apn)
#### An interface to the Apple Push Notification service for Node.js

[![NPM](https://nodei.co/npm/apn.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/apn)

[![apidoc](https://npmdoc.github.io/node-npmdoc-apn/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-apn/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-apn/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-apn/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Andrew Naylor"
    },
    "bugs": {
        "url": "https://github.com/node-apn/node-apn/issues"
    },
    "contributors": [
        {
            "name": "Florian Reinhart"
        }
    ],
    "dependencies": {
        "debug": "^2.6.0",
        "http2": "https://github.com/node-apn/node-http2/archive/apn-2.1.4.tar.gz",
        "jsonwebtoken": "^7.2.1",
        "node-forge": "^0.6.48",
        "verror": "^1.9.0"
    },
    "description": "An interface to the Apple Push Notification service for Node.js",
    "devDependencies": {
        "chai": "3.x",
        "chai-as-promised": "*",
        "mocha": "*",
        "sinon": "^1.12.2",
        "sinon-chai": "^2.6.0"
    },
    "directories": {},
    "dist": {
        "shasum": "0d6cb583893affa4c1606b507b3052b42810677b",
        "tarball": "https://registry.npmjs.org/apn/-/apn-2.1.4.tgz"
    },
    "engines": {
        "node": ">= 4.6.0"
    },
    "eslintConfig": {
        "ecmaVersion": 6,
        "env": {
            "es6": true,
            "node": true
        }
    },
    "gitHead": "f7456dfe249905ce11a27b0217991d9cc36929a1",
    "homepage": "https://github.com/node-apn/node-apn#readme",
    "jshintConfig": {
        "node": true
    },
    "keywords": [
        "apple",
        "push",
        "push notifications",
        "iOS",
        "apns",
        "notifications"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "argon"
        },
        {
            "name": "florianreinhart"
        }
    ],
    "name": "apn",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/node-apn/node-apn.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "types": "index.d.ts",
    "version": "2.1.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module apn](#apidoc.module.apn)
1.  [function <span class="apidocSignatureSpan">apn.</span>Notification (payload)](#apidoc.element.apn.Notification)
1.  [function <span class="apidocSignatureSpan">apn.</span>Provider (options)](#apidoc.element.apn.Provider)
1.  [function <span class="apidocSignatureSpan">apn.</span>token (input)](#apidoc.element.apn.token)
1.  object <span class="apidocSignatureSpan">apn.</span>Notification.prototype
1.  object <span class="apidocSignatureSpan">apn.</span>Provider.prototype

#### [module apn.Notification](#apidoc.module.apn.Notification)
1.  [function <span class="apidocSignatureSpan">apn.</span>Notification (payload)](#apidoc.element.apn.Notification.Notification)

#### [module apn.Notification.prototype](#apidoc.module.apn.Notification.prototype)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>apsPayload ()](#apidoc.element.apn.Notification.prototype.apsPayload)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>compile ()](#apidoc.element.apn.Notification.prototype.compile)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>headers ()](#apidoc.element.apn.Notification.prototype.headers)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>length ()](#apidoc.element.apn.Notification.prototype.length)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>prepareAlert ()](#apidoc.element.apn.Notification.prototype.prepareAlert)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setAction (value)](#apidoc.element.apn.Notification.prototype.setAction)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setActionLocKey (value)](#apidoc.element.apn.Notification.prototype.setActionLocKey)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setAlert (value)](#apidoc.element.apn.Notification.prototype.setAlert)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setBadge (value)](#apidoc.element.apn.Notification.prototype.setBadge)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setBody (value)](#apidoc.element.apn.Notification.prototype.setBody)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setCategory (value)](#apidoc.element.apn.Notification.prototype.setCategory)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setContentAvailable (value)](#apidoc.element.apn.Notification.prototype.setContentAvailable)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setExpiry (value)](#apidoc.element.apn.Notification.prototype.setExpiry)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setLaunchImage (value)](#apidoc.element.apn.Notification.prototype.setLaunchImage)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setLocArgs (value)](#apidoc.element.apn.Notification.prototype.setLocArgs)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setLocKey (value)](#apidoc.element.apn.Notification.prototype.setLocKey)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setMdm (value)](#apidoc.element.apn.Notification.prototype.setMdm)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setMutableContent (value)](#apidoc.element.apn.Notification.prototype.setMutableContent)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setPayload (value)](#apidoc.element.apn.Notification.prototype.setPayload)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setPriority (value)](#apidoc.element.apn.Notification.prototype.setPriority)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setSound (value)](#apidoc.element.apn.Notification.prototype.setSound)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setSubtitle (value)](#apidoc.element.apn.Notification.prototype.setSubtitle)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setThreadId (value)](#apidoc.element.apn.Notification.prototype.setThreadId)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setTitle (value)](#apidoc.element.apn.Notification.prototype.setTitle)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setTitleLocArgs (value)](#apidoc.element.apn.Notification.prototype.setTitleLocArgs)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setTitleLocKey (value)](#apidoc.element.apn.Notification.prototype.setTitleLocKey)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setUrlArgs (value)](#apidoc.element.apn.Notification.prototype.setUrlArgs)
1.  [function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>toJSON ()](#apidoc.element.apn.Notification.prototype.toJSON)

#### [module apn.Provider](#apidoc.module.apn.Provider)
1.  [function <span class="apidocSignatureSpan">apn.</span>Provider (options)](#apidoc.element.apn.Provider.Provider)

#### [module apn.Provider.prototype](#apidoc.module.apn.Provider.prototype)
1.  [function <span class="apidocSignatureSpan">apn.Provider.prototype.</span>send (notification, recipients)](#apidoc.element.apn.Provider.prototype.send)
1.  [function <span class="apidocSignatureSpan">apn.Provider.prototype.</span>shutdown ()](#apidoc.element.apn.Provider.prototype.shutdown)



# <a name="apidoc.module.apn"></a>[module apn](#apidoc.module.apn)

#### <a name="apidoc.element.apn.Notification"></a>[function <span class="apidocSignatureSpan">apn.</span>Notification (payload)](#apidoc.element.apn.Notification)
- description and source-code
```javascript
function Notification(payload) {
  this.encoding = "utf8";
  this.payload = {};
  this.compiled = false;

  this.aps = {};
  this.expiry = 0;
  this.priority = 10;

  if (payload) {
    for(let key in payload) {
      if (payload.hasOwnProperty(key)) {
        this[key] = payload[key];
      }
    }
  }
}
```
- example usage
```shell
...
'''javascript
let deviceToken = "a9d0ed10e9cfd022a61cb08753f49c5a0b0dfb383697bf9f9d750a1003da19c7"
'''

Create a notification object, configuring it with the relevant parameters (See the [notification documentation](doc/notification
.markdown) for more details.)

'''javascript
var note = new apn.Notification();

note.expiry = Math.floor(Date.now() / 1000) + 3600; // Expires 1 hour from now.
note.badge = 3;
note.sound = "ping.aiff";
note.alert = "\uD83D\uDCE7 \u2709 You have a new message";
note.payload = {'messageFrom': 'John Appleseed'};
note.topic = "<your-app-bundle-id>";
...
```

#### <a name="apidoc.element.apn.Provider"></a>[function <span class="apidocSignatureSpan">apn.</span>Provider (options)](#apidoc.element.apn.Provider)
- description and source-code
```javascript
function Provider(options) {
  if(false === (this instanceof Provider)) {
    return new Provider(options);
  }

  this.client = new Client(options);

  EventEmitter.call(this);
}
```
- example usage
```shell
...
    key: "path/to/key.p8",
    keyId: "T0K3NK3Y1D",
    teamId: "T34M1D"
  },
  production: false
};

var apnProvider = new apn.Provider(options);
'''

By default, the provider will connect to the sandbox unless the environment variable 'NODE_ENV=production' is set.

For more information about configuration options consult the [provider documentation](doc/provider.markdown).

Help with preparing the key and certificate files for connection can be found in the [wiki][certificateWiki]
...
```

#### <a name="apidoc.element.apn.token"></a>[function <span class="apidocSignatureSpan">apn.</span>token (input)](#apidoc.element.apn.token)
- description and source-code
```javascript
function token(input) {
  let token;

  if (typeof input === "string") {
    token = input;
  } else if (Buffer.isBuffer(input)) {
    token = input.toString("hex");
  }

  token = token.replace(/[^0-9a-f]/gi, "");

  if (token.length === 0) {
    throw new Error("Token has invalid length");
  }

  return token;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.apn.Notification"></a>[module apn.Notification](#apidoc.module.apn.Notification)

#### <a name="apidoc.element.apn.Notification.Notification"></a>[function <span class="apidocSignatureSpan">apn.</span>Notification (payload)](#apidoc.element.apn.Notification.Notification)
- description and source-code
```javascript
function Notification(payload) {
  this.encoding = "utf8";
  this.payload = {};
  this.compiled = false;

  this.aps = {};
  this.expiry = 0;
  this.priority = 10;

  if (payload) {
    for(let key in payload) {
      if (payload.hasOwnProperty(key)) {
        this[key] = payload[key];
      }
    }
  }
}
```
- example usage
```shell
...
'''javascript
let deviceToken = "a9d0ed10e9cfd022a61cb08753f49c5a0b0dfb383697bf9f9d750a1003da19c7"
'''

Create a notification object, configuring it with the relevant parameters (See the [notification documentation](doc/notification
.markdown) for more details.)

'''javascript
var note = new apn.Notification();

note.expiry = Math.floor(Date.now() / 1000) + 3600; // Expires 1 hour from now.
note.badge = 3;
note.sound = "ping.aiff";
note.alert = "\uD83D\uDCE7 \u2709 You have a new message";
note.payload = {'messageFrom': 'John Appleseed'};
note.topic = "<your-app-bundle-id>";
...
```



# <a name="apidoc.module.apn.Notification.prototype"></a>[module apn.Notification.prototype](#apidoc.module.apn.Notification.prototype)

#### <a name="apidoc.element.apn.Notification.prototype.apsPayload"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>apsPayload ()](#apidoc.element.apn.Notification.prototype.apsPayload)
- description and source-code
```javascript
apsPayload = function () {
  var aps = this.aps;

  return Object.keys(aps).find( key => aps[key] !== undefined ) ? aps : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.compile"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>compile ()](#apidoc.element.apn.Notification.prototype.compile)
- description and source-code
```javascript
compile = function () {
  if(!this.compiled) {
    this.compiled = JSON.stringify(this);
  }
  return this.compiled;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.headers"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>headers ()](#apidoc.element.apn.Notification.prototype.headers)
- description and source-code
```javascript
function headers() {
  let headers = {};

  if (this.priority !== 10) {
    headers["apns-priority"] = this.priority;
  }

  if (this.id) {
    headers["apns-id"] = this.id;
  }

  if (this.expiry > 0) {
    headers["apns-expiration"] = this.expiry;
  }

  if (this.topic) {
    headers["apns-topic"] = this.topic;
  }

  if (this.collapseId) {
    headers["apns-collapse-id"] = this.collapseId;
  }

  return headers;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.length"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>length ()](#apidoc.element.apn.Notification.prototype.length)
- description and source-code
```javascript
length = function () {
  return Buffer.byteLength(this.compile(), this.encoding || "utf8");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.prepareAlert"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>prepareAlert ()](#apidoc.element.apn.Notification.prototype.prepareAlert)
- description and source-code
```javascript
prepareAlert = function () {
  if (typeof this.aps.alert !== "object") {
    this.aps.alert = {"body": this.aps.alert};
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setAction"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setAction (value)](#apidoc.element.apn.Notification.prototype.setAction)
- description and source-code
```javascript
setAction = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setActionLocKey"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setActionLocKey (value)](#apidoc.element.apn.Notification.prototype.setActionLocKey)
- description and source-code
```javascript
setActionLocKey = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setAlert"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setAlert (value)](#apidoc.element.apn.Notification.prototype.setAlert)
- description and source-code
```javascript
setAlert = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setBadge"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setBadge (value)](#apidoc.element.apn.Notification.prototype.setBadge)
- description and source-code
```javascript
setBadge = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setBody"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setBody (value)](#apidoc.element.apn.Notification.prototype.setBody)
- description and source-code
```javascript
setBody = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setCategory"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setCategory (value)](#apidoc.element.apn.Notification.prototype.setCategory)
- description and source-code
```javascript
setCategory = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setContentAvailable"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setContentAvailable (value)](#apidoc.element.apn.Notification.prototype.setContentAvailable)
- description and source-code
```javascript
setContentAvailable = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setExpiry"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setExpiry (value)](#apidoc.element.apn.Notification.prototype.setExpiry)
- description and source-code
```javascript
setExpiry = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setLaunchImage"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setLaunchImage (value)](#apidoc.element.apn.Notification.prototype.setLaunchImage)
- description and source-code
```javascript
setLaunchImage = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setLocArgs"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setLocArgs (value)](#apidoc.element.apn.Notification.prototype.setLocArgs)
- description and source-code
```javascript
setLocArgs = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setLocKey"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setLocKey (value)](#apidoc.element.apn.Notification.prototype.setLocKey)
- description and source-code
```javascript
setLocKey = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setMdm"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setMdm (value)](#apidoc.element.apn.Notification.prototype.setMdm)
- description and source-code
```javascript
setMdm = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setMutableContent"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setMutableContent (value)](#apidoc.element.apn.Notification.prototype.setMutableContent)
- description and source-code
```javascript
setMutableContent = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setPayload"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setPayload (value)](#apidoc.element.apn.Notification.prototype.setPayload)
- description and source-code
```javascript
setPayload = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setPriority"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setPriority (value)](#apidoc.element.apn.Notification.prototype.setPriority)
- description and source-code
```javascript
setPriority = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setSound"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setSound (value)](#apidoc.element.apn.Notification.prototype.setSound)
- description and source-code
```javascript
setSound = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setSubtitle"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setSubtitle (value)](#apidoc.element.apn.Notification.prototype.setSubtitle)
- description and source-code
```javascript
setSubtitle = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setThreadId"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setThreadId (value)](#apidoc.element.apn.Notification.prototype.setThreadId)
- description and source-code
```javascript
setThreadId = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setTitle"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setTitle (value)](#apidoc.element.apn.Notification.prototype.setTitle)
- description and source-code
```javascript
setTitle = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setTitleLocArgs"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setTitleLocArgs (value)](#apidoc.element.apn.Notification.prototype.setTitleLocArgs)
- description and source-code
```javascript
setTitleLocArgs = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setTitleLocKey"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setTitleLocKey (value)](#apidoc.element.apn.Notification.prototype.setTitleLocKey)
- description and source-code
```javascript
setTitleLocKey = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.setUrlArgs"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>setUrlArgs (value)](#apidoc.element.apn.Notification.prototype.setUrlArgs)
- description and source-code
```javascript
setUrlArgs = function (value) {
  this[propName] = value;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.apn.Notification.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">apn.Notification.prototype.</span>toJSON ()](#apidoc.element.apn.Notification.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  if (this.rawPayload != null) {
    return this.rawPayload;
  }

  if (typeof this._mdm === "string") {
    return { "mdm": this._mdm };
  }

  return Object.assign({}, this.payload, {aps: this.apsPayload()});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.apn.Provider"></a>[module apn.Provider](#apidoc.module.apn.Provider)

#### <a name="apidoc.element.apn.Provider.Provider"></a>[function <span class="apidocSignatureSpan">apn.</span>Provider (options)](#apidoc.element.apn.Provider.Provider)
- description and source-code
```javascript
function Provider(options) {
  if(false === (this instanceof Provider)) {
    return new Provider(options);
  }

  this.client = new Client(options);

  EventEmitter.call(this);
}
```
- example usage
```shell
...
    key: "path/to/key.p8",
    keyId: "T0K3NK3Y1D",
    teamId: "T34M1D"
  },
  production: false
};

var apnProvider = new apn.Provider(options);
'''

By default, the provider will connect to the sandbox unless the environment variable 'NODE_ENV=production' is set.

For more information about configuration options consult the [provider documentation](doc/provider.markdown).

Help with preparing the key and certificate files for connection can be found in the [wiki][certificateWiki]
...
```



# <a name="apidoc.module.apn.Provider.prototype"></a>[module apn.Provider.prototype](#apidoc.module.apn.Provider.prototype)

#### <a name="apidoc.element.apn.Provider.prototype.send"></a>[function <span class="apidocSignatureSpan">apn.Provider.prototype.</span>send (notification, recipients)](#apidoc.element.apn.Provider.prototype.send)
- description and source-code
```javascript
function send(notification, recipients) {
  const builtNotification = {
    headers: notification.headers(),
    body:    notification.compile(),
  };

  if (!Array.isArray(recipients)) {
    recipients = [recipients];
  }

  return Promise.all( recipients.map( token => this.client.write(builtNotification, token) ))
    .then( responses => {
    let sent = [];
    let failed = [];

    responses.forEach( response => {
      if (response.status || response.error) {
        failed.push(response);
      } else {
        sent.push(response);
      }
    });
    return {sent, failed};
  });
}
```
- example usage
```shell
...
note.payload = {'messageFrom': 'John Appleseed'};
note.topic = "<your-app-bundle-id>";
'''

Send the notification to the API with 'send', which returns a promise.

'''javascript
apnProvider.send(note, deviceToken).then( (result) => {
  // see documentation for an explanation of result
});
'''

This will result in the the following notification payload being sent to the device

'''json
...
```

#### <a name="apidoc.element.apn.Provider.prototype.shutdown"></a>[function <span class="apidocSignatureSpan">apn.Provider.prototype.</span>shutdown ()](#apidoc.element.apn.Provider.prototype.shutdown)
- description and source-code
```javascript
function shutdown() {
  this.client.shutdown();
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
