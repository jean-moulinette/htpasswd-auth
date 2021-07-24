# htpasswd-authenticator

Forked from [dickeyxxx's htpasswd-auth](https://github.com/dickeyxxx/htpasswd-auth)
This fork contains updated hash node modules which allows usage for node >8

read/write htpasswd files

## Setup

```js
npm install --save htpasswd-auth
```

## Checking if a password is valid

```js
var htpasswd = require('htpasswd-authenticator');
var file     = fs.readFileSync('./path-to-htpasswd', 'utf-8');

htpasswd.authenticate('dickeyxxx', 'pass', file)
.then(function (auth) {
  // auth is true if the password is valid
});
```
