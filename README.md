# api documentation for  [passport-twitter (v1.0.4)](https://github.com/jaredhanson/passport-twitter#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-passport-twitter.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-passport-twitter) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-passport-twitter.svg)](https://travis-ci.org/npmdoc/node-npmdoc-passport-twitter)
#### Twitter authentication strategy for Passport.

[![NPM](https://nodei.co/npm/passport-twitter.png?downloads=true)](https://www.npmjs.com/package/passport-twitter)

[![apidoc](https://npmdoc.github.io/node-npmdoc-passport-twitter/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-passport-twitter_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-passport-twitter/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-passport-twitter/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-passport-twitter/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jared Hanson",
        "email": "jaredhanson@gmail.com",
        "url": "http://www.jaredhanson.net/"
    },
    "bugs": {
        "url": "http://github.com/jaredhanson/passport-twitter/issues"
    },
    "dependencies": {
        "passport-oauth1": "1.x.x",
        "xtraverse": "0.1.x"
    },
    "description": "Twitter authentication strategy for Passport.",
    "devDependencies": {
        "chai": "2.x.x",
        "chai-passport-strategy": "1.x.x",
        "make-node": "0.3.x",
        "mocha": "1.x.x"
    },
    "directories": {},
    "dist": {
        "shasum": "01a799e1f760bf2de49f2ba5fba32282f18932d7",
        "tarball": "https://registry.npmjs.org/passport-twitter/-/passport-twitter-1.0.4.tgz"
    },
    "engines": {
        "node": ">= 0.4.0"
    },
    "gitHead": "46c1fe216f2539463c6e7043855fe4264bab8f96",
    "homepage": "https://github.com/jaredhanson/passport-twitter#readme",
    "keywords": [
        "passport",
        "twitter",
        "auth",
        "authn",
        "authentication",
        "identity"
    ],
    "license": "MIT",
    "licenses": [
        {
            "type": "MIT",
            "url": "http://opensource.org/licenses/MIT"
        }
    ],
    "main": "./lib",
    "maintainers": [
        {
            "name": "jaredhanson",
            "email": "jaredhanson@gmail.com"
        }
    ],
    "name": "passport-twitter",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/jaredhanson/passport-twitter.git"
    },
    "scripts": {
        "test": "mocha --require test/bootstrap/node test/*.test.js"
    },
    "version": "1.0.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module passport-twitter](#apidoc.module.passport-twitter)
1.  [function <span class="apidocSignatureSpan">passport-twitter.</span>Strategy (options, verify)](#apidoc.element.passport-twitter.Strategy)
1.  [function <span class="apidocSignatureSpan">passport-twitter.</span>super_ (options, verify)](#apidoc.element.passport-twitter.super_)
1.  [function <span class="apidocSignatureSpan">passport-twitter.</span>super_.InternalOAuthError (message, err)](#apidoc.element.passport-twitter.super_.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-twitter.</span>super_.super_ ()](#apidoc.element.passport-twitter.super_.super_)
1.  object <span class="apidocSignatureSpan">passport-twitter.</span>profile
1.  object <span class="apidocSignatureSpan">passport-twitter.</span>super_.InternalOAuthError.prototype
1.  object <span class="apidocSignatureSpan">passport-twitter.</span>super_.prototype
1.  object <span class="apidocSignatureSpan">passport-twitter.</span>super_.super_.prototype

#### [module passport-twitter.profile](#apidoc.module.passport-twitter.profile)
1.  [function <span class="apidocSignatureSpan">passport-twitter.profile.</span>parse (json)](#apidoc.element.passport-twitter.profile.parse)

#### [module passport-twitter.super_](#apidoc.module.passport-twitter.super_)
1.  [function <span class="apidocSignatureSpan">passport-twitter.</span>super_ ()](#apidoc.element.passport-twitter.super_.super_)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.</span>InternalOAuthError (message, err)](#apidoc.element.passport-twitter.super_.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.</span>Strategy (options, verify)](#apidoc.element.passport-twitter.super_.Strategy)

#### [module passport-twitter.super_.InternalOAuthError](#apidoc.module.passport-twitter.super_.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.</span>InternalOAuthError (message, err)](#apidoc.element.passport-twitter.super_.InternalOAuthError.InternalOAuthError)

#### [module passport-twitter.super_.InternalOAuthError.prototype](#apidoc.module.passport-twitter.super_.InternalOAuthError.prototype)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.InternalOAuthError.prototype.</span>toString ()](#apidoc.element.passport-twitter.super_.InternalOAuthError.prototype.toString)

#### [module passport-twitter.super_.prototype](#apidoc.module.passport-twitter.super_.prototype)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>_createOAuthError (message, err)](#apidoc.element.passport-twitter.super_.prototype._createOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>_loadUserProfile (token, tokenSecret, params, done)](#apidoc.element.passport-twitter.super_.prototype._loadUserProfile)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>authenticate (req, options)](#apidoc.element.passport-twitter.super_.prototype.authenticate)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>parseErrorResponse (body, status)](#apidoc.element.passport-twitter.super_.prototype.parseErrorResponse)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>requestTokenParams (options)](#apidoc.element.passport-twitter.super_.prototype.requestTokenParams)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>userAuthorizationParams (options)](#apidoc.element.passport-twitter.super_.prototype.userAuthorizationParams)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>userProfile (token, tokenSecret, params, done)](#apidoc.element.passport-twitter.super_.prototype.userProfile)

#### [module passport-twitter.super_.super_](#apidoc.module.passport-twitter.super_.super_)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.</span>super_ ()](#apidoc.element.passport-twitter.super_.super_.super_)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.super_.</span>Strategy ()](#apidoc.element.passport-twitter.super_.super_.Strategy)

#### [module passport-twitter.super_.super_.prototype](#apidoc.module.passport-twitter.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">passport-twitter.super_.super_.prototype.</span>authenticate (req, options)](#apidoc.element.passport-twitter.super_.super_.prototype.authenticate)



# <a name="apidoc.module.passport-twitter"></a>[module passport-twitter](#apidoc.module.passport-twitter)

#### <a name="apidoc.element.passport-twitter.Strategy"></a>[function <span class="apidocSignatureSpan">passport-twitter.</span>Strategy (options, verify)](#apidoc.element.passport-twitter.Strategy)
- description and source-code
```javascript
function Strategy(options, verify) {
  options = options || {};
  options.requestTokenURL = options.requestTokenURL || 'https://api.twitter.com/oauth/request_token';
  options.accessTokenURL = options.accessTokenURL || 'https://api.twitter.com/oauth/access_token';
  options.userAuthorizationURL = options.userAuthorizationURL || 'https://api.twitter.com/oauth/authenticate';
  options.sessionKey = options.sessionKey || 'oauth:twitter';

  OAuthStrategy.call(this, options, verify);
  this.name = 'twitter';
  this._userProfileURL = options.userProfileURL || 'https://api.twitter.com/1.1/account/verify_credentials.json';
  this._skipExtendedUserProfile = (options.skipExtendedUserProfile !== undefined) ? options.skipExtendedUserProfile : false;
  this._includeEmail = (options.includeEmail !== undefined) ? options.includeEmail : false;
  this._includeStatus = (options.includeStatus !== undefined) ? options.includeStatus : true;
  this._includeEntities = (options.includeEntities !== undefined) ? options.includeEntities : true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_"></a>[function <span class="apidocSignatureSpan">passport-twitter.</span>super_ (options, verify)](#apidoc.element.passport-twitter.super_)
- description and source-code
```javascript
function OAuthStrategy(options, verify) {
  if (typeof options == 'function') {
    verify = options;
    options = undefined;
  }
  options = options || {};

  if (!verify) { throw new TypeError('OAuthStrategy requires a verify callback'); }
  if (!options.requestTokenURL) { throw new TypeError('OAuthStrategy requires a requestTokenURL option'); }
  if (!options.accessTokenURL) { throw new TypeError('OAuthStrategy requires a accessTokenURL option'); }
  if (!options.userAuthorizationURL) { throw new TypeError('OAuthStrategy requires a userAuthorizationURL option'); }
  if (!options.consumerKey) { throw new TypeError('OAuthStrategy requires a consumerKey option'); }
  if (options.consumerSecret === undefined) { throw new TypeError('OAuthStrategy requires a consumerSecret option'); }

  passport.Strategy.call(this);
  this.name = 'oauth';
  this._verify = verify;

  // NOTE: The _oauth property is considered "protected".  Subclasses are
  //       allowed to use it when making protected resource requests to retrieve
  //       the user profile.
  this._oauth = new OAuth(options.requestTokenURL, options.accessTokenURL,
                          options.consumerKey,  options.consumerSecret,
                          '1.0', null, options.signatureMethod || 'HMAC-SHA1',
                          null, options.customHeaders);

  this._userAuthorizationURL = options.userAuthorizationURL;
  this._callbackURL = options.callbackURL;
  this._key = options.sessionKey || 'oauth';
  this._requestTokenStore = options.requestTokenStore || new SessionRequestTokenStore({ key: this._key });
  this._trustProxy = options.proxy;
  this._passReqToCallback = options.passReqToCallback;
  this._skipUserProfile = (options.skipUserProfile === undefined) ? false : options.skipUserProfile;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-twitter.</span>super_.InternalOAuthError (message, err)](#apidoc.element.passport-twitter.super_.InternalOAuthError)
- description and source-code
```javascript
function InternalOAuthError(message, err) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.oauthError = err;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_.super_"></a>[function <span class="apidocSignatureSpan">passport-twitter.</span>super_.super_ ()](#apidoc.element.passport-twitter.super_.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-twitter.profile"></a>[module passport-twitter.profile](#apidoc.module.passport-twitter.profile)

#### <a name="apidoc.element.passport-twitter.profile.parse"></a>[function <span class="apidocSignatureSpan">passport-twitter.profile.</span>parse (json)](#apidoc.element.passport-twitter.profile.parse)
- description and source-code
```javascript
parse = function (json) {
  if ('string' == typeof json) {
    json = JSON.parse(json);
  }

  var profile = {};
  profile.id = String(json.id);
  if (json.id_str) { profile.id = json.id_str; }
  profile.username = json.screen_name;
  profile.displayName = json.name;
  if (json.email) {
    profile.emails = [{ value: json.email }];
  }
  profile.photos = [{ value: json.profile_image_url_https }];

  return profile;
}
```
- example usage
```shell
...
 *
 * @param {object|string} json
 * @return {object}
 * @api public
 */
exports.parse = function(json) {
if ('string' == typeof json) {
  json = JSON.parse(json);
}

var profile = {};
profile.id = String(json.id);
if (json.id_str) { profile.id = json.id_str; }
profile.username = json.screen_name;
profile.displayName = json.name;
...
```



# <a name="apidoc.module.passport-twitter.super_"></a>[module passport-twitter.super_](#apidoc.module.passport-twitter.super_)

#### <a name="apidoc.element.passport-twitter.super_.super_"></a>[function <span class="apidocSignatureSpan">passport-twitter.</span>super_ ()](#apidoc.element.passport-twitter.super_.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.</span>InternalOAuthError (message, err)](#apidoc.element.passport-twitter.super_.InternalOAuthError)
- description and source-code
```javascript
function InternalOAuthError(message, err) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.oauthError = err;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_.Strategy"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.</span>Strategy (options, verify)](#apidoc.element.passport-twitter.super_.Strategy)
- description and source-code
```javascript
function OAuthStrategy(options, verify) {
  if (typeof options == 'function') {
    verify = options;
    options = undefined;
  }
  options = options || {};

  if (!verify) { throw new TypeError('OAuthStrategy requires a verify callback'); }
  if (!options.requestTokenURL) { throw new TypeError('OAuthStrategy requires a requestTokenURL option'); }
  if (!options.accessTokenURL) { throw new TypeError('OAuthStrategy requires a accessTokenURL option'); }
  if (!options.userAuthorizationURL) { throw new TypeError('OAuthStrategy requires a userAuthorizationURL option'); }
  if (!options.consumerKey) { throw new TypeError('OAuthStrategy requires a consumerKey option'); }
  if (options.consumerSecret === undefined) { throw new TypeError('OAuthStrategy requires a consumerSecret option'); }

  passport.Strategy.call(this);
  this.name = 'oauth';
  this._verify = verify;

  // NOTE: The _oauth property is considered "protected".  Subclasses are
  //       allowed to use it when making protected resource requests to retrieve
  //       the user profile.
  this._oauth = new OAuth(options.requestTokenURL, options.accessTokenURL,
                          options.consumerKey,  options.consumerSecret,
                          '1.0', null, options.signatureMethod || 'HMAC-SHA1',
                          null, options.customHeaders);

  this._userAuthorizationURL = options.userAuthorizationURL;
  this._callbackURL = options.callbackURL;
  this._key = options.sessionKey || 'oauth';
  this._requestTokenStore = options.requestTokenStore || new SessionRequestTokenStore({ key: this._key });
  this._trustProxy = options.proxy;
  this._passReqToCallback = options.passReqToCallback;
  this._skipUserProfile = (options.skipUserProfile === undefined) ? false : options.skipUserProfile;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-twitter.super_.InternalOAuthError"></a>[module passport-twitter.super_.InternalOAuthError](#apidoc.module.passport-twitter.super_.InternalOAuthError)

#### <a name="apidoc.element.passport-twitter.super_.InternalOAuthError.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.</span>InternalOAuthError (message, err)](#apidoc.element.passport-twitter.super_.InternalOAuthError.InternalOAuthError)
- description and source-code
```javascript
function InternalOAuthError(message, err) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.oauthError = err;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-twitter.super_.InternalOAuthError.prototype"></a>[module passport-twitter.super_.InternalOAuthError.prototype](#apidoc.module.passport-twitter.super_.InternalOAuthError.prototype)

#### <a name="apidoc.element.passport-twitter.super_.InternalOAuthError.prototype.toString"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.InternalOAuthError.prototype.</span>toString ()](#apidoc.element.passport-twitter.super_.InternalOAuthError.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var m = this.name;
  if (this.message) { m += ': ' + this.message; }
  if (this.oauthError) {
    if (this.oauthError instanceof Error) {
      m = this.oauthError.toString();
    } else if (this.oauthError.statusCode && this.oauthError.data) {
      m += ' (status: ' + this.oauthError.statusCode + ' data: ' + this.oauthError.data + ')';
    }
  }
  return m;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-twitter.super_.prototype"></a>[module passport-twitter.super_.prototype](#apidoc.module.passport-twitter.super_.prototype)

#### <a name="apidoc.element.passport-twitter.super_.prototype._createOAuthError"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>_createOAuthError (message, err)](#apidoc.element.passport-twitter.super_.prototype._createOAuthError)
- description and source-code
```javascript
_createOAuthError = function (message, err) {
  var e;
  if (err.statusCode && err.data) {
    try {
      e = this.parseErrorResponse(err.data, err.statusCode);
    } catch (_) {}
  }
  if (!e) { e = new InternalOAuthError(message, err); }
  return e;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_.prototype._loadUserProfile"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>_loadUserProfile (token, tokenSecret, params, done)](#apidoc.element.passport-twitter.super_.prototype._loadUserProfile)
- description and source-code
```javascript
_loadUserProfile = function (token, tokenSecret, params, done) {
  var self = this;

  function loadIt() {
    return self.userProfile(token, tokenSecret, params, done);
  }
  function skipIt() {
    return done(null);
  }

  if (typeof this._skipUserProfile == 'function' && this._skipUserProfile.length > 1) {
    // async
    this._skipUserProfile(token, tokenSecret, function(err, skip) {
      if (err) { return done(err); }
      if (!skip) { return loadIt(); }
      return skipIt();
    });
  } else {
    var skip = (typeof this._skipUserProfile == 'function') ? this._skipUserProfile() : this._skipUserProfile;
    if (!skip) { return loadIt(); }
    return skipIt();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>authenticate (req, options)](#apidoc.element.passport-twitter.super_.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (req, options) {
  options = options || {};

  var self = this;
  var meta = {
    requestTokenURL: this._oauth._requestUrl,
    accessTokenURL: this._oauth._accessUrl,
    userAuthorizationURL:  this._userAuthorizationURL,
    consumerKey: this._oauth._consumerKey
  }

  if (req.query && req.query.oauth_token) {
    // The request being authenticated contains an oauth_token parameter in the
    // query portion of the URL.  This indicates that the service provider has
    // redirected the user back to the application, after authenticating the
    // user and obtaining their authorization.
    //
    // The value of the oauth_token parameter is the request token.  Together
    // with knowledge of the token secret (stored in the session), the request
    // token can be exchanged for an access token and token secret.
    //
    // This access token and token secret, along with the optional ability to
    // fetch profile information from the service provider, is sufficient to
    // establish the identity of the user.
    var oauthToken = req.query.oauth_token;

    function loaded(err, oauthTokenSecret, state) {
      if (err) { return self.error(err); }
      if (!oauthTokenSecret) {
        return self.fail(state, 403);
      }

      // NOTE: The oauth_verifier parameter will be supplied in the query portion
      //       of the redirect URL, if the server supports OAuth 1.0a.
      var oauthVerifier = req.query.oauth_verifier || null;

      self._oauth.getOAuthAccessToken(oauthToken, oauthTokenSecret, oauthVerifier, function(err, token, tokenSecret, params) {
        if (err) { return self.error(self._createOAuthError('Failed to obtain access token', err)); }

        function destroyed(err) {
          if (err) { return self.error(err); }

          self._loadUserProfile(token, tokenSecret, params, function(err, profile) {
            if (err) { return self.error(err); }

            function verified(err, user, info) {
              if (err) { return self.error(err); }
              if (!user) { return self.fail(info); }

              info = info || {};
              if (state) { info.state = state; }
              self.success(user, info);
            }

            try {
              if (self._passReqToCallback) {
                var arity = self._verify.length;
                if (arity == 6) {
                  self._verify(req, token, tokenSecret, params, profile, verified);
                } else { // arity == 5
                  self._verify(req, token, tokenSecret, profile, verified);
                }
              } else {
                var arity = self._verify.length;
                if (arity == 5) {
                  self._verify(token, tokenSecret, params, profile, verified);
                } else { // arity == 4
                  self._verify(token, tokenSecret, profile, verified);
                }
              }
            } catch (ex) {
              return self.error(ex);
            }
          });
        }

        // The request token has been exchanged for an access token.  Since the
        // request token is a single-use token, that data can be removed from the
        // store.
        try {
          var arity = self._requestTokenStore.destroy.length;
          if (arity == 4) {
            self._requestTokenStore.destroy(req, oauthToken, meta, destroyed);
          } else { // arity == 3
            self._requestTokenStore.destroy(req, oauthToken, destroyed);
          }
        } catch (ex) {
          return self.error(ex);
        }
      });
    }

    try {
      var arity = self._requestTokenStore.get.length;
      if (arity == 4) {
        this._requestTokenStore.get(req, oauthToken, meta, loaded);
      } else { // arity == 3
        this._requestTokenStore.get(req, oauthToken, loaded);
      }
    } catch (ex) {
      return this.error(ex);
    }
  } else {
    // In order to authenticate via OAuth, the application must obtain a request
    // token from the service provider and redirect th ...
```
- example usage
```shell
...
      return cb(err, user);
    });
  }
));

#### Authenticate Requests

Use 'passport.authenticate()', specifying the ''twitter'' strategy, to
authenticate requests.

For example, as route middleware in an [Express](http://expressjs.com/)
application:

app.get('/auth/twitter',
  passport.authenticate('twitter'));
...
```

#### <a name="apidoc.element.passport-twitter.super_.prototype.parseErrorResponse"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>parseErrorResponse (body, status)](#apidoc.element.passport-twitter.super_.prototype.parseErrorResponse)
- description and source-code
```javascript
parseErrorResponse = function (body, status) {
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_.prototype.requestTokenParams"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>requestTokenParams (options)](#apidoc.element.passport-twitter.super_.prototype.requestTokenParams)
- description and source-code
```javascript
requestTokenParams = function (options) {
  return {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_.prototype.userAuthorizationParams"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>userAuthorizationParams (options)](#apidoc.element.passport-twitter.super_.prototype.userAuthorizationParams)
- description and source-code
```javascript
userAuthorizationParams = function (options) {
  return {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_.prototype.userProfile"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.prototype.</span>userProfile (token, tokenSecret, params, done)](#apidoc.element.passport-twitter.super_.prototype.userProfile)
- description and source-code
```javascript
userProfile = function (token, tokenSecret, params, done) {
  return done(null, {});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-twitter.super_.super_"></a>[module passport-twitter.super_.super_](#apidoc.module.passport-twitter.super_.super_)

#### <a name="apidoc.element.passport-twitter.super_.super_.super_"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.</span>super_ ()](#apidoc.element.passport-twitter.super_.super_.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-twitter.super_.super_.Strategy"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.super_.</span>Strategy ()](#apidoc.element.passport-twitter.super_.super_.Strategy)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-twitter.super_.super_.prototype"></a>[module passport-twitter.super_.super_.prototype](#apidoc.module.passport-twitter.super_.super_.prototype)

#### <a name="apidoc.element.passport-twitter.super_.super_.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">passport-twitter.super_.super_.prototype.</span>authenticate (req, options)](#apidoc.element.passport-twitter.super_.super_.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (req, options) {
  throw new Error('Strategy#authenticate must be overridden by subclass');
}
```
- example usage
```shell
...
      return cb(err, user);
    });
  }
));

#### Authenticate Requests

Use 'passport.authenticate()', specifying the ''twitter'' strategy, to
authenticate requests.

For example, as route middleware in an [Express](http://expressjs.com/)
application:

app.get('/auth/twitter',
  passport.authenticate('twitter'));
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
