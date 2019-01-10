### Cookies
---
https://github.com/ScottHamper/Cookies

```
npm install cookies-js
bower install cookies-js
```

```js
var jsdom = require('jsdom');
var window = jsdom.jsdom().parentWindow;
var Cookies = require('cookies-js')(window);

Cookies.set('key', 'value');
Cookies.set('key', 'value').set('hello', 'world');
Cookies.set('key', 'value', { domain: 'www.example.com', secure: true });
Cookies.set('key', 'value', { expires: 600 });
Cookies.set('key', 'value', { expires: '01/01/2012' });
Cookies.set('key', 'value', { expires: new Date(2012, 0, 1) });
Cookies.set('key', 'value', { expires: Infinity });
Cookies('key', 'value', { secure: true });

Cookies.set('key', 'value');
Cookies.get('key');
Cookies('key');

Cookies.set('key', value).get('key');
Cookies.set('key').get('key');
Cookies('key', undefined);

if (Cookies.enabled){
  Cookies.set('key', 'value');
}

Cookies.defaults = {
  path: '/',
  secure: true
};
Cookies.set('key', 'value');
Cookies.expire('key');
```

```
```

