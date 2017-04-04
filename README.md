# api documentation for  [passport-facebook (v2.1.1)](https://github.com/jaredhanson/passport-facebook#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-passport-facebook.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-passport-facebook) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-passport-facebook.svg)](https://travis-ci.org/npmdoc/node-npmdoc-passport-facebook)
#### Facebook authentication strategy for Passport.

[![NPM](https://nodei.co/npm/passport-facebook.png?downloads=true)](https://www.npmjs.com/package/passport-facebook)

[![apidoc](https://npmdoc.github.io/node-npmdoc-passport-facebook/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-passport-facebook_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-passport-facebook/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-passport-facebook/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-passport-facebook/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jared Hanson",
        "email": "jaredhanson@gmail.com",
        "url": "http://www.jaredhanson.net/"
    },
    "bugs": {
        "url": "http://github.com/jaredhanson/passport-facebook/issues"
    },
    "dependencies": {
        "passport-oauth2": "1.x.x"
    },
    "description": "Facebook authentication strategy for Passport.",
    "devDependencies": {
        "chai": "2.x.x",
        "chai-passport-strategy": "1.x.x",
        "make-node": "0.3.x",
        "mocha": "1.x.x"
    },
    "directories": {},
    "dist": {
        "shasum": "c39d0b52ae4d59163245a4e21a7b9b6321303311",
        "tarball": "https://registry.npmjs.org/passport-facebook/-/passport-facebook-2.1.1.tgz"
    },
    "engines": {
        "node": ">= 0.4.0"
    },
    "gitHead": "2b74dd0eff976e85b029178e8012cb3703231112",
    "homepage": "https://github.com/jaredhanson/passport-facebook#readme",
    "keywords": [
        "passport",
        "facebook",
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
    "name": "passport-facebook",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/jaredhanson/passport-facebook.git"
    },
    "scripts": {
        "test": "mocha --require test/bootstrap/node test/*.test.js"
    },
    "version": "2.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module passport-facebook](#apidoc.module.passport-facebook)
1.  [function <span class="apidocSignatureSpan">passport-facebook.</span>Strategy (options, verify)](#apidoc.element.passport-facebook.Strategy)
1.  [function <span class="apidocSignatureSpan">passport-facebook.</span>super_ (options, verify)](#apidoc.element.passport-facebook.super_)
1.  [function <span class="apidocSignatureSpan">passport-facebook.</span>super_.InternalOAuthError (message, err)](#apidoc.element.passport-facebook.super_.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-facebook.</span>super_.super_ ()](#apidoc.element.passport-facebook.super_.super_)
1.  object <span class="apidocSignatureSpan">passport-facebook.</span>profile
1.  object <span class="apidocSignatureSpan">passport-facebook.</span>super_.InternalOAuthError.prototype
1.  object <span class="apidocSignatureSpan">passport-facebook.</span>super_.prototype
1.  object <span class="apidocSignatureSpan">passport-facebook.</span>super_.super_.prototype

#### [module passport-facebook.profile](#apidoc.module.passport-facebook.profile)
1.  [function <span class="apidocSignatureSpan">passport-facebook.profile.</span>parse (json)](#apidoc.element.passport-facebook.profile.parse)

#### [module passport-facebook.super_](#apidoc.module.passport-facebook.super_)
1.  [function <span class="apidocSignatureSpan">passport-facebook.</span>super_ ()](#apidoc.element.passport-facebook.super_.super_)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.</span>AuthorizationError (message, code, uri, status)](#apidoc.element.passport-facebook.super_.AuthorizationError)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.</span>InternalOAuthError (message, err)](#apidoc.element.passport-facebook.super_.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.</span>Strategy (options, verify)](#apidoc.element.passport-facebook.super_.Strategy)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.</span>TokenError (message, code, uri, status)](#apidoc.element.passport-facebook.super_.TokenError)

#### [module passport-facebook.super_.InternalOAuthError](#apidoc.module.passport-facebook.super_.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.</span>InternalOAuthError (message, err)](#apidoc.element.passport-facebook.super_.InternalOAuthError.InternalOAuthError)

#### [module passport-facebook.super_.InternalOAuthError.prototype](#apidoc.module.passport-facebook.super_.InternalOAuthError.prototype)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.InternalOAuthError.prototype.</span>toString ()](#apidoc.element.passport-facebook.super_.InternalOAuthError.prototype.toString)

#### [module passport-facebook.super_.prototype](#apidoc.module.passport-facebook.super_.prototype)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>_createOAuthError (message, err)](#apidoc.element.passport-facebook.super_.prototype._createOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>_loadUserProfile (accessToken, done)](#apidoc.element.passport-facebook.super_.prototype._loadUserProfile)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>authenticate (req, options)](#apidoc.element.passport-facebook.super_.prototype.authenticate)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>authorizationParams (options)](#apidoc.element.passport-facebook.super_.prototype.authorizationParams)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>parseErrorResponse (body, status)](#apidoc.element.passport-facebook.super_.prototype.parseErrorResponse)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>tokenParams (options)](#apidoc.element.passport-facebook.super_.prototype.tokenParams)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>userProfile (accessToken, done)](#apidoc.element.passport-facebook.super_.prototype.userProfile)

#### [module passport-facebook.super_.super_](#apidoc.module.passport-facebook.super_.super_)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.</span>super_ ()](#apidoc.element.passport-facebook.super_.super_.super_)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.super_.</span>Strategy ()](#apidoc.element.passport-facebook.super_.super_.Strategy)

#### [module passport-facebook.super_.super_.prototype](#apidoc.module.passport-facebook.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">passport-facebook.super_.super_.prototype.</span>authenticate (req, options)](#apidoc.element.passport-facebook.super_.super_.prototype.authenticate)



# <a name="apidoc.module.passport-facebook"></a>[module passport-facebook](#apidoc.module.passport-facebook)

#### <a name="apidoc.element.passport-facebook.Strategy"></a>[function <span class="apidocSignatureSpan">passport-facebook.</span>Strategy (options, verify)](#apidoc.element.passport-facebook.Strategy)
- description and source-code
```javascript
function Strategy(options, verify) {
  options = options || {};
  options.authorizationURL = options.authorizationURL || 'https://www.facebook.com/dialog/oauth';
  options.tokenURL = options.tokenURL || 'https://graph.facebook.com/oauth/access_token';
  options.scopeSeparator = options.scopeSeparator || ',';

  OAuth2Strategy.call(this, options, verify);
  this.name = 'facebook';
  this._profileURL = options.profileURL || 'https://graph.facebook.com/v2.5/me';
  this._profileFields = options.profileFields || null;
  this._enableProof = options.enableProof;
  this._clientSecret = options.clientSecret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-facebook.super_"></a>[function <span class="apidocSignatureSpan">passport-facebook.</span>super_ (options, verify)](#apidoc.element.passport-facebook.super_)
- description and source-code
```javascript
function OAuth2Strategy(options, verify) {
  if (typeof options == 'function') {
    verify = options;
    options = undefined;
  }
  options = options || {};

  if (!verify) { throw new TypeError('OAuth2Strategy requires a verify callback'); }
  if (!options.authorizationURL) { throw new TypeError('OAuth2Strategy requires a authorizationURL option'); }
  if (!options.tokenURL) { throw new TypeError('OAuth2Strategy requires a tokenURL option'); }
  if (!options.clientID) { throw new TypeError('OAuth2Strategy requires a clientID option'); }

  passport.Strategy.call(this);
  this.name = 'oauth2';
  this._verify = verify;

  // NOTE: The _oauth2 property is considered "protected".  Subclasses are
  //       allowed to use it when making protected resource requests to retrieve
  //       the user profile.
  this._oauth2 = new OAuth2(options.clientID,  options.clientSecret,
      '', options.authorizationURL, options.tokenURL, options.customHeaders);

  this._callbackURL = options.callbackURL;
  this._scope = options.scope;
  this._scopeSeparator = options.scopeSeparator || ' ';
  this._key = options.sessionKey || ('oauth2:' + url.parse(options.authorizationURL).hostname);

  if (options.store) {
    this._stateStore = options.store;
  } else {
    if (options.state) {
      this._stateStore = new SessionStateStore({ key: this._key });
    } else {
      this._stateStore = new NullStateStore();
    }
  }
  this._trustProxy = options.proxy;
  this._passReqToCallback = options.passReqToCallback;
  this._skipUserProfile = (options.skipUserProfile === undefined) ? false : options.skipUserProfile;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-facebook.super_.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-facebook.</span>super_.InternalOAuthError (message, err)](#apidoc.element.passport-facebook.super_.InternalOAuthError)
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

#### <a name="apidoc.element.passport-facebook.super_.super_"></a>[function <span class="apidocSignatureSpan">passport-facebook.</span>super_.super_ ()](#apidoc.element.passport-facebook.super_.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-facebook.profile"></a>[module passport-facebook.profile](#apidoc.module.passport-facebook.profile)

#### <a name="apidoc.element.passport-facebook.profile.parse"></a>[function <span class="apidocSignatureSpan">passport-facebook.profile.</span>parse (json)](#apidoc.element.passport-facebook.profile.parse)
- description and source-code
```javascript
parse = function (json) {
  if ('string' == typeof json) {
    json = JSON.parse(json);
  }

  var profile = {};
  profile.id = json.id;
  profile.username = json.username;
  profile.displayName = json.name;
  profile.name = { familyName: json.last_name,
                   givenName: json.first_name,
                   middleName: json.middle_name };

  profile.gender = json.gender;
  profile.profileUrl = json.link;

  if (json.email) {
    profile.emails = [{ value: json.email }];
  }

  if (json.picture) {
    if (typeof json.picture == 'object' && json.picture.data) {
      // October 2012 Breaking Changes
      profile.photos = [{ value: json.picture.data.url }];
    } else {
      profile.photos = [{ value: json.picture }];
    }
  }

  return profile;
}
```
- example usage
```shell
...
 *
 * @param {object|string} json
 * @return {object}
 * @access public
 */
exports.parse = function(json) {
if ('string' == typeof json) {
  json = JSON.parse(json);
}

var profile = {};
profile.id = json.id;
profile.username = json.username;
profile.displayName = json.name;
profile.name = { familyName: json.last_name,
...
```



# <a name="apidoc.module.passport-facebook.super_"></a>[module passport-facebook.super_](#apidoc.module.passport-facebook.super_)

#### <a name="apidoc.element.passport-facebook.super_.super_"></a>[function <span class="apidocSignatureSpan">passport-facebook.</span>super_ ()](#apidoc.element.passport-facebook.super_.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-facebook.super_.AuthorizationError"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.</span>AuthorizationError (message, code, uri, status)](#apidoc.element.passport-facebook.super_.AuthorizationError)
- description and source-code
```javascript
function AuthorizationError(message, code, uri, status) {
  if (!status) {
    switch (code) {
      case 'access_denied': status = 403; break;
      case 'server_error': status = 502; break;
      case 'temporarily_unavailable': status = 503; break;
    }
  }

  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.code = code || 'server_error';
  this.uri = uri;
  this.status = status || 500;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-facebook.super_.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.</span>InternalOAuthError (message, err)](#apidoc.element.passport-facebook.super_.InternalOAuthError)
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

#### <a name="apidoc.element.passport-facebook.super_.Strategy"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.</span>Strategy (options, verify)](#apidoc.element.passport-facebook.super_.Strategy)
- description and source-code
```javascript
function OAuth2Strategy(options, verify) {
  if (typeof options == 'function') {
    verify = options;
    options = undefined;
  }
  options = options || {};

  if (!verify) { throw new TypeError('OAuth2Strategy requires a verify callback'); }
  if (!options.authorizationURL) { throw new TypeError('OAuth2Strategy requires a authorizationURL option'); }
  if (!options.tokenURL) { throw new TypeError('OAuth2Strategy requires a tokenURL option'); }
  if (!options.clientID) { throw new TypeError('OAuth2Strategy requires a clientID option'); }

  passport.Strategy.call(this);
  this.name = 'oauth2';
  this._verify = verify;

  // NOTE: The _oauth2 property is considered "protected".  Subclasses are
  //       allowed to use it when making protected resource requests to retrieve
  //       the user profile.
  this._oauth2 = new OAuth2(options.clientID,  options.clientSecret,
      '', options.authorizationURL, options.tokenURL, options.customHeaders);

  this._callbackURL = options.callbackURL;
  this._scope = options.scope;
  this._scopeSeparator = options.scopeSeparator || ' ';
  this._key = options.sessionKey || ('oauth2:' + url.parse(options.authorizationURL).hostname);

  if (options.store) {
    this._stateStore = options.store;
  } else {
    if (options.state) {
      this._stateStore = new SessionStateStore({ key: this._key });
    } else {
      this._stateStore = new NullStateStore();
    }
  }
  this._trustProxy = options.proxy;
  this._passReqToCallback = options.passReqToCallback;
  this._skipUserProfile = (options.skipUserProfile === undefined) ? false : options.skipUserProfile;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-facebook.super_.TokenError"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.</span>TokenError (message, code, uri, status)](#apidoc.element.passport-facebook.super_.TokenError)
- description and source-code
```javascript
function TokenError(message, code, uri, status) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.code = code || 'invalid_request';
  this.uri = uri;
  this.status = status || 500;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-facebook.super_.InternalOAuthError"></a>[module passport-facebook.super_.InternalOAuthError](#apidoc.module.passport-facebook.super_.InternalOAuthError)

#### <a name="apidoc.element.passport-facebook.super_.InternalOAuthError.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.</span>InternalOAuthError (message, err)](#apidoc.element.passport-facebook.super_.InternalOAuthError.InternalOAuthError)
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



# <a name="apidoc.module.passport-facebook.super_.InternalOAuthError.prototype"></a>[module passport-facebook.super_.InternalOAuthError.prototype](#apidoc.module.passport-facebook.super_.InternalOAuthError.prototype)

#### <a name="apidoc.element.passport-facebook.super_.InternalOAuthError.prototype.toString"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.InternalOAuthError.prototype.</span>toString ()](#apidoc.element.passport-facebook.super_.InternalOAuthError.prototype.toString)
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



# <a name="apidoc.module.passport-facebook.super_.prototype"></a>[module passport-facebook.super_.prototype](#apidoc.module.passport-facebook.super_.prototype)

#### <a name="apidoc.element.passport-facebook.super_.prototype._createOAuthError"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>_createOAuthError (message, err)](#apidoc.element.passport-facebook.super_.prototype._createOAuthError)
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

#### <a name="apidoc.element.passport-facebook.super_.prototype._loadUserProfile"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>_loadUserProfile (accessToken, done)](#apidoc.element.passport-facebook.super_.prototype._loadUserProfile)
- description and source-code
```javascript
_loadUserProfile = function (accessToken, done) {
  var self = this;

  function loadIt() {
    return self.userProfile(accessToken, done);
  }
  function skipIt() {
    return done(null);
  }

  if (typeof this._skipUserProfile == 'function' && this._skipUserProfile.length > 1) {
    // async
    this._skipUserProfile(accessToken, function(err, skip) {
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

#### <a name="apidoc.element.passport-facebook.super_.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>authenticate (req, options)](#apidoc.element.passport-facebook.super_.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (req, options) {
  options = options || {};
  var self = this;

  if (req.query && req.query.error) {
    if (req.query.error == 'access_denied') {
      return this.fail({ message: req.query.error_description });
    } else {
      return this.error(new AuthorizationError(req.query.error_description, req.query.error, req.query.error_uri));
    }
  }

  var callbackURL = options.callbackURL || this._callbackURL;
  if (callbackURL) {
    var parsed = url.parse(callbackURL);
    if (!parsed.protocol) {
      // The callback URL is relative, resolve a fully qualified URL from the
      // URL of the originating request.
      callbackURL = url.resolve(utils.originalURL(req, { proxy: this._trustProxy }), callbackURL);
    }
  }

  var meta = {
    authorizationURL: this._oauth2._authorizeUrl,
    tokenURL: this._oauth2._accessTokenUrl,
    clientID: this._oauth2._clientId
  }

  if (req.query && req.query.code) {
    function loaded(err, ok, state) {
      if (err) { return self.error(err); }
      if (!ok) {
        return self.fail(state, 403);
      }

      var code = req.query.code;

      var params = self.tokenParams(options);
      params.grant_type = 'authorization_code';
      if (callbackURL) { params.redirect_uri = callbackURL; }

      self._oauth2.getOAuthAccessToken(code, params,
        function(err, accessToken, refreshToken, params) {
          if (err) { return self.error(self._createOAuthError('Failed to obtain access token', err)); }

          self._loadUserProfile(accessToken, function(err, profile) {
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
                  self._verify(req, accessToken, refreshToken, params, profile, verified);
                } else { // arity == 5
                  self._verify(req, accessToken, refreshToken, profile, verified);
                }
              } else {
                var arity = self._verify.length;
                if (arity == 5) {
                  self._verify(accessToken, refreshToken, params, profile, verified);
                } else { // arity == 4
                  self._verify(accessToken, refreshToken, profile, verified);
                }
              }
            } catch (ex) {
              return self.error(ex);
            }
          });
        }
      );
    }

    var state = req.query.state;
    try {
      var arity = this._stateStore.verify.length;
      if (arity == 4) {
        this._stateStore.verify(req, state, meta, loaded);
      } else { // arity == 3
        this._stateStore.verify(req, state, loaded);
      }
    } catch (ex) {
      return this.error(ex);
    }
  } else {
    var params = this.authorizationParams(options);
    params.response_type = 'code';
    if (callbackURL) { params.redirect_uri = callbackURL; }
    var scope = options.scope || this._scope;
    if (scope) {
      if (Array.isArray(scope)) { scope = scope.join(this._scopeSeparator); }
      params.scope = scope;
    }

    var state = options.state;
    if (state) {
      params.state = state;

      var parsed = url.parse(this._oauth2._authorizeUrl, true);
      utils.merge(parsed.query, params);
      parsed.query['client_id'] = this._oauth2._clientId;
      delete parsed.search;
      var location = url.format(parsed);
      this.redirect(location);
    } else {
      function stored(err, state) {
        if (err) { return self.error(err); }

        if (state) { params.state = state; }
        var parsed = url.parse(self._oauth2._authorizeUrl, true);
        utils.merge(parsed.query, params);
        parsed.query['client_id'] = self._oauth2._clientId;
        delete parsed.search; ...
```
- example usage
```shell
...
    });
  }
));
'''

#### Authenticate Requests

Use 'passport.authenticate()', specifying the ''facebook'' strategy, to
authenticate requests.

For example, as route middleware in an [Express](http://expressjs.com/)
application:

'''js
app.get('/auth/facebook',
...
```

#### <a name="apidoc.element.passport-facebook.super_.prototype.authorizationParams"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>authorizationParams (options)](#apidoc.element.passport-facebook.super_.prototype.authorizationParams)
- description and source-code
```javascript
authorizationParams = function (options) {
  return {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-facebook.super_.prototype.parseErrorResponse"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>parseErrorResponse (body, status)](#apidoc.element.passport-facebook.super_.prototype.parseErrorResponse)
- description and source-code
```javascript
parseErrorResponse = function (body, status) {
  var json = JSON.parse(body);
  if (json.error) {
    return new TokenError(json.error_description, json.error, json.error_uri);
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-facebook.super_.prototype.tokenParams"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>tokenParams (options)](#apidoc.element.passport-facebook.super_.prototype.tokenParams)
- description and source-code
```javascript
tokenParams = function (options) {
  return {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-facebook.super_.prototype.userProfile"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.prototype.</span>userProfile (accessToken, done)](#apidoc.element.passport-facebook.super_.prototype.userProfile)
- description and source-code
```javascript
userProfile = function (accessToken, done) {
  return done(null, {});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-facebook.super_.super_"></a>[module passport-facebook.super_.super_](#apidoc.module.passport-facebook.super_.super_)

#### <a name="apidoc.element.passport-facebook.super_.super_.super_"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.</span>super_ ()](#apidoc.element.passport-facebook.super_.super_.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-facebook.super_.super_.Strategy"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.super_.</span>Strategy ()](#apidoc.element.passport-facebook.super_.super_.Strategy)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-facebook.super_.super_.prototype"></a>[module passport-facebook.super_.super_.prototype](#apidoc.module.passport-facebook.super_.super_.prototype)

#### <a name="apidoc.element.passport-facebook.super_.super_.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">passport-facebook.super_.super_.prototype.</span>authenticate (req, options)](#apidoc.element.passport-facebook.super_.super_.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (req, options) {
  throw new Error('Strategy#authenticate must be overridden by subclass');
}
```
- example usage
```shell
...
    });
  }
));
'''

#### Authenticate Requests

Use 'passport.authenticate()', specifying the ''facebook'' strategy, to
authenticate requests.

For example, as route middleware in an [Express](http://expressjs.com/)
application:

'''js
app.get('/auth/facebook',
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
