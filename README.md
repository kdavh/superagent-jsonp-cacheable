# superagent-jsonp-cacheable
Adds cacheable jsonp behaviour to superagent. Basically a copy of superagent-jsonp package with a line change to allow caching.  Thanks to @lamp.

## To use with browserify

First install with npm

``` npm i superagent-jsonp-cacheable --save ```

Then use like so;

```js
var superagent = require('superagent');

let jsonp = require('superagent-jsonp-cacheable');

superagent.get('http://example.com/foo.json').use(jsonp).end(function(err, res){
  // everything is as normal
});

```

## To use with bower

First install:

``` bower i superagent-jsonp-cacheable --save```

Include it from your bower components in the usual way

Then use pretty much as you do above

```js
superagent.get('http://example.com/foo.json').use(superagentJSONP).end(function(err, res){
  // everything is as normal
});
```
